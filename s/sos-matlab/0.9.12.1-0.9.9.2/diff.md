# Comparing `tmp/sos-matlab-0.9.12.1.tar.gz` & `tmp/sos-matlab-0.9.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sos-matlab-0.9.12.1.tar", last modified: Tue May  8 19:35:18 2018, max compression
+gzip compressed data, was "dist/sos-matlab-0.9.9.2.tar", last modified: Thu Oct  5 21:14:07 2017, max compression
```

## Comparing `sos-matlab-0.9.12.1.tar` & `sos-matlab-0.9.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      217 2017-10-06 19:45:41.000000 sos-matlab-0.9.12.1/MANIFEST.in
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      888 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      710 2017-10-06 19:45:41.000000 sos-matlab-0.9.12.1/README.md
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/setup.cfg
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2417 2018-03-05 23:33:01.000000 sos-matlab-0.9.12.1/setup.py
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-06 19:45:41.000000 sos-matlab-0.9.12.1/src/sos_matlab/__init__.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1717 2018-05-08 19:35:14.000000 sos-matlab-0.9.12.1/src/sos_matlab/_version.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7180 2018-05-08 19:34:35.000000 sos-matlab-0.9.12.1/src/sos_matlab/kernel.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      973 2018-02-12 15:46:15.000000 sos-matlab-0.9.12.1/src/sos_matlab/sos_load_obj.m
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     4897 2018-02-12 15:46:15.000000 sos-matlab-0.9.12.1/src/sos_matlab/sos_py_repr.m
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/dependency_links.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       93 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/entry_points.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      888 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/PKG-INFO
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       37 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/requires.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      452 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/SOURCES.txt
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       11 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/src/sos_matlab.egg-info/top_level.txt
-drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2018-05-08 19:35:18.000000 sos-matlab-0.9.12.1/test/
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6161 2018-02-12 15:46:15.000000 sos-matlab-0.9.12.1/test/test_Matlab_kernel.py
--rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5927 2017-10-06 19:45:41.000000 sos-matlab-0.9.12.1/test/test_Octave_kernel.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      217 2017-10-05 21:13:03.000000 sos-matlab-0.9.9.2/MANIFEST.in
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      862 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-05 21:06:04.000000 sos-matlab-0.9.9.2/README.md
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       38 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/setup.cfg
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     2474 2017-10-05 21:08:47.000000 sos-matlab-0.9.9.2/setup.py
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:09:06.000000 sos-matlab-0.9.9.2/src/sos_matlab/__init__.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1716 2017-10-05 21:09:12.000000 sos-matlab-0.9.9.2/src/sos_matlab/_version.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     1571 2017-10-05 21:06:04.000000 sos-matlab-0.9.9.2/src/sos_matlab/actions.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     7115 2017-10-05 21:06:04.000000 sos-matlab-0.9.9.2/src/sos_matlab/kernel.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     3759 2017-10-05 21:06:04.000000 sos-matlab-0.9.9.2/src/sos_matlab/sos_py_repr.m
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        1 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/dependency_links.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      143 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/entry_points.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      862 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/PKG-INFO
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       31 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/requires.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)      448 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/SOURCES.txt
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)       11 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/src/sos_matlab.egg-info/top_level.txt
+drwxr-xr-x   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)        0 2017-10-05 21:14:07.000000 sos-matlab-0.9.9.2/test/
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     6042 2017-10-05 21:09:53.000000 sos-matlab-0.9.9.2/test/test_Matlab_kernel.py
+-rw-r--r--   0 bpeng1   (1985961928) MDANDERSON\Domain Users (895809667)     5927 2017-10-05 21:10:07.000000 sos-matlab-0.9.9.2/test/test_Octave_kernel.py
```

### Comparing `sos-matlab-0.9.12.1/PKG-INFO` & `sos-matlab-0.9.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: sos-matlab
-Version: 0.9.12.1
+Version: 0.9.9.2
 Summary: SoS Notebook extension for Matlab and Octave
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
-Maintainer: Bo Peng
-Maintainer-email: bpeng@mdanderson.org
 License: GPL3
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sos-matlab-0.9.12.1/setup.py` & `sos-matlab-0.9.9.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,17 +51,21 @@
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: Implementation :: CPython',
         ],
     packages = find_packages('src'),
     package_dir = {'': 'src'},
     install_requires=[
-          'sos>=0.9.12.0',
-          'sos-notebook>=0.9.12.6',
+          'sos',
+          'sos-notebook',
+          'matlab_kernel',
       ],
     entry_points= '''
+[sos_actions]
+matlab = sos_matlab.actions:matlab
+
 [sos_languages]
-MATLAB = sos_matlab.kernel:sos_MATLAB
-Octave = sos_matlab.kernel:sos_MATLAB
+Matlab = sos_matlab.kernel:sos_Matlab
+Octave = sos_matlab.kernel:sos_Matlab
 '''
 )
```

### Comparing `sos-matlab-0.9.12.1/src/sos_matlab/_version.py` & `sos-matlab-0.9.9.2/src/sos_matlab/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     raise SystemError('SOS requires Python 3.4 or higher. Please upgrade your Python {}.{}.{}.'
         .format(_py_ver.major, _py_ver.minor, _py_ver.micro))
 
 
 # version of the SoS language
 __sos_version__ = '1.0'
 # version of the sos command
-__version__ = '0.9.12.1'
+__version__ = '0.9.9.2'
 __py_version__ = '{}.{}.{}'.format(_py_ver.major, _py_ver.minor, _py_ver.micro)
 
 #
 SOS_FULL_VERSION='{} for Python {}.{}.{}'.format(__version__, _py_ver.major, _py_ver.minor, _py_ver.micro)
 SOS_COPYRIGHT = '''SoS {} : Copyright (c) 2016 Bo Peng'''.format(__version__)
 SOS_CONTACT = '''Please visit http://github.com/vatlab/SOS for more information.'''
```

### Comparing `sos-matlab-0.9.12.1/src/sos_matlab/kernel.py` & `sos-matlab-0.9.9.2/src/sos_matlab/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,18 @@
     else:
         return True if all(isinstance(x, first_type) for x in iseq) else False
 
 Matlab_init_statements = r'''
 path(path, {!r})
 '''.format(os.path.split(__file__)[0])
 
-class sos_MATLAB:
-    supported_kernels = {'MATLAB': ['imatlab', 'matlab'], 'Octave': ['octave']}
-    background_color = {'MATLAB': '#8ee7f1', 'Octave': '#dff8fb'}
+class sos_Matlab:
+    supported_kernels = {'Matlab': ['matlab', 'imatlab'], 'Octave': ['octave']}
+    background_color = '#dff8fb'
     options = {}
-    cd_command = 'cd {dir}'
 
     def __init__(self, sos_kernel, kernel_name='matlab'):
         self.sos_kernel = sos_kernel
         self.kernel_name = kernel_name
         self.init_statements = Matlab_init_statements
         if self.kernel_name == 'octave':
             self.init_statements += 'pkg load dataframe\n'
@@ -103,16 +102,16 @@
             sio.savemat('mat2mtlb.mat', {'obj': obj})
             return 'cell2mat(struct2cell(load(fullfile(' + '\'' + dic + '\'' + ',' \
                 + '\'mat2mtlb.mat\'))))'
         elif isinstance(obj, np.ndarray):
             dic = tempfile.tempdir
             os.chdir(dic)
             sio.savemat('ary2mtlb.mat', {'obj': obj})
-            return 'sos_load_obj(fullfile(' + '\'' + dic + '\'' + ',' \
-                + '\'ary2mtlb.mat\'))'
+            return 'load(fullfile(' + '\'' + dic + '\'' + ',' \
+                + '\'ary2mtlb.mat\')).obj'
         elif isinstance(obj, dict):
             dic = tempfile.tempdir
             os.chdir(dic)
             sio.savemat('dict2mtlb.mat', {'obj': obj})
             return 'load(fullfile(' + '\'' + dic + '\'' + ',' \
                 + '\'dict2mtlb.mat\'))'
         elif isinstance(obj, pd.DataFrame):
```

### Comparing `sos-matlab-0.9.12.1/src/sos_matlab.egg-info/PKG-INFO` & `sos-matlab-0.9.9.2/src/sos_matlab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: sos-matlab
-Version: 0.9.12.1
+Version: 0.9.9.2
 Summary: SoS Notebook extension for Matlab and Octave
 Home-page: https://github.com/vatlab/SOS
 Author: Bo Peng
 Author-email: bpeng@mdanderson.org
-Maintainer: Bo Peng
-Maintainer-email: bpeng@mdanderson.org
 License: GPL3
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `sos-matlab-0.9.12.1/test/test_Matlab_kernel.py` & `sos-matlab-0.9.9.2/test/test_Matlab_kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,23 +51,23 @@
 import numpy as np
 import scipy.io as sio
 arr = np.random.randn(1000)
 arr[::10] = np.nan
 df = pd.DataFrame({'column_{0}'.format(i): arr for i in range(10)})
 ''')
             clear_channels(iopub)
-            execute(kc=kc, code="%use MATLAB")
+            execute(kc=kc, code="%use Matlab")
             wait_for_idle(kc)
             #_, stderr = assemble_output(iopub)
             #self.assertEqual(stderr, '')
             execute(kc=kc, code="%get df")
             wait_for_idle(kc)
             execute(kc=kc, code="display(size(df))")
             stdout, _ = assemble_output(iopub)
-            self.assertEqual(stdout.strip().split(), ['1000', '10'])
+            self.assertEqual(stdout.strip().split(), ['900', '10'])
             execute(kc=kc, code="%use sos")
             wait_for_idle(kc)
 
     @unittest.skipIf(not shutil.which('matlab'), 'Matlab not installed')
     def testGetPythonDataFromMatlab(self):
         with sos_kernel() as kc:
             iopub = kc.iopub_channel
@@ -75,54 +75,52 @@
 null_var = None
 num_var = 123
 import numpy
 import scipy.io as sio
 num_arr_var = numpy.array([1, 2, 3])
 logic_var = True
 logic_arr_var = [True, False, True]
-float_var = [1.2, 2.1]
 char_var = '1"23'
 char_arr_var = ['1', '2', '3']
 list_var = [1, 2, '3']
 dict_var = dict(a=1, b=2, c='3')
 set_var = {1, 2, '3'}
 mat_var = numpy.matrix([[1,2],[3,4]])
 recursive_var = {'a': {'b': 123}, 'c': True}
 ''')
             wait_for_idle(kc)
             execute(kc=kc, code='''
-%use MATLAB
-%get null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var float_var
+%use Matlab
+%get null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var
 %dict -r
-%put null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var float_var
+%put null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var
 %use sos
-%dict null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var float_var
+%dict null_var num_var num_arr_var logic_var logic_arr_var char_var char_arr_var mat_var set_var list_var dict_var recursive_var
                 ''')
             res = get_result(iopub)
             self.assertEqual(res['null_var'], None)
             self.assertEqual(res['num_var'], 123)
             self.assertEqual(list(res['num_arr_var']), [1,2,3], "Got {}".format(res['num_arr_var']))
             self.assertEqual(res['logic_var'], True)
             self.assertEqual(res['logic_arr_var'], [True, False, True])
             self.assertEqual(res['char_var'], '1"23')
-            self.assertEqual(list(res['float_var']), [1.2, 2.1])
             self.assertEqual(list(res['list_var']), [1,2,'3'], 'Got {}'.format(res['list_var']))
             self.assertEqual(res['dict_var'], {'a': 1, 'b': 2, 'c': '3'})
             self.assertTrue(len(res['set_var']) ==3 and '3' in res['set_var'] and 1 in res['set_var'] and 2 in res['set_var'])
 
             self.assertEqual(res['mat_var'].shape, (2,2))
             self.assertEqual(res['recursive_var'],  {'a': {'b': 123}, 'c': True})
             #self.assertEqual(res['char_arr_var'], ['1', '2', '3'])
 
     @unittest.skipIf(not shutil.which('matlab'), 'Matlab not installed')
     def testPutMatlabDataToPython(self):
         with sos_kernel() as kc:
             iopub = kc.iopub_channel
             execute(kc=kc, code="""
-%use MATLAB
+%use Matlab
 null_var = NaN
 num_var = 123
 num_arr_var = [1, 2, 3]
 logic_var = true
 logic_arr_var = [true, false, true]
 char_var = '1"23'
 char_arr_var = ['1'; '2'; '3']
```

### Comparing `sos-matlab-0.9.12.1/test/test_Octave_kernel.py` & `sos-matlab-0.9.9.2/test/test_Octave_kernel.py`

 * *Files identical despite different names*

