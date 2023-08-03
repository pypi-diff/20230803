# Comparing `tmp/discco-0.2.4.tar.gz` & `tmp/discco-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discco-0.2.4.tar", last modified: Wed Apr 26 14:34:11 2023, max compression
+gzip compressed data, was "/home/runner/work/discco/discco/dist/.tmp-hswyall6/discco-0.2.5.tar", last modified: Thu Aug  3 11:02:57 2023, max compression
```

## Comparing `discco-0.2.4.tar` & `discco-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.505150 discco-0.2.4/
--rw-r--r--   0 blandt   (743162876) 1934034978    18650 2021-09-23 09:56:26.000000 discco-0.2.4/LICENSE
--rw-r--r--   0 blandt   (743162876) 1934034978     3776 2023-04-26 14:34:11.505403 discco-0.2.4/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978     2927 2023-01-31 12:49:19.000000 discco-0.2.4/README.md
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.489488 discco-0.2.4/discco/
--rw-r--r--   0 blandt   (743162876) 1934034978       22 2023-01-24 10:52:48.000000 discco-0.2.4/discco/__init__.py
--rw-r--r--   0 blandt   (743162876) 1934034978    21470 2023-01-27 22:05:05.000000 discco-0.2.4/discco/discco.py
-drwxr-xr-x   0 blandt   (743162876) 1934034978        0 2023-04-26 14:34:11.504119 discco-0.2.4/discco.egg-info/
--rw-r--r--   0 blandt   (743162876) 1934034978     3776 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/PKG-INFO
--rw-r--r--   0 blandt   (743162876) 1934034978      221 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/SOURCES.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        1 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/dependency_links.txt
--rw-r--r--   0 blandt   (743162876) 1934034978       69 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/requires.txt
--rw-r--r--   0 blandt   (743162876) 1934034978        7 2023-04-26 14:34:11.000000 discco-0.2.4/discco.egg-info/top_level.txt
--rw-r--r--   0 blandt   (743162876) 1934034978      103 2023-04-26 14:34:11.508332 discco-0.2.4/setup.cfg
--rw-r--r--   0 blandt   (743162876) 1934034978      924 2023-04-26 14:34:03.000000 discco-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:02:57.000000 discco-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:02:38.000000 discco-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-03 11:02:57.000000 discco-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-08-03 11:02:38.000000 discco-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:02:57.000000 discco-0.2.5/discco/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 11:02:38.000000 discco-0.2.5/discco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-08-03 11:02:38.000000 discco-0.2.5/discco/discco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 11:02:57.000000 discco-0.2.5/discco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:02:57.000000 discco-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-03 11:02:38.000000 discco-0.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `discco-0.2.4/LICENSE` & `discco-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discco-0.2.4/PKG-INFO` & `discco-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,59 @@
-Metadata-Version: 2.1
-Name: discco
-Version: 0.2.4
-Summary: Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images
-Home-page: UNKNOWN
-Author: Tom Bland
-Author-email: tom_bland@hotmail.co.uk
-License: CC BY 4.0
-Project-URL: Source Code, https://github.com/tsmbland/discco
-Description: # DISCCo: Differentiable Image Simulation of the Cell Cortex
-        
-        [![CC BY 4.0][cc-by-shield]][cc-by]
-        [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
-        
-        Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
-        Designed for use on images of PAR proteins in C. elegans zygotes.
-        
-        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
-        
-        ## Methods
-        
-        Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
-        Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
-        Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
-        Full straightened images can then be simulated as the addition of two tensor products:
-        
-        sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
-        
-        where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
-        Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
-        
-        <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/schematic.png" width="100%" height="100%"/>
-        </p>
-        
-        In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
-        
-        <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
-        </p>
-        
-        For full details of the model and training procedures, see
-        
-        PAPER IN PREP
-        
-        And the accompanying GitHub repository:
-        
-        IN PREP
-        
-        ## Installation
-        
-            pip install discco
-        
-        ## License
-        
-        This work is licensed under a
-        [Creative Commons Attribution 4.0 International License][cc-by].
-        
-        [![CC BY 4.0][cc-by-image]][cc-by]
-        
-        [cc-by]: http://creativecommons.org/licenses/by/4.0/
-        [cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
-        [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
-        
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# DISCCo: Differentiable Image Simulation of the Cell Cortex
+
+[![CC BY 4.0][cc-by-shield]][cc-by]
+[![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
+
+Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
+Designed for use on images of PAR proteins in C. elegans zygotes.
+
+This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
+
+## Methods
+
+Our method is adapted from previous methods that model intensity profiles perpendicular to the membrane as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). Typically these two components are modelled as an error-function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. Using this model, one can generate simulated images of straightened cortices as the sum of two tensor products which represent distinct membrane and cytoplasmic signal contributions (Figure 1):
+
+sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
+
+where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles and s<sub>cyt</sub> and s<sub>mem</sub> are, by default, error-function and Gaussian profiles. We impose the constraint that the cytoplasmic concentration c<sub>cyt</sub> is uniform throughout each image.
+<p align="center">
+    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/schematic.png" width="100%" height="100%"/>
+    <i>Figure 1: Schematic of differentiable model for image quantification</i>
+</p>
+<br>
+
+Using a differentiable programming paradigm, the input parameters to the model can be iteratively adjusted by backpropagation to minimize the mean squared error between simulated images and ground truth images.
+As well as allowing the image-specific concentration parameters (c<sub>cyt</sub> and c<sub>mem</sub>) to be learnt, this procedure also allows the global signal profiles s<sub>cyt</sub> and s<sub>mem</sub> to be optimised and take any arbitrary form, allowing the model to generalise beyond a simple Gaussian PSF model and account for complex sample-specific light-scattering behaviors. In practice we find that this additional flexibility is necessary to minimise model bias and prevent underfitting:
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="80%" height="80%"/>
+    <br>
+    <i>Figure 2: Example of ground truth and simulated images. Naive model refers to a mechanistic optical model with a Guassian PSF. Gaussian noise has been added to simulated images to allow for closer visual comparison to the ground truth image.</i>
+   
+</p>  
+<br>
+
+An additional step, described in the paper, puts the cytoplasmic and membrane concentrations outputted by the model into biologically meaningful units, which has great utility for mathematical models.
+
+For full details of the model and training procedures, see
+
+PAPER IN PREP
+
+And the accompanying GitHub repository:
+
+IN PREP
+
+## Installation
+
+    pip install discco
+
+## License
+
+This work is licensed under a
+[Creative Commons Attribution 4.0 International License][cc-by].
+
+[![CC BY 4.0][cc-by-image]][cc-by]
+
+[cc-by]: http://creativecommons.org/licenses/by/4.0/
+[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
+[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+
```

### Comparing `discco-0.2.4/README.md` & `discco-0.2.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,53 @@
+Metadata-Version: 2.1
+Name: discco
+Version: 0.2.5
+Summary: Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images
+Author: Tom Bland
+Author-email: tom_bland@hotmail.co.uk
+License: CC BY 4.0
+Project-URL: Source Code, https://github.com/tsmbland/discco
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DISCCo: Differentiable Image Simulation of the Cell Cortex
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
 
 Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
 Designed for use on images of PAR proteins in C. elegans zygotes.
 
 This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
 
 ## Methods
 
-Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
-Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
-Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
-Full straightened images can then be simulated as the addition of two tensor products:
+Our method is adapted from previous methods that model intensity profiles perpendicular to the membrane as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). Typically these two components are modelled as an error-function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. Using this model, one can generate simulated images of straightened cortices as the sum of two tensor products which represent distinct membrane and cytoplasmic signal contributions (Figure 1):
 
 sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
 
-where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
-Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
-
+where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles and s<sub>cyt</sub> and s<sub>mem</sub> are, by default, error-function and Gaussian profiles. We impose the constraint that the cytoplasmic concentration c<sub>cyt</sub> is uniform throughout each image.
 <p align="center">
     <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/schematic.png" width="100%" height="100%"/>
+    <i>Figure 1: Schematic of differentiable model for image quantification</i>
 </p>
+<br>
 
-In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
+Using a differentiable programming paradigm, the input parameters to the model can be iteratively adjusted by backpropagation to minimize the mean squared error between simulated images and ground truth images.
+As well as allowing the image-specific concentration parameters (c<sub>cyt</sub> and c<sub>mem</sub>) to be learnt, this procedure also allows the global signal profiles s<sub>cyt</sub> and s<sub>mem</sub> to be optimised and take any arbitrary form, allowing the model to generalise beyond a simple Gaussian PSF model and account for complex sample-specific light-scattering behaviors. In practice we find that this additional flexibility is necessary to minimise model bias and prevent underfitting:
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
-</p>
+    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="80%" height="80%"/>
+    <br>
+    <i>Figure 2: Example of ground truth and simulated images. Naive model refers to a mechanistic optical model with a Guassian PSF. Gaussian noise has been added to simulated images to allow for closer visual comparison to the ground truth image.</i>
+   
+</p>  
+<br>
+
+An additional step, described in the paper, puts the cytoplasmic and membrane concentrations outputted by the model into biologically meaningful units, which has great utility for mathematical models.
 
 For full details of the model and training procedures, see
 
 PAPER IN PREP
 
 And the accompanying GitHub repository:
```

### Comparing `discco-0.2.4/discco/discco.py` & `discco-0.2.5/discco/discco.py`

 * *Files identical despite different names*

### Comparing `discco-0.2.4/discco.egg-info/PKG-INFO` & `discco-0.2.5/discco.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 Metadata-Version: 2.1
 Name: discco
-Version: 0.2.4
+Version: 0.2.5
 Summary: Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images
-Home-page: UNKNOWN
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
 Project-URL: Source Code, https://github.com/tsmbland/discco
-Description: # DISCCo: Differentiable Image Simulation of the Cell Cortex
-        
-        [![CC BY 4.0][cc-by-shield]][cc-by]
-        [![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
-        
-        Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
-        Designed for use on images of PAR proteins in C. elegans zygotes.
-        
-        This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
-        
-        ## Methods
-        
-        Our method is adapted from previous methods that model cross-cortex intensity profiles at each position around the cortex as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). 
-        Typically, these two components are modelled as an error function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. 
-        In our model we relax these assumptions to account for the possibility of a non-Gaussian PSF and complex light-scattering behaviours which cannot be captured with these simplistic descriptions. 
-        Instead, cytoplasmic and membrane signal profiles are modelled as arbitrary vectors of length 50 pixels which can take on any shape (s<sub>mem</sub> and s<sub>cyt</sub>). 
-        Full straightened images can then be simulated as the addition of two tensor products:
-        
-        sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
-        
-        where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles.
-        Building the model using the differentiable programming language JAX allows input parameters to be iteratively adjusted by backpropagation to minimise the mean squared error between simulated images and ground truth images: 
-        
-        <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/schematic.png" width="100%" height="100%"/>
-        </p>
-        
-        In doing so, both the image-specific concentration parameters and the underlying quantification model (i.e. s<sub>mem</sub> and s<sub>cyt</sub>) can be optimised, allowing for closer simulations and more accurate quantification:
-        
-        <p align="center">
-            <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="100%" height="100%"/>
-        </p>
-        
-        For full details of the model and training procedures, see
-        
-        PAPER IN PREP
-        
-        And the accompanying GitHub repository:
-        
-        IN PREP
-        
-        ## Installation
-        
-            pip install discco
-        
-        ## License
-        
-        This work is licensed under a
-        [Creative Commons Attribution 4.0 International License][cc-by].
-        
-        [![CC BY 4.0][cc-by-image]][cc-by]
-        
-        [cc-by]: http://creativecommons.org/licenses/by/4.0/
-        [cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
-        [cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DISCCo: Differentiable Image Simulation of the Cell Cortex
+
+[![CC BY 4.0][cc-by-shield]][cc-by]
+[![PyPi version](https://badgen.net/pypi/v/discco/)](https://pypi.org/project/discco)
+
+Quantification of membrane and cytoplasmic concentrations based on differentiable simulation of cell cortex images.
+Designed for use on images of PAR proteins in C. elegans zygotes.
+
+This extends on the segmentation and straightening algorithm described [here](https://github.com/tsmbland/par-segmentation), and uses straightened cortices obtained by that method as input.
+
+## Methods
+
+Our method is adapted from previous methods that model intensity profiles perpendicular to the membrane as the sum of distinct cytoplasmic and membrane signal components (Gross et al., 2018; Reich et al., 2019). Typically these two components are modelled as an error-function and Gaussian function respectively, representing the expected shape of a step and a point convolved by a Gaussian point spread function (PSF) in one dimension. Using this model, one can generate simulated images of straightened cortices as the sum of two tensor products which represent distinct membrane and cytoplasmic signal contributions (Figure 1):
+
+sim = c<sub>cyt</sub> ⊗ s<sub>cyt</sub> + c<sub>mem</sub> ⊗ s<sub>mem</sub>
+
+where c<sub>cyt</sub> and c<sub>mem</sub> are cytoplasmic and membrane concentration profiles and s<sub>cyt</sub> and s<sub>mem</sub> are, by default, error-function and Gaussian profiles. We impose the constraint that the cytoplasmic concentration c<sub>cyt</sub> is uniform throughout each image.
+<p align="center">
+    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/schematic.png" width="100%" height="100%"/>
+    <i>Figure 1: Schematic of differentiable model for image quantification</i>
+</p>
+<br>
+
+Using a differentiable programming paradigm, the input parameters to the model can be iteratively adjusted by backpropagation to minimize the mean squared error between simulated images and ground truth images.
+As well as allowing the image-specific concentration parameters (c<sub>cyt</sub> and c<sub>mem</sub>) to be learnt, this procedure also allows the global signal profiles s<sub>cyt</sub> and s<sub>mem</sub> to be optimised and take any arbitrary form, allowing the model to generalise beyond a simple Gaussian PSF model and account for complex sample-specific light-scattering behaviors. In practice we find that this additional flexibility is necessary to minimise model bias and prevent underfitting:
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/tsmbland/discco/master/docs/simulation comparison.png" width="80%" height="80%"/>
+    <br>
+    <i>Figure 2: Example of ground truth and simulated images. Naive model refers to a mechanistic optical model with a Guassian PSF. Gaussian noise has been added to simulated images to allow for closer visual comparison to the ground truth image.</i>
+   
+</p>  
+<br>
+
+An additional step, described in the paper, puts the cytoplasmic and membrane concentrations outputted by the model into biologically meaningful units, which has great utility for mathematical models.
+
+For full details of the model and training procedures, see
+
+PAPER IN PREP
+
+And the accompanying GitHub repository:
+
+IN PREP
+
+## Installation
+
+    pip install discco
+
+## License
+
+This work is licensed under a
+[Creative Commons Attribution 4.0 International License][cc-by].
+
+[![CC BY 4.0][cc-by-image]][cc-by]
+
+[cc-by]: http://creativecommons.org/licenses/by/4.0/
+[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
+[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+
```

### Comparing `discco-0.2.4/setup.py` & `discco-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='discco',
-    version='0.2.4',
+    version='0.2.5',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     install_requires=['numpy',
                       'matplotlib',
                       'pandas',
```

