# Comparing `tmp/electricalsim_opf_quadratic-1.1.tar.gz` & `tmp/electricalsim_opf_quadratic-1.2.tar.gz`

## Comparing `electricalsim_opf_quadratic-1.1.tar` & `electricalsim_opf_quadratic-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/README.md
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/EGS_extension_manager.png
--rw-r--r--   0        0        0   129135 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/opf_with_EGS.png
--rw-r--r--   0        0        0   197876 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/results.png
--rw-r--r--   0        0        0    64393 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab1.png
--rw-r--r--   0        0        0    55999 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab2.png
--rw-r--r--   0        0        0    65976 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab3.png
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/__init__.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/extension.py
--rw-r--r--   0        0        0    43291 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/input.ui
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/electricalsim_opf_quadratic.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/misc.xml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/modules.xml
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/workspace.xml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/LICENSE
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/README_PyPI.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/pyproject.toml
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/README.md
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/EGS_extension_manager.png
+-rw-r--r--   0        0        0   129135 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/opf_with_EGS.png
+-rw-r--r--   0        0        0   197876 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/results.png
+-rw-r--r--   0        0        0    64393 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/tab1.png
+-rw-r--r--   0        0        0    55999 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/tab2.png
+-rw-r--r--   0        0        0    65976 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/img/tab3.png
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/__init__.py
+-rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/extension.py
+-rw-r--r--   0        0        0    43291 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/input.ui
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/electricalsim_opf_quadratic.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/misc.xml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/modules.xml
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/workspace.xml
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/LICENSE
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/README_PyPI.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/pyproject.toml
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.2/PKG-INFO
```

### Comparing `electricalsim_opf_quadratic-1.1/README.md` & `electricalsim_opf_quadratic-1.2/README.md`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/EGS_extension_manager.png` & `electricalsim_opf_quadratic-1.2/img/EGS_extension_manager.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/opf_with_EGS.png` & `electricalsim_opf_quadratic-1.2/img/opf_with_EGS.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/results.png` & `electricalsim_opf_quadratic-1.2/img/results.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/tab1.png` & `electricalsim_opf_quadratic-1.2/img/tab1.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/tab2.png` & `electricalsim_opf_quadratic-1.2/img/tab2.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/img/tab3.png` & `electricalsim_opf_quadratic-1.2/img/tab3.png`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/extension.py` & `electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,45 +42,52 @@
         'cp2_eur_per_mw2', 'cq2_eur_per_mvar2'
         """
         data = pd.DataFrame(columns=['name', 'element_type', 'element_id',
                                      'bus', 'cp1_eur_per_mw', 'cp0_eur',
                                      'cq1_eur_per_mvar', 'cq0_eur',
                                      'cp2_eur_per_mw2', 'cq2_eur_per_mvar2'])  # Empty DataFrame
 
-        for _, row in self.net.poly_cost.iterrows():
-            new_data_row = pd.Series(index=['name', 'element_type', 'element_id',
-                                            'bus', 'cp1_eur_per_mw', 'cp0_eur',
-                                            'cq1_eur_per_mvar', 'cq0_eur',
-                                            'cp2_eur_per_mw2', 'cq2_eur_per_mvar2'])
-
-            type_ = row['et']
-            element_id = row['element']
-            new_data_row['element_id'] = element_id
-            new_data_row['element_type'] = type_
-            new_data_row['cp0_eur'] = row['cp0_eur']
-            new_data_row['cp1_eur_per_mw'] = row['cp1_eur_per_mw']
-            new_data_row['cp2_eur_per_mw2'] = row['cp2_eur_per_mw2']
-            new_data_row['cq0_eur'] = row['cq0_eur']
-            new_data_row['cq1_eur_per_mvar'] = row['cq1_eur_per_mvar']
-            new_data_row['cq2_eur_per_mvar2'] = row['cq2_eur_per_mvar2']
-            new_data_row['name'] = self.net[type_].at[element_id, 'name']
-            if type_=='dcline':
-                bus_id_from = self.net.dcline.at[element_id, 'bus_from']
-                bus_id_to = self.net.dcline.at[element_id, 'bus_to']
-
-                bus_name_from = self.net.bus.at[bus_id_from, 'name']
-                bus_name_to = self.net.bus.at[bus_id_to, 'name']
-
-                new_data_row['bus'] = f"{bus_id_from} - {bus_id_to} ({bus_name_from} - {bus_name_to})"
-            else:
-                bus_id = self.net[type_].at[element_id, 'bus']
-                bus_name = self.net.bus.at[bus_id, 'name']
-                new_data_row['bus'] = f"{bus_id} ({bus_name})"
-
-            data = pd.concat((data, new_data_row.to_frame().T), axis=0, ignore_index=True)
+        try:
+            for _, row in self.net.poly_cost.iterrows():
+                new_data_row = pd.Series(index=['name', 'element_type', 'element_id',
+                                                'bus', 'cp1_eur_per_mw', 'cp0_eur',
+                                                'cq1_eur_per_mvar', 'cq0_eur',
+                                                'cp2_eur_per_mw2', 'cq2_eur_per_mvar2'])
+
+                type_ = row['et']
+                element_id = row['element']
+                new_data_row['element_id'] = element_id
+                new_data_row['element_type'] = type_
+                new_data_row['cp0_eur'] = row['cp0_eur']
+                new_data_row['cp1_eur_per_mw'] = row['cp1_eur_per_mw']
+                new_data_row['cp2_eur_per_mw2'] = row['cp2_eur_per_mw2']
+                new_data_row['cq0_eur'] = row['cq0_eur']
+                new_data_row['cq1_eur_per_mvar'] = row['cq1_eur_per_mvar']
+                new_data_row['cq2_eur_per_mvar2'] = row['cq2_eur_per_mvar2']
+                new_data_row['name'] = self.net[type_].at[element_id, 'name']
+                if type_=='dcline':
+                    bus_id_from = self.net.dcline.at[element_id, 'bus_from']
+                    bus_id_to = self.net.dcline.at[element_id, 'bus_to']
+
+                    bus_name_from = self.net.bus.at[bus_id_from, 'name']
+                    bus_name_to = self.net.bus.at[bus_id_to, 'name']
+
+                    new_data_row['bus'] = f"{bus_id_from} - {bus_id_to} ({bus_name_from} - {bus_name_to})"
+                else:
+                    bus_id = self.net[type_].at[element_id, 'bus']
+                    bus_name = self.net.bus.at[bus_id, 'name']
+                    new_data_row['bus'] = f"{bus_id} ({bus_name})"
+
+                data = pd.concat((data, new_data_row.to_frame().T), axis=0, ignore_index=True)
+
+        except KeyError:
+            data = pd.DataFrame(columns=['name', 'element_type', 'element_id',
+                                         'bus', 'cp1_eur_per_mw', 'cp0_eur',
+                                         'cq1_eur_per_mvar', 'cq0_eur',
+                                         'cp2_eur_per_mw2', 'cq2_eur_per_mvar2'])  # Empty DataFrame
 
         return data
 
     def __call__(self):
         if self.compute_opf is False:
             return
 
@@ -108,38 +115,45 @@
         trafo3w_losses = self.input_dialog.trafo3w_losses.currentText()
         consider_line_temperature = self.input_dialog.consider_line_temperature.isChecked()
         self.copy_net = deepcopy(self.net)
 
         # tmp = sys.stdout  # Capture old stdout with a temporary variable
         my_result = StringIO()
         # sys.stdout = my_result  # New stdout liked to the new StrigIO object
-        if self.input_dialog.radio_acopf.isChecked():
-            pp.runopp(self.copy_net, verbose=False,
-                      calculate_voltage_angles=calculate_voltage_angles,
-                      check_connectivity=True, suppress_warnings=True,
-                      switch_rx_ratio=switch_rx_ratio, delta=delta, init=init,
-                      numba=True, trafo3w_losses=trafo3w_losses,
-                      consider_line_temperature=consider_line_temperature,
-                      OPF_VIOLATION=self.input_dialog.OPF_VIOLATION.value()*1e-6,
-                      PDIPM_COSTTOL=self.input_dialog.PDIPM_COSTTOL.value()*1e-6,
-                      PDIPM_GRADTOL=self.input_dialog.PDIPM_GRADTOL.value()*1e-6,
-                      PDIPM_COMPTOL=self.input_dialog.PDIPM_COMPTOL.value()*1e-6,
-                      PDIPM_FEASTOL=self.input_dialog.PDIPM_FEASTOL.value()*1e-6,
-                      PDIPM_MAX_IT=self.input_dialog.PDIPM_MAX_IT.value(),
-                      SCPDIPM_RED_IT=self.input_dialog.SCPDIPM_RED_IT.value())
-        else:
-            pp.rundcopp(self.copy_net, verbose=False, check_connectivity=True,
-                        suppress_warnings=True, switch_rx_ratio=switch_rx_ratio,
-                        delta=delta, trafo3w_losses=trafo3w_losses)
+
+        try:
+            if self.input_dialog.radio_acopf.isChecked():
+                pp.runopp(self.copy_net, verbose=False,
+                          calculate_voltage_angles=calculate_voltage_angles,
+                          check_connectivity=True, suppress_warnings=True,
+                          switch_rx_ratio=switch_rx_ratio, delta=delta, init=init,
+                          numba=True, trafo3w_losses=trafo3w_losses,
+                          consider_line_temperature=consider_line_temperature,
+                          OPF_VIOLATION=self.input_dialog.OPF_VIOLATION.value()*1e-6,
+                          PDIPM_COSTTOL=self.input_dialog.PDIPM_COSTTOL.value()*1e-6,
+                          PDIPM_GRADTOL=self.input_dialog.PDIPM_GRADTOL.value()*1e-6,
+                          PDIPM_COMPTOL=self.input_dialog.PDIPM_COMPTOL.value()*1e-6,
+                          PDIPM_FEASTOL=self.input_dialog.PDIPM_FEASTOL.value()*1e-6,
+                          PDIPM_MAX_IT=self.input_dialog.PDIPM_MAX_IT.value(),
+                          SCPDIPM_RED_IT=self.input_dialog.SCPDIPM_RED_IT.value())
+            else:
+                pp.rundcopp(self.copy_net, verbose=False, check_connectivity=True,
+                            suppress_warnings=True, switch_rx_ratio=switch_rx_ratio,
+                            delta=delta, trafo3w_losses=trafo3w_losses)
+
+        except pp.optimal_powerflow.OPFNotConverged:
+            self.print('Solver did not converge!')
+            return
         # sys.stdout = tmp  # Back to normal
 
         if not self.copy_net['OPF_converged']:
-            title = 'Not converged!'
-            text_content = 'Solver did not converge.'
-            QtWidgets.QMessageBox.critical(self.input_dialog, title, text_content)
+            # title = 'Not converged!'
+            # text_content = 'Solver did not converge.'
+            # QtWidgets.QMessageBox.critical(self.input_dialog, title, text_content)
+            self.print('Solver did not converge!')
             return
 
         ac = self.copy_net["_options"]["ac"]
         if ac is True:
             result = self.copy_net['_ppc_opf']
             init = self.copy_net["_options"]["init"]
             ppopt = ppoption(VERBOSE=True, PF_DC=not ac, INIT=init)
```

### Comparing `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/input.ui` & `electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/input.ui`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/workspace.xml` & `electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim_opf_quadratic-1.2/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/LICENSE` & `electricalsim_opf_quadratic-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/README_PyPI.md` & `electricalsim_opf_quadratic-1.2/README_PyPI.md`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.1/pyproject.toml` & `electricalsim_opf_quadratic-1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim_opf_quadratic"
-version = "1.1"
+version = "1.2"
 author = "Dr. Ing. Ariel S. Loyarte"
 authors = [
   { name="Dr. Ing. Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
 description = "Optimal Power Flow calculation with quadratic costs for the Electrical Grid Simulator (EGS)"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
```

### Comparing `electricalsim_opf_quadratic-1.1/PKG-INFO` & `electricalsim_opf_quadratic-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electricalsim_opf_quadratic
-Version: 1.1
+Version: 1.2
 Summary: Optimal Power Flow calculation with quadratic costs for the Electrical Grid Simulator (EGS)
 Project-URL: Homepage, https://github.com/aloytag/electricalsim-opf-quadratic
 Project-URL: Bug Tracker, https://github.com/aloytag/electricalsim-opf-quadratic/issues
 Project-URL: Repository, https://github.com/aloytag/electricalsim-opf-quadratic
 Author-email: "Dr. Ing. Ariel S. Loyarte" <aloyarte@frsf.utn.edu.ar>
 License: MIT
 License-File: LICENSE
```

