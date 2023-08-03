# Comparing `tmp/tgwrap-0.7.8.tar.gz` & `tmp/tgwrap-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.7.8.tar", max compression
+gzip compressed data, was "tgwrap-0.7.9.tar", max compression
```

## Comparing `tgwrap-0.7.8.tar` & `tgwrap-0.7.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.7.8/LICENSE
--rw-r--r--   0        0        0     8381 2023-06-21 12:44:31.502352 tgwrap-0.7.8/README.md
--rw-r--r--   0        0        0      902 2023-07-07 12:52:16.036468 tgwrap-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.7.8/tgwrap/__init__.py
--rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.7.8/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    26583 2023-07-07 08:50:53.225395 tgwrap-0.7.8/tgwrap/cli.py
--rwxr-xr-x   0        0        0    66391 2023-07-07 12:47:28.321787 tgwrap-0.7.8/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.7.8/tgwrap/printer.py
--rw-r--r--   0        0        0     9561 1970-01-01 00:00:00.000000 tgwrap-0.7.8/setup.py
--rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 tgwrap-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.7.9/LICENSE
+-rw-r--r--   0        0        0     8381 2023-06-21 12:44:31.502352 tgwrap-0.7.9/README.md
+-rw-r--r--   0        0        0      902 2023-08-02 12:41:12.851771 tgwrap-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.7.9/tgwrap/__init__.py
+-rw-r--r--   0        0        0     9164 2023-05-26 12:32:25.245403 tgwrap-0.7.9/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    26602 2023-08-02 12:32:22.264509 tgwrap-0.7.9/tgwrap/cli.py
+-rwxr-xr-x   0        0        0    66937 2023-08-02 12:38:01.263215 tgwrap-0.7.9/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.7.9/tgwrap/printer.py
+-rw-r--r--   0        0        0     9561 1970-01-01 00:00:00.000000 tgwrap-0.7.9/setup.py
+-rw-r--r--   0        0        0     9464 1970-01-01 00:00:00.000000 tgwrap-0.7.9/PKG-INFO
```

### Comparing `tgwrap-0.7.8/LICENSE` & `tgwrap-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.7.8/README.md` & `tgwrap-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.7.8/pyproject.toml` & `tgwrap-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.7.8"
+version = "0.7.9"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.7.8/tgwrap/analyze.py` & `tgwrap-0.7.9/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.7.8/tgwrap/cli.py` & `tgwrap-0.7.9/tgwrap/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,14 +599,15 @@
     required=True, default="manifest.yaml", show_default=True,
     )
 @click.option('--version-tag', '-V',
     help="Version tag, use 'latest' to, well, get the latest version.",
     required=True, default='latest', show_default=True,
     )
 @click.option('--target-stage', '-t',
+    multiple=True,
     help='Stage to deploy to',
     type=click.Choice(STAGES, case_sensitive=True), required=True,
     )
 @click.option('--include-global-config-files/--exclude-global-config-files', '-i/-x',
     help='Whether or not to include deploying the (in the manifest specified) global config files',
     is_flag=True, default=True, show_default=True,
     )
```

### Comparing `tgwrap-0.7.8/tgwrap/main.py` & `tgwrap-0.7.9/tgwrap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1140,20 +1140,14 @@
 
             # do we have a working dir? 
             working_dir = working_dir if working_dir else os.getcwd()
 
             manifest = self.load_yaml_file(os.path.join(working_dir, manifest_file))
 
             source_dir = os.path.join(temp_dir, manifest['base_path'])
-            target_dir = os.path.join(working_dir, target_stage)
-
-            try:
-                os.mkdir(target_dir)
-            except FileExistsError:
-                pass
 
             self._clone_repo(
                 manifest=manifest,
                 target_dir=temp_dir,
                 version_tag=version_tag,
                 )
 
@@ -1162,139 +1156,147 @@
             substacks = ['substacks', 'sub_stacks']
             for ss, substack in manifest.get('sub_stacks', {}).items():
                 # get the base directory of the sub stack so that we can ignore it when deploying the regular modules
                 substacks.append(substack['source'].split(os.path.sep)[0])
 
             substacks = set(substacks)
 
-            deploy_actions = {}
-            for key, value in manifest['deploy'].items():
-                if target_stage not in value['applies_to_stages']:
-                    self.printer.verbose(f'Target stage {target_stage} not applicable for action {key}.')
-                else:
-                    source_stage = value['source_stage']
-                    self.printer.verbose(f'Found deployment step {key} using source stage {source_stage}')
+            for stage in target_stage:
+                target_dir = os.path.join(working_dir, stage)
+                self.printer.header(f'Deploy stage {stage} to {target_dir}...')
+                try:
+                    os.mkdir(target_dir)
+                except FileExistsError:
+                    pass
+
+                deploy_actions = {}
+                for key, value in manifest['deploy'].items():
+                    if stage not in value['applies_to_stages']:
+                        self.printer.verbose(f'Target stage {stage} not applicable for action {key}.')
+                    else:
+                        source_stage = value['source_stage']
+                        self.printer.verbose(f'Found deployment step {key} using source stage {source_stage}')
 
-                    source_path = os.path.join(source_dir, source_stage)
-                    source_modules = {
-                        entry:{} for entry in os.listdir(source_path) if os.path.isdir(os.path.join(source_path, entry))
-                    }
-                    self.printer.verbose(f'Found modules: {source_modules}')
-
-                    include_modules = value['include_modules'] if len(value.get('include_modules', {})) > 0 else source_modules
-                    self.printer.verbose(f'Include modules: {include_modules}')
-
-                    # optionally, the moduels can be placed in another dir than the current
-                    base_dir = value.get('base_dir', '')
-
-                    for module, module_details in include_modules.items():
-                        source_module = module_details.get('source', module)
-                        target_module = module_details.get('target', module)
-
-                        full_source_path = os.path.join(source_path, source_module, '')
-                        full_target_path = os.path.join(target_dir, base_dir, target_module, '')
-
-                        if not os.path.isfile(os.path.join(full_source_path, self.TERRAGRUNT_FILE)):
-                            self.printer.warning(f'Module {source_module} seems substack and not a terragrunt module: skip it!')
-                        elif source_module in value.get('exclude_modules', []) or source_module in substacks:
-                            self.printer.verbose(f'Exclude module {source_module}')
-                        else:
-                            key = f'base -> {os.path.join(base_dir, module)}' if base_dir else module
-                            deploy_actions[key] = {
-                                "source": full_source_path,
-                                "target": full_target_path,
-                            }
+                        source_path = os.path.join(source_dir, source_stage)
+                        source_modules = {
+                            entry:{} for entry in os.listdir(source_path) if os.path.isdir(os.path.join(source_path, entry))
+                        }
+                        self.printer.verbose(f'Found modules: {source_modules}')
+
+                        include_modules = value['include_modules'] if len(value.get('include_modules', {})) > 0 else source_modules
+                        self.printer.verbose(f'Include modules: {include_modules}')
+
+                        # optionally, the moduels can be placed in another dir than the current
+                        base_dir = value.get('base_dir', '')
 
-                    for ss, substack in manifest.get('sub_stacks', {}).items():
-                        self.printer.verbose(f'Found substack : {ss}')
+                        for module, module_details in include_modules.items():
+                            source_module = module_details.get('source', module)
+                            target_module = module_details.get('target', module)
+
+                            full_source_path = os.path.join(source_path, source_module, '')
+                            full_target_path = os.path.join(target_dir, base_dir, target_module, '')
+
+                            if not os.path.isfile(os.path.join(full_source_path, self.TERRAGRUNT_FILE)):
+                                self.printer.warning(f'Module {source_module} seems substack and not a terragrunt module: skip it!')
+                            elif source_module in value.get('exclude_modules', []) or source_module in substacks:
+                                self.printer.verbose(f'Exclude module {source_module}')
+                            else:
+                                key = f'base -> {os.path.join(base_dir, module)}' if base_dir else module
+                                deploy_actions[key] = {
+                                    "source": full_source_path,
+                                    "target": full_target_path,
+                                }
+
+                        for ss, substack in manifest.get('sub_stacks', {}).items():
+                            self.printer.verbose(f'Found substack : {ss}')
+
+                            source_path = os.path.join(
+                                source_dir, source_stage, substack['source'], ''
+                                )
+                            target_path = os.path.join(
+                                target_dir, substack['target'], ''
+                                )
+
+                            include_modules = substack['include_modules'] if len(substack.get('include_modules', {})) > 0 else []
+                            self.printer.verbose(f'Include modules: {include_modules}')
+
+                            if include_modules:
+                                # get all directories in the substack and create an exlude_modules list from that
+                                source_directories = get_directories(source_path)
+                                exclude_modules = list(set(source_directories) - set(include_modules))
+                                print("Dirs: ", include_modules, source_directories, source_path, exclude_modules)
+                            else:
+                                exclude_modules = substack.get('exclude_modules', [])
+                            
+                            if os.path.exists(source_path):
+                                deploy_actions[f'substack -> {substack["target"]}'] = {
+                                    "source": source_path,
+                                    "target": target_path,
+                                    "excludes": exclude_modules,
+                                }
+                            else:
+                                self.printer.warning(f'Source path of substack does not exist: {source_path}')
+
+                if include_global_config_files:
+                    for gc, global_config in manifest.get('global_config_files', {}).items():
+                        self.printer.verbose(f'Found global config : {gc}')
 
                         source_path = os.path.join(
-                            source_dir, source_stage, substack['source'], ''
+                            source_dir, global_config['source']
                             )
+                        target = global_config.get('target', global_config['source'])
                         target_path = os.path.join(
-                            target_dir, substack['target'], ''
+                            working_dir, target,
                             )
 
-                        include_modules = substack['include_modules'] if len(substack.get('include_modules', {})) > 0 else []
-                        self.printer.verbose(f'Include modules: {include_modules}')
-
-                        if include_modules:
-                            # get all directories in the substack and create an exlude_modules list from that
-                            source_directories = get_directories(source_path)
-                            exclude_modules = list(set(source_directories) - set(include_modules))
-                            print("Dirs: ", include_modules, source_directories, source_path, exclude_modules)
-                        else:
-                            exclude_modules = substack.get('exclude_modules', [])
-                        
                         if os.path.exists(source_path):
-                            deploy_actions[f'substack -> {substack["target"]}'] = {
+                            deploy_actions[f'global configs -> {target}'] = {
                                 "source": source_path,
                                 "target": target_path,
-                                "excludes": exclude_modules,
                             }
                         else:
-                            self.printer.warning(f'Source path of substack does not exist: {source_path}')
-
-            if include_global_config_files:
-                for gc, global_config in manifest.get('global_config_files', {}).items():
-                    self.printer.verbose(f'Found global config : {gc}')
-
-                    source_path = os.path.join(
-                        source_dir, global_config['source']
-                        )
-                    target = global_config.get('target', global_config['source'])
-                    target_path = os.path.join(
-                        working_dir, target,
-                        )
-
-                    if os.path.exists(source_path):
-                        deploy_actions[f'global configs -> {target}'] = {
-                            "source": source_path,
-                            "target": target_path,
-                        }
-                    else:
-                        self.printer.warning(f'Source path of global configs does not exist: {source_path}')
-            else:
-                self.printer.verbose(f'Skipping global configs')
-
-            self.printer.header('Modules to deploy:')
-            self.printer.normal(f'-> git repository: {manifest["git_repository"]}')
-            self.printer.normal(f'-> version tag: {version_tag}')
-            self.printer.normal('Modules:')
-            for key, value in deploy_actions.items():
-                self.printer.normal(f'--> {key}')
-
-            if not auto_approve:
-                response = input("\nDo you want to continue? (y/N) ")
-                if response.lower() != "y":
-                    sys.exit(1)
-
-            for key, value in deploy_actions.items():
-                self._run_sync(
-                    source_path=value['source'],
-                    target_path=value['target'],
-                    excludes=value.get('excludes', []),
-                    include_lock_file=True,
-                    auto_approve=True,
-                    dry_run=dry_run,
-                    clean=False,
-                    chmod_to_readonly=True,
-                )
+                            self.printer.warning(f'Source path of global configs does not exist: {source_path}')
+                else:
+                    self.printer.verbose(f'Skipping global configs')
 
-            if not dry_run:
-                        # write the version file
-                with open(os.path.join(target_dir, self.VERSION_FILE), 'w') as f:
-                    f.write(f"""
-locals {{
-    version_tag="{version_tag}"
-}}
-""")
+                self.printer.header('Modules to deploy:')
+                self.printer.normal(f'-> git repository: {manifest["git_repository"]}')
+                self.printer.normal(f'-> version tag: {version_tag}')
+                self.printer.normal('Modules:')
+                for key, value in deploy_actions.items():
+                    self.printer.normal(f'--> {key}')
+
+                if not auto_approve:
+                    response = input("\nDo you want to continue? (y/N) ")
+                    if response.lower() != "y":
+                        sys.exit(1)
+
+                for key, value in deploy_actions.items():
+                    self._run_sync(
+                        source_path=value['source'],
+                        target_path=value['target'],
+                        excludes=value.get('excludes', []),
+                        include_lock_file=True,
+                        auto_approve=True,
+                        dry_run=dry_run,
+                        clean=False,
+                        chmod_to_readonly=True,
+                    )
+
+                if not dry_run:
+                            # write the version file
+                    with open(os.path.join(target_dir, self.VERSION_FILE), 'w') as f:
+                        f.write(f"""
+    locals {{
+        version_tag="{version_tag}"
+    }}
+    """)
 
-                # clean up the cache in the deployed directory to avoid strange issues when planning
-                self.clean(working_dir=target_dir)
+                    # clean up the cache in the deployed directory to avoid strange issues when planning
+                    self.clean(working_dir=target_dir)
 
         except KeyError as e:
             self.printer.error(f'Error interpreting the manifest file. Please ensure it uses the proper format. Could not find element: {e}')
             sys.exit(1)
         except Exception as e:
             self.printer.error(f'Unexpected error: {e}')
             if self.printer.print_verbose:
```

### Comparing `tgwrap-0.7.8/tgwrap/printer.py` & `tgwrap-0.7.9/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.7.8/setup.py` & `tgwrap-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'terrasafe>=0.5.1,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['tgwrap = tgwrap.cli:main']}
 
 setup_kwargs = {
     'name': 'tgwrap',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'A (terragrunt) wrapper around a (terraform) wrapper around ....',
     'long_description': '# tg-wrap\n\nThis app simply wraps terragrunt (which is a wrapper around terraform, which is a wrapper around cloud APIs, which is...).\n\nWait, why on earth do we need a wrapper for a wrapper (for a wrapper)?\n\nWell, first of all it is pretty opinionated so what works for us, doesn\'t necessarily work for you.\n\nBut our reasoning for creating this is as follows:\n\n## 1. Less typing\n\nterraform is great, and in combination with terragrunt even greater! But let\'s face it, terragrunt does not excel in conciseness! The options are pretty long, which leads to lots of typing. We don\'t like typing!\n\n## 2. Testing modules locally\n\nHowever, more importantly, we are heavily utilising [TERRAGRUNT_SOURCE](https://terragrunt.gruntwork.io/docs/features/execute-terraform-commands-on-multiple-modules-at-once/#testing-multiple-modules-locally) when developing.\n\nThe thing is that as long as you use `run-all` you can use one setting for that variable (and conveniently set it as an environment variable), while if you run a regular command, you need to specify the full path. Which is obviously different for each project.\n\nWhich leads to (even) more typing, and worse: a higher chance for errors.\n\nLuckily you can use `run-all` and add the appriopriate flags to ensure it behaves like a regular plan|apply|destroy etc. But again, more typing.\n\nNothing a [bunch a aliases](https://gitlab.com/lunadata/terragrunt-utils/-/blob/main/tg-shell.sh) can\'t solve though!\n\n## 3. But the original reason was: Errors when using run-all are challenging\n\nOne of the main boons of terragrunt is the ability to break up large projects in smaller steps while still retaining the inter-dependencies. However, when working on such a large project and something goes wrong somewhere in the middle is pretty challenging.\n\nterragrunt\'s error messages are pretty massive, and this is extrapolated with every individual project in your dependency chain.\n\nAnd if it fails somewhere at the front, it keeps on trying until the last one, blowing up your terminal in the process.\n\nSo we wanted a possibility to run the projects step by step, using the dependency graph of terragrunt and have a bit more control over it.\n\nAnd this was not something a bunch of aliases could solve, hence this wrapper was born. And while we we\'re at it, replacing the aliases with this was then pretty straightforward next step as well.\n\n## 4. Analyzing plan files\n\nWhen using the run-all, analyzing what is about to be changed is not going to be easier. Hence we created the `tgwrap analyze` function that lists all the planned changes and (if a config file is availabe) calculates a drift score and runs a [terrasafe](https://pypi.org/project/terrasafe/) style validation check.\n\nIt needs a config file as follows:\n\n```yaml\n---\n#\n# Critically of resources as interpreted by \'tgwrap analyze\'.\n# It uses it for a \'terrasafe\' like validation if resources can safely be deleted.\n# On top of that it tries to analyze and quantify the drift impact of the changes,\n# so that this can be monitored.\n#\nlow:\n  # defaults:\n  #   terrasafe_level: ignore_deletions\n  #   drift_impact:\n  #     default: minor\n  #     delete: medium\n  azuread_application.: {} # if we you want to use the defaults\n  azuread_app_role_assignment: # or if you want to override these\n    drift_impact:\n      delete: minor\n  # and so on, and so forth\nmedium:\n  # defaults:\n  #   terrasafe_level: ignore_deletion_if_recreation\n  #   drift_impact:\n  #     default: medium\n  #     delete: major\n  azurerm_data_factory_linked_service_key_vault.: {}\n  # and so on, and so forth\nhigh:\n  # defaults:\n  #   terrasafe_level: unauthorized_deletion\n  #   drift_impact:\n  #     default: major\n  #     update: medium\n  azuread_group.:\n    drift_impact:\n      create: minor\n      update: minor\n  azurerm_application_insights.: {}\n  # and so on, and so forth\n```\n\n### Speeding up the performance of analyze\n\nThis `analyze` function turned out to be pretty slow, where most of the time went into the `terragrunt show` function that is executed for each individual module. \n\nThis was a bit surprising as the plan file is already available on the file system, but it turns out that terragrunt is taking quite a bit of time for managing the depdencies. Even when you\'re excluding the external dependencies and are located in a particular module.\n\nSo, if you add the following to your root `terragrunt.hcl`:\n\n```hcl\nterraform {\n  after_hook "link_to_current_module" {\n    commands = ["init", "plan", "apply", "validate", "destroy"]\n    execute  = ["bash", "-c", "ln -sf $(pwd) ${get_terragrunt_dir()}/.terragrunt-cache/current"]\n  }\n}\n```\n\nThe directory where the plan file is stored (including the other resources that terraform needs) becomes predictable and it becomes possible to run a native `terraform show` (instead `terragrunt show`) which dramatically speed up things.\n\nJust set the proper value as an environment variable:\n\n```console\nexport TGWRAP_PLANFILE_DIR=".terragrunt-cache/current"\n```\n\nOr pass it along with the `--planfile-dir|-P` option and it will use that.\n\n## Usage\n\n```console\n# general help\ntgwrap --help\n\ntgwrap run -h\ntgwrap run-all -h\n\n# run a plan\ntgwrap plan # which is the same as tgwrap run plan\n\n# run-all a plan\ntgwrap run-all plan\n\n# or do the same in step-by-step mode\ntgwrap run-all plan -s\n\n# or excluding (aka ignoring) external dependencies\ntgwrap run-all plan -sx\n\n# if you want to add additional arguments it is recommended to use -- as separator (although it *might* work without)\ntgwrap output -- -json\n```\n\n> Note: special precautions are needed when passing on parameters that contain quotes. For instance, if you want to move state like below, escape the double quote in the staate address:\n\n`tgwrap state mv \'azuread_group.this[\\"viewers\\"]\' \'azuread_group.this[\\"readers\\"]\'`\n\n## A word about escaping inputs\n\nYour shell is escaping special characters such as `*` and `"` before passing it to the program (`tgwrap` in this case). So some inputs **need** to be escaped in order to function properly.\n\nFor example:\n\n```console\n# to exclude certain modules from an action (such as analyze):\ntgwrap analyze -E \'integrations/\\*/\\*\'\n\n# to import a resource that has a " in its address:\ntgwrap import -a \'azuread_group.this[\\"my_group\\"]\' -i ${GROUP_ID}\n```\n\n## Deploy manifests\n\nIn order to easily deploy a new version of the terraform (and associated terragrunt) modules, we include a manifest file in the root of the landing zone:\n\n```yaml\n---\ngit_repository: ssh://git@gitlab.com/my-org/my-terraform-modules-repo.git\nbase_path: terragrunt/my-platform\n\ndeploy: # which modules do you want to deploy\n  dtap:\n    applies_to_stages:\n      - dev\n      - tst\n      - acc\n      - prd\n    source_stage: dev\n    base_dir: platform # optional, if you want to deploy the base modules in its own dir, side by side with substacks\n    exclude_modules: # these modules will always be excluded, can be omitted\n      - my-specific-module\n    include_modules: {} # omit or use an empty dict for all of them\n      # or specify your modules as follows\n      # base: {} # just a simple include\n      # networking-connected: # or a bit more complicated\n      #  - source: networking\n      #  - target: networking-connected\n\nsub_stacks:\n  is01:\n    source: shared-integration/intsvc01\n    target: integration/is01\n    exclude_modules:  # a list of modules that will always be excluded, can be omitted\n      - my-specific-module\n  is02:\n    source: shared-integration/intsvc01\n    target: integration/is02\n\n# global configuration files that are deployed as well\n# note that these files are typically applicable to all landing zones and stages!\n# this might lead to unexpected behaviour\n# note that you can exclude syncing these files with a command line switch\nglobal_config_files:\n  root-terragrunt:\n    source: ../../terragrunt.hcl # relative to base_path\n    target: ../../terragrunt.hcl # can be omitted, then it is same as source path\n  terrasafe-config:\n    source: ../../terrasafe-config.json\n```\n\n## Development\n\nIn order to develop, you need to apply it to your terragrunt projects. For that you can use the `--terragrunt-working-dir` option and just run it from the poetry directory. Alternatively you can use the [tgwrap-dev](./tgwrap-dev) script and invoke that from your terragrunt directories. Either put it in your `PATH` or create an alias for convenience.\n',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/lunadata/tgwrap',
```

### Comparing `tgwrap-0.7.8/PKG-INFO` & `tgwrap-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.7.8
+Version: 0.7.9
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
```

