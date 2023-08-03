# Comparing `tmp/abstract_modules-0.0.1.0-py3-none-any.whl.zip` & `tmp/abstract_modules-0.0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 7729 bytes, number of entries: 8
+Zip file size: 18467 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       40 b- defN 23-Aug-02 04:34 abstract_modules/__init__.py
+-rw-r--r--  2.0 unx    32997 b- defN 23-Aug-03 04:11 abstract_modules/create_module_folder.py
 -rw-r--r--  2.0 unx     1290 b- defN 23-Aug-02 04:34 abstract_modules/main.py
--rw-r--r--  2.0 unx     3407 b- defN 23-Aug-02 06:19 abstract_modules/module_utils.py
--rw-r--r--  2.0 unx     9008 b- defN 23-Aug-02 07:25 abstract_modules/upload_utils.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Aug-02 07:26 abstract_modules-0.0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 07:26 abstract_modules-0.0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Aug-02 07:26 abstract_modules-0.0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      684 b- defN 23-Aug-02 07:26 abstract_modules-0.0.1.0.dist-info/RECORD
-8 files, 18488 bytes uncompressed, 6523 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     3681 b- defN 23-Aug-02 08:02 abstract_modules/module_utils.py
+-rw-r--r--  2.0 unx    10684 b- defN 23-Aug-03 07:00 abstract_modules/upload_utils.py
+-rw-r--r--  2.0 unx     3950 b- defN 23-Aug-03 07:52 abstract_modules-0.0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 07:52 abstract_modules-0.0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Aug-03 07:52 abstract_modules-0.0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      783 b- defN 23-Aug-03 07:52 abstract_modules-0.0.1.1.dist-info/RECORD
+9 files, 53534 bytes uncompressed, 17105 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: abstract_modules/__init__.py
 Comment: 
 
+Filename: abstract_modules/create_module_folder.py
+Comment: 
+
 Filename: abstract_modules/main.py
 Comment: 
 
 Filename: abstract_modules/module_utils.py
 Comment: 
 
 Filename: abstract_modules/upload_utils.py
 Comment: 
 
-Filename: abstract_modules-0.0.1.0.dist-info/METADATA
+Filename: abstract_modules-0.0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: abstract_modules-0.0.1.0.dist-info/WHEEL
+Filename: abstract_modules-0.0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: abstract_modules-0.0.1.0.dist-info/top_level.txt
+Filename: abstract_modules-0.0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: abstract_modules-0.0.1.0.dist-info/RECORD
+Filename: abstract_modules-0.0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abstract_modules/module_utils.py

```diff
@@ -1,21 +1,23 @@
 import os
 import ast
 import re
 from abstract_gui import get_browser
 import pkg_resources
-
 def scan_folder_for_required_modules(folder_path=None):
     """
     Scan the specified folder for Python files and create a list of necessary Python modules.
     :param folder_path: The path of the folder to scan. If None, a folder will be picked using a GUI window.
     :return: A list of required Python modules based on all Python files found in the folder.
     """
     if folder_path is None:
-        folder_path = get_browser(title="please choose the destination for your import scripts to be analyzed",initial_folder=os.getcwd())["output"]
+        folder_path = get_browser(
+            title="Please choose the destination for your import scripts to be analyzed",
+            initial_folder=os.getcwd()
+        )["output"]
 
     required_modules = set()
 
     def visit_file(file_path):
         try:
             with open(file_path, 'r', encoding='utf-8') as file:
                 tree = ast.parse(file.read())
@@ -35,19 +37,23 @@
             pass
 
     for root, _, files in os.walk(folder_path):
         for file in files:
             if file.endswith('.py'):
                 file_path = os.path.join(root, file)
                 visit_file(file_path)
-    required_list = []
-    for each in list(required_modules):
-        each = each.split('.')[0]
-        if each not in required_list:
-            required_list.append(each)
+                
+    # Update the required_modules to include submodules
+    updated_required_modules = set()
+    for module in required_modules:
+        parts = module.split('.')
+        for i in range(len(parts)):
+            updated_required_modules.add('.'.join(parts[:i+1]))
+
+    required_list = list(updated_required_modules)
     return required_list
 def is_valid_package_name(package_name):
     # Python package names must start with a letter and can only contain ASCII letters, numbers, and underscores
     return re.match(r'^[a-zA-Z][a-zA-Z0-9_]*$', package_name) is not None
 
 def get_installed_versions(install_requires):
     """
@@ -74,7 +80,8 @@
             installed_versions.append(f'{module_name}>={version}')
         elif '==' in requirement:
             installed_versions.append(f'{module_name}=={version}')
         else:
             installed_versions.append(f'{module_name}>={version}')
 
     return installed_versions
+input(get_installed_versions(scan_folder_for_required_modules(folder_path=None)))
```

## abstract_modules/upload_utils.py

```diff
@@ -10,15 +10,15 @@
 windows_mgr,bridge,script_name=create_window_manager(global_var=globals())
 def get_parent_directory(directory:str=os.getcwd()):
     browser_values = None
     while browser_values == None:
         browser_values = get_browser(title="pick a module directory", type="folder", initial_folder=directory)
     # Now you can access the "Browse" key from browser_values dictionary
     if browser_values and "output" in browser_values:
-        globals()['parent_dir'] = browser_values["output"]
+        return browser_values["output"]
         # Just for debugging purposes, you can remove this line once it's working correctly
 # Call the function to test it
 
 def get_output_text():
     return os.path.join(parent_dir,'output.txt')
 def get_src_dir():
     globals()['src_dir'] = os.path.join(parent_dir,project,"src")
@@ -33,130 +33,163 @@
     if not os.path.exists("dist"):
         os.makedirs("dist")
     return "sudo python3 setup.py bdist_wheel"
 def module_upload_cmd():
     return "python3 -m twine upload dist/*.whl --skip-existing"
 def upload_module():
     return pexpect_cmd_with_args(command=module_upload_cmd(),child_runs=[{"prompt":"Enter your username: ","pass":None,"key":"PYPI_USERNAME"},{"prompt":"Enter your password: ","pass":None,"key":"PYPI_PASSWORD"}],output_text=get_output_text())
-def save_new_setup(setup_file):
-    with open('setup.py', 'w', encoding='utf-8') as fh:
-        fh.write(setup_file)
-def read_setup():
-    with open('setup.py', 'r', encoding='utf-8') as fh:
+def save_new_setup(contents,directory:str=os.getcwd()):
+    if os.path.isdir(directory):
+        if os.path.isfile(os.path.join(directory,'setup.py')):
+          filepath= os.path.join(directory,'setup.py')
+    elif os.path.isfile(directory):
+        if os.path.basename(directory) =='setup.py':
+            filepath = directory
+            directory = directory[:-len('setup.py')]
+    with open(filepath, 'w', encoding='utf-8') as fh:
+        fh.write(contents)
+def read_setup(directory:str=os.getcwd()):
+    if os.path.isdir(directory):
+        if os.path.isfile(os.path.join(directory,'setup.py')):
+          filepath= os.path.join(directory,'setup.py')
+    elif os.path.isfile(directory):
+        if os.path.basename(directory) =='setup.py':
+            filepath = directory
+            directory = directory[:-len('setup.py')]
+    with open(filepath, 'r', encoding='utf-8') as fh:
         setup_file = fh.read()
     cleaner_ls =['',' ','\n','\t','"',"'"]
     version = eatAll(x=setup_file.split('version=')[-1].split(',')[0],ls=cleaner_ls)
     name= eatAll(x=setup_file.split('name=')[-1].split(',')[0],ls=cleaner_ls)
     url = eatAll(x=setup_file.split('url=')[-1].split(',')[0],ls=cleaner_ls)
     install_requires = eatAll(x=setup_file.split('install_requires=')[-1].split(']')[0]+']',ls=cleaner_ls)
-    return {"file":setup_file,"version":version,"name":name,"url":url,"install_requires":install_requires}
+    return {"filepath":filepath,"directory":directory,"file":setup_file,"version":version,"name":name,"url":url,"install_requires":install_requires}
 def get_url(setup_js):
     if setup_js["url"].split('/')[-1] != setup_js["name"]:
         url_new = setup_js["url"][:-len(setup_js["url"].split('/')[-1])]+setup_js["name"]
         permission = get_yes_no(text=f"would you like to change the url requires from {setup_js['url']} to {url_new}?'")
         windows_mgr.while_quick(windows_mgr.get_new_window(title='version number', args={"layout": [
                 [[get_gui_fun("T", {"text": "would you like to change the url requires from {setup_js['url']} to {url_new}?"})],
                 [get_gui_fun('Input', {"default_text": url_new, "key": "output"})],
                 [sg.Button("OK")]]]},exit_events=["OK","Override"]))["output"]
         if permission == 'Yes':
-            save_new_setup(read_setup()["file"].replace(install_requires,install_requires_new))
+            save_new_setup(directory=setup_js['filepath'],contents=read_setup(setup_js['filepath'])["file"].replace(install_requires,install_requires_new))
 def get_install_requires(setup_js):
     install_requires_new = get_installed_versions(scan_folder_for_required_modules())
     if setup_js['install_requires'] != install_requires_new:
         permission = get_yes_no(text=f"would you like to change the install requires from {setup_js['install_requires']} to {install_requires_new}?'")
         if permission == 'Yes':
-            save_new_setup(read_setup()["file"].replace(str(setup_js['install_requires']),str(install_requires_new)))
+            save_new_setup(directory=setup_js['filepath'],contents=read_setup(setup_js['filepath'])["file"].replace(str(setup_js['install_requires']),str(install_requires_new)))
 def organize_versions_from_high_to_low(version_list):
     """
     Organize the list of version numbers from highest to lowest.
     :param version_list: A list of version numbers to organize.
     :return: A new list of version numbers sorted from highest to lowest.
     """
     sorted_versions = sorted(version_list, key=lambda x: list(map(int, x.split('.'))), reverse=True)
     return sorted_versions
 
-def get_distributions_from_packages(setup_js,version_numbers):
-    if os.path.isdir('dist'):
-        dist_list = os.listdir('dist')
+def get_distributions_from_packages(setup_js,version_numbers:list=[]):
+    dist_dir = os.path.join(setup_js['directory'],'dist')
+    if os.path.isdir(dist_dir):
+        dist_list = os.listdir(dist_dir)
         for dist in dist_list:
             rest = dist[len(setup_js['name'] + '-'):]
             version = ''
             while len(rest) > 0 and rest[0] in '0123456789.':
                 version += rest[0]
                 rest = rest[1:]
             version = version.rstrip('.')
             if version not in version_numbers:
                 version_numbers.append(version)
     return version_numbers
-def get_version_text(current_version,version_numbers):
+def get_version_input(highest):
     text = ''
-    version_number_exists = False
-    version_number_highest = True
-    if current_version not in version_numbers:
-        version_numbers.append(current_version)
-    else:
-        version_number_exists = True
-        text = f'Version number {current_version} already exists.'
-    version_numbers = organize_versions_from_high_to_low(version_numbers)
-    if version_numbers[0] != current_version:
-        version_number_highest = False
-        text = text + f" Your version number {current_version} is lower than the highest version number {version_numbers[0]}."
-    return text,version_number_highest
-def get_distributions(setup_js):
-   
-    version_numbers = get_distributions_from_packages(setup_js,[])
-    installed_versions = get_installed_versions(setup_js['name'])
-    for version in installed_versions:
-        version_number = version.split('=')[-1]
-        if version_number not in version_numbers:
-            version_numbers.append(version_number)
-    new_version = setup_js['version']
-    
-    while get_version_text(new_version,version_numbers)[1] !=True:
-        text = get_version_text(new_version,version_numbers)[0] +' please enter a new version number'
-        layout = [
-            [get_gui_fun("T", {"text": text})],
-            [get_gui_fun('Input', {"default_text": organize_versions_from_high_to_low(version_numbers)[0], "key": "version_number"})],
-            [sg.Button("OK")]
-        ]
-        new_version = windows_mgr.while_basic(windows_mgr.get_new_window(title='Version number', args={"layout": layout},exit_events=["OK", "Override"]))["version_number"]
-        setup_file = read_setup()["file"].replace(setup_js['version'], new_version)
-        override_prompt = f"Would you like to override the version number with {new_version}?"
-        override = get_yes_no(text=override_prompt)
-        if override == "Yes":
+    if highest["exists"] == True:
+        text += f"Version number {highest['version']} already exists."
+    if highest["exists"] == True:
+        text += f"Version number {highest['version']} does not exist."
+    if highest["bool"] == False:
+        text += f"\nYour version number {highest['version']} is lower than the highest version number {highest['highest']}."
+    if highest["bool"] == True:
+        text += f"\nYour version number {highest['version']} is the highest version number found."
+    text += '\n\nplease enter a new version number:'
+    layout = [
+        [get_gui_fun("T", {"text": text})],
+        [get_gui_fun('Input', {"default_text": highest['highest'], "key": "version_number"})],
+        [sg.Button("OK")]
+    ]
+    new_version = windows_mgr.while_basic(windows_mgr.get_new_window(title='Version number', args={"layout": layout},exit_events=["OK", "Override"]))["version_number"]
+    return new_version
+def get_highest(distributions,version):
+    highest = {"bool":False,"version":version,"highest":version,"exists":False}
+    if highest['version'] in distributions:
+        highest["bool"] = False
+        highest["highest"] = distributions[0]
+        highest["exists"] = True
+    if highest['version'] not in distributions:
+        highest["exists"] = False
+        curr_high = organize_versions_from_high_to_low([distributions[0],version])
+        if curr_high[0] == version:
+            highest["bool"]=True
+            highest["highest"] = version
+        if curr_high[0] != version:
+            highest["bool"]=False
+            highest["highest"] = curr_high[0]
+    return highest
+def get_all_versions(distributions,installed):
+    if len(installed) != 0:
+        if '=' in installed[0]:
+            version_number = installed[0].split('=')[-1]
+    if version_number not in distributions:
+        distributions.append(version_number)
+    return organize_versions_from_high_to_low(distributions)
+def finalize_version(setup_js):
+    version = setup_js['version']
+    distributions = get_all_versions(get_distributions_from_packages(setup_js),get_installed_versions([setup_js['name']]))
+    while True:
+        highest = get_highest(distributions,version)
+        if highest["bool"] == False:
+            new_version=get_version_input(highest)
+            if highest['highest'] == organize_versions_from_high_to_low([highest['highest'],new_version])[0]:
+                override_prompt = f"this is still not the highest version number;\nWould you like to override the version number with {new_version}?"
+                override = get_yes_no(text=override_prompt)
+                if override == "Yes":
+                    break
+            else:
+                version = new_version
+        if highest["bool"] == True and highest["exists"] == False:
             break
-
-    globals()["version_current"] = new_version
-    # Save the updated version in setup.py
-    save_new_setup(setup_file = read_setup()['file'].replace(setup_js['version'], new_version))
+    save_new_setup(directory=setup_js['filepath'],contents=read_setup(setup_js['filepath'])["file"].replace(str(setup_js['version']),str(version)))
 def install_module(event):
     if event == "install":
         cmd_run(f'pip install {read_setup()["name"]}=={read_setup()["version"]} --break-system-packages')
 def install_mods_layout():
     win=windows_mgr.get_new_window(title="install module",layout=[[get_gui_fun('Button',{'button_text':'install_module','key':'install'}),get_gui_fun('Button',{'button_text':'exit','key':'EXIT'})]],event_function='install_module')
     while True:
         events = windows_mgr.while_basic(window=win)
         if events == None:
             return 
 def get_list_of_projects():
     win=windows_mgr.get_new_window(title="list_window",layout=[[get_gui_fun('Listbox',{"values":os.listdir(parent_dir),"size":(25,10),'key':'projects',"enable_events":True}),get_gui_fun('Button',{'button_text':'submit','key':'exit'})]])
     globals()['project'] = windows_mgr.while_basic(window=win)['projects'][0]
-def run_setup_loop():
-    cmd_run_sudo(cmd=install_twine(),key="SUDO_PASSWORD",output_text="/home/john-putkey/Documents/python_projects/modules/abstract_essentials/output.txt")
+def run_setup_loop(directory:str=os.getcwd()):
+    globals()['parent_dir'] = directory
+    output_text = os.path.join(parent_dir,"output.txt")
+    cmd_run_sudo(cmd=install_twine(),key="SUDO_PASSWORD",output_text=output_text)
     get_list_of_projects()
     get_src_dir()
     get_project_dirs()
     globals()['project_dir'] = os.path.join(parent_dir,project)
     os.chdir(project_dir)
     setup_js = read_setup()
-    get_distributions(setup_js)
+    finalize_version(setup_js)
     get_install_requires(setup_js)
     get_url(setup_js)
     print(f"Running setup.py for project: {project_dir}")
-    cmd_run_sudo(cmd=install_setup(),key="SUDO_PASSWORD",output_text="/home/john-putkey/Documents/python_projects/modules/abstract_essentials/output.txt")
-    cmd_run_sudo(cmd=build_module(),key="SUDO_PASSWORD",output_text="/home/john-putkey/Documents/python_projects/modules/abstract_essentials/output.txt")
+    cmd_run_sudo(cmd=install_setup(),key="SUDO_PASSWORD",output_text=output_text)
+    cmd_run_sudo(cmd=build_module(),key="SUDO_PASSWORD",output_text=output_text)
     upload_module()
     print(f"Completed setup.py for project: {project_dir}")
     install_mods_layout()
 def upload_main(directory:str=os.getcwd()):
-    get_parent_directory(directory)
-    run_setup_loop()
+    run_setup_loop(get_parent_directory(directory))
```

## Comparing `abstract_modules-0.0.1.0.dist-info/METADATA` & `abstract_modules-0.0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: abstract-modules
-Version: 0.0.1.0
+Version: 0.0.1.1
 Summary: abstract_modules allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community..
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/tree/main/abstract_modules
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: abstract-gui (>=0.0.53.5)
-Requires-Dist: abstract-utilities (>=0.0.1700)
+Requires-Dist: abstract-utilities (>=0.0.1740)
 Requires-Dist: pexpect (>=4.8.0)
 
 #abstract_modules
 # Python Module Upload to PyPI
 
 This utility script allows you to easily upload your Python module to the Python Package Index (PyPI) using Twine. It automates several steps of the packaging and distribution process, making it easier to share your module with the Python community.
```

## Comparing `abstract_modules-0.0.1.0.dist-info/RECORD` & `abstract_modules-0.0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 abstract_modules/__init__.py,sha256=0LNjFqr-o-wHdm5LGqcJ2NyZGfe0l7_GunRKIl1PSvs,40
+abstract_modules/create_module_folder.py,sha256=Z1w1XX2beIfO2Hei4-0QKY6ROOw1kkWeOsYkZ2nQG3Y,32997
 abstract_modules/main.py,sha256=zrkeuBjXVoW_DfUx2uVV-mEWDUsnGgpwWPdkSYqhoT0,1290
-abstract_modules/module_utils.py,sha256=d9p1ayFVT1PQLX86e1L9kbwC1K6zcVwW6Yh-XueieKA,3407
-abstract_modules/upload_utils.py,sha256=cHyqRYMd25QUmfU54WQrNeOwTCvsV6bExaxSsonq8gE,9008
-abstract_modules-0.0.1.0.dist-info/METADATA,sha256=cpvsGlhcrvvmWHIlnDcHCZediIRm3RRe5ezHo5tDup8,3950
-abstract_modules-0.0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-abstract_modules-0.0.1.0.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
-abstract_modules-0.0.1.0.dist-info/RECORD,,
+abstract_modules/module_utils.py,sha256=nJW5qU1RuVg8Irm7p-KFvFzALjSLwfXQ2pGA62rteJw,3681
+abstract_modules/upload_utils.py,sha256=b7aDrnDZXjxB7NyOAWKSvl64Ma0wMmOzIG8hH5qHiRc,10684
+abstract_modules-0.0.1.1.dist-info/METADATA,sha256=35rjmz9D-51BBp45Hz4Zycub421b5pFlIFT29W5b0Tk,3950
+abstract_modules-0.0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+abstract_modules-0.0.1.1.dist-info/top_level.txt,sha256=f9o4Vw5Mulr8ed3JeHE83u5oi5GQ3By2vY_v5nbAEMM,17
+abstract_modules-0.0.1.1.dist-info/RECORD,,
```

