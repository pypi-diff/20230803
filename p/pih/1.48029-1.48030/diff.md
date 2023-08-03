# Comparing `tmp/pih-1.48029.tar.gz` & `tmp/pih-1.48030.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48029.tar", last modified: Wed Aug  2 07:45:33 2023, max compression
+gzip compressed data, was "pih-1.48030.tar", last modified: Thu Aug  3 07:29:45 2023, max compression
```

## Comparing `pih-1.48029.tar` & `pih-1.48030.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.855038 pih-1.48029/
--rw-rw-rw-   0        0        0      261 2023-08-02 07:45:33.855038 pih-1.48029/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.261299 pih-1.48029/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48029/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48029/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48029/pih/console_api.py
--rw-rw-rw-   0        0        0   111167 2023-08-02 07:34:14.000000 pih-1.48029/pih/const.py
--rw-rw-rw-   0        0        0   317983 2023-08-02 07:45:25.000000 pih-1.48029/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48029/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48029/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48029/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48029/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48029/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48029/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48029/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48029/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.823792 pih-1.48029/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-02 07:45:31.000000 pih-1.48029/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:45:31.000000 pih-1.48029/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48029/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-02 07:45:33.855038 pih-1.48029/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 07:29:44.169885 pih-1.48030/
+-rw-rw-rw-   0        0        0      261 2023-08-03 07:29:45.419870 pih-1.48030/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 07:29:45.232406 pih-1.48030/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48030/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48030/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48030/pih/console_api.py
+-rw-rw-rw-   0        0        0   110658 2023-08-03 05:55:46.000000 pih-1.48030/pih/const.py
+-rw-rw-rw-   0        0        0   319265 2023-08-03 07:29:08.000000 pih-1.48030/pih/pih.py
+-rw-rw-rw-   0        0        0    25037 2023-08-03 07:28:58.000000 pih-1.48030/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48030/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48030/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48030/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48030/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48030/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48030/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48030/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:29:45.388620 pih-1.48030/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-03 07:29:43.000000 pih-1.48030/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-03 07:29:44.000000 pih-1.48030/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:29:43.000000 pih-1.48030/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-03 07:29:43.000000 pih-1.48030/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 07:29:43.000000 pih-1.48030/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48030/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:29:45.435501 pih-1.48030/setup.cfg
```

### Comparing `pih-1.48029/pih/collection.py` & `pih-1.48030/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/console_api.py` & `pih-1.48030/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/const.py` & `pih-1.48030/pih/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
 
         PRERECORDING_PIN: int = 10
         PERSON_MINIMAL_PIN: int = 100
         RESERVED_TIME_A_PIN: int = 5
         RESERVED_TIME_B_PIN: int = 6
         RESERVED_TIME_C_PIN: int = 7
         EMPTY_VALUE: str = "xxxxx"
-        EMPTY_EMAIL_VARIANTS: list[str] = ["нет", "-"]
+        EMPTY_EMAIL_VARIANTS: list[str] = ["нет", "-", "no"]
         TELEPHONE_NUMBER_COUNT: int = 4
 
         CARD_REGISTRY_FOLDER_QR_CODE_COUNT: int = 2
 
         CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN: list[str] = ["п", "т", "b", "p", "t", "б"]
     
         #145 - Средний Медицинский Персонал
@@ -947,46 +947,28 @@
 
 class PATH_WS:
 
     NAME: str = f"WS{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
     PATH: str = os.path.join(PATH_FACADE.VALUE, NAME)
 
 
-class PATH_BACKUP:
-
-    class ROBOCOPY_CONFIG:
-
-        NAME: str = "robocopy_config"
-        ROOT: str = os.path.join(PATH_FACADE.VALUE, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
-
-    class COMMAND:
-
-        NAME: str = "command"
-        ROOT: str = os.path.join(
-            PATH_FACADE.VALUE, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
-        
-        ATTACH_SHARED_DISKS: str = os.path.join(ROOT, "attach_shared_disks.ps1")
-
-    
-
 class PATHS:
 
     SHARE: PATH_SHARE = PATH_SHARE()
     SCAN: PATH_SCAN = PATH_SCAN()
     SCAN_TEST = PATH_SCAN_TEST()
     SCAN_SOURCE = PATH_SCAN_SOURCE()
     SCAN_RESULT = PATH_SCAN_RESULT()
     WS_816_SCAN: PATH_WS_816_SCAN = PATH_WS_816_SCAN()
     OMS: PATH_OMS = PATH_OMS()
     IT: PATH_IT = PATH_IT()
     USER: PATH_USER = PATH_USER()
     POLIBASE: PATH_POLIBASE = PATH_POLIBASE()
     POLIBASE_APP_DATA: PATH_POLIBASE_APP_DATA = PATH_POLIBASE_APP_DATA()
     WS: PATH_WS = PATH_WS()
-    BACKUP: PATH_BACKUP = PATH_BACKUP()
     DOCS: PATH_DOCS = PATH_DOCS()
     FONTS: PATH_FONTS = PATH_FONTS()
     MOBILE_HELPER: PATH_MOBILE_HELPER = PATH_MOBILE_HELPER()
     APP_DATA: PATH_APP_DATA = PATH_APP_DATA()
     INDICATIONS: PATH_INDICATIONS = PATH_INDICATIONS()
     STATISTICS: PATH_STATISTICS = PATH_STATISTICS()
     FACADE: PATH_FACADE = PATH_FACADE()
```

### Comparing `pih-1.48029/pih/pih.py` & `pih-1.48030/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from contextlib import contextmanager
 import base64
 import uuid
 import time
 from enum import Enum
 from string import Formatter
 import urllib.parse
+import argparse
+from argparse import Namespace
+from pathlib import Path
 
 from transliterate import translit
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih.collection import  *
@@ -562,14 +565,15 @@
 
 
 class Session(SessionBase):
 
     def __init__(self, input: InputBase = None, output: OutputBase = None):
         super().__init__(input, output)
         self.authenticated: bool = False
+        self.arg_parser: ArgumentParser | None = None
        
     def run_forever_untill_enter_not_pressed(self) -> None:
         try:
             self.output.green("Нажмите Ввод для выхода...")
             input()
         except KeyboardInterrupt:
             pass
@@ -612,17 +616,21 @@
         self.output.error(f"Ты кто такой? Давай, до свидания...")
         self.exit()
 
     @property
     def argv(self) -> list[str]:
         return sys.argv[1:] if len(sys.argv) > 1 else []
     
-    def arg(self, index: int = 0, default_value: Any | None = None) -> str:
+    def arg(self, index: int = 0, default_value: Any | None = None) -> str | Namespace:
         return DataTool.by_index(self.argv, index, default_value)
-
+    
+    @property
+    def arg_namespace(self) -> Namespace:
+        return self.arg_parser.parse_args()
+    
     @property
     def file_path(self) -> str:
         return sys.argv[0]
 
     @property
     def is_standalone(self) -> bool:
         return self.file_path.endswith(FILE.EXTENSION.EXE)
@@ -919,35 +927,35 @@
         os.system('cls' if os.name == 'nt' else 'clear')
 
     def pih_title(self) -> None:
         self.cyan(self.text_color(Fore.WHITE, "███ ███ █┼█"))
         self.cyan(
             self.text_color(Fore.WHITE, "█▄█ ┼█┼ █▄█"))
         self.cyan(self.text_color(Fore.WHITE, "█┼┼ ▄█▄ █┼█") +
-                         self.text_color(Fore.BLACK, f" {PIH.VERSION.local()}"))
+                         self.text_color(Fore.BLACK, f" {PIH.VERSION.value}"))
         self.new_line()
 
     def rpc_service_header(self, host: str, port: int, description: str) -> None:
         self.blue("PIH service")
-        self.blue(f"Version: {PIH.VERSION.local()}")
+        self.blue(f"Version: {PIH.VERSION.value}")
         #self.blue(f"PyPi Version: {PIH.VERSION.remote()}")
         self.green(f"Service host: {host}")
         self.green(f"Service port: {port}")
         self.green(f"Service name: {description}")
 
     def service_header(self, information: ServiceInformation) -> None:
+        self.blue("Service starting")
+        self.set_indent(1)
         if information.isolated:
             self.blue(f"[Isolate]")
-        self.blue("Запуск сервиса")
-        #self.blue(f"PIH версия: {PIH.VERSION.remote()}")
-        self.green(f"Хост: {information.host}")
-        self.green(f"Порт: {information.port}")
-        self.green(f"Имя сервиса: {information.name}")
-        self.green(
-            f"Идентификатор процесса: {information.pid}")
+        self.value("Host", information.host)
+        self.value("Port", information.port)
+        self.value("Service name", information.name)
+        self.value("PID process",  information.pid)
+        self.set_indent(0)
 
     def free_marks(self, show_guest_marks: bool, use_index: bool = False, sort_by_tab_number: bool = True) -> None:
         def sort_function(item: Mark) -> Any:
             return item.TabNumber if sort_by_tab_number else item.GroupName
         self.table_with_caption_first_title_is_centered(ResultTool.sort(PIH.RESULT.MARK.free_list(show_guest_marks), sort_function), "Свободные карты доступа:", use_index)
 
     def guest_marks(self, use_index: bool = False) -> None:
@@ -1600,16 +1608,14 @@
             self.input: Input = input
         if session is None: 
             PIH.session: Session = Session(input, output)
         else:
             self.session: Session = session
         
     class MIO:
-
-        NAME: str = "mio"
     
         ANSWER: dict[str, list[str]] = defaultdict(list)
 
         @staticmethod
         def create_output(recipient: str | Enum, say_hello: bool = True) -> Output:
             from MobileHelperCore.api import MobileOutput, MobileSession, Flags, format_given_name
             recipient = recipient if isinstance(recipient, str) else EnumTool.get(recipient)
@@ -1634,28 +1640,20 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        class MIO:
-            
-            @staticmethod
-            def local() -> str:
-                return "1.48022"  
-
-        @staticmethod
-        def local() -> str:
-            return "1.48029"
+        value: str = "1.48030"
 
         @staticmethod
         def need_update() -> bool:
             return False
-            #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
+            #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
 
         NAME: str = "RecipientWaitingForInput"
 
         @staticmethod
         def _get_name(group_name: str, recipient:str) -> str:
@@ -1681,16 +1679,22 @@
             return DataTool.is_not_none(result) and (DataTool.is_none(result.timeout) or (DateTimeTool.now() - result.timestamp).seconds < result.timeout)
 
     class ERROR:
 
         notify_about_error: bool = True
 
         @staticmethod
+        def service_host_is_unchanachable(host: str) -> None:
+             PIH.output.error(
+                f"Sorry, but service can't be start, cause service host is unchangeble.\n You are trying to start service on {PIH.DATA.FORMAT.donain(PIH.OS.host())}, but service must be started on {PIH.DATA.FORMAT.donain(host)}")
+
+
+        @staticmethod
         def create_error_header(details: str) -> str:
-            return f"\nВерсия: {PIH.VERSION.local()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
+            return f"\nВерсия: {PIH.VERSION.value}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
 
         @contextmanager
         def detect() -> bool:
             try:
                 yield True
             except Exception as error:
                 PIH.ERROR.global_except_hook(type(error), error, error.__traceback__)
@@ -1703,15 +1707,23 @@
                if_else(DataTool.is_none(message), None, PIH.output.red(message))
         
         @staticmethod
         def rpc_error_handler(details: str, code: tuple, description: ServiceRoles, command: ServiceCommands) -> None:
             if isinstance(command, ServiceCommands):
                 if code == StatusCode.UNAVAILABLE:
                     if PIH.ERROR.notify_about_error:
-                        PIH.output.error(f"Error: {details}")
+                        PIH.output.error(f"Error:")
+                        PIH.output.set_indent(1)
+                        for item in details.splitlines():
+                            parts: list[str] = item.split(": ")
+                            if len(parts) > 1:
+                                PIH.output.value(parts[0], j(parts[1:]))  
+                            else:
+                                PIH.output.write_line(parts[0]) 
+                        PIH.output.set_indent(0)    
                     return
                 elif code == StatusCode.DEADLINE_EXCEEDED or details.lower().find("stream removed") != -1:
                     return
                 else:
                     if PIH.ERROR.notify_about_error:
                         PIH.LOG.debug(
                             PIH.ERROR.create_error_header(details), LogMessageFlags.ERROR)
@@ -2287,15 +2299,15 @@
             argv_str: str = ""
             if not DataTool.is_empty(argv):
                 argv_str = " ".join(argv)
                 argv_str = f"({argv_str})"
             login: str = PIH.session.get_login()
             user: User = PIH.RESULT.USER.by_login(login).data
             PIH.EVENT.send(Events.SESSION_STARTED, (user.name, login,
-                                                        f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.local()}", PIH.OS.host()))
+                                                        f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.value}", PIH.OS.host()))
 
         @staticmethod
         def backup_robocopy_job_was_started(name: str, job_status: RobocopyJobStatus) -> None:
             PIH.EVENT.send(
                 Events.BACKUP_ROBOCOPY_JOB_WAS_STARTED, (name, job_status.pid))
 
         @staticmethod
@@ -2491,15 +2503,15 @@
 
         class DATA_HOLDER:
             long_operation_listeners: list[Callable[[None], None]] = []
 
         @staticmethod
         def check_on_host_chanchable(role_or_information: ServiceRoles | ServiceInformationBase) -> bool:
             description: ServiceDescription = ServiceRoles.description(role_or_information)
-            return not description.host_changeable and StringTool.contains(PIH.OS.host(), description.host)
+            return description.host_changeable or StringTool.contains(PIH.OS.host(), description.host)
 
         @staticmethod
         def call_listeners_on_long_operation() -> None:
             for listener in PIH.SERVICE.DATA_HOLDER.long_operation_listeners:
                 listener()
 
         @staticmethod
@@ -2667,49 +2679,50 @@
                       max_workers: int | None = None, 
                       stop_before: bool = True, 
                       depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
                       isolate: bool = False,
                       show_output: bool = True) -> None:
                 host: str = PIH.OS.host()
                 service_description: ServiceInformationBase = ServiceRoles.description(role_or_information)
-                if isolate:
-                     PIH.SERVICE.ADMIN.isolate(service_description)
-                else:
-                    if not PIH.DATA.contains(host, service_description.host):
-                        if service_description.host_changeable:
+                if PIH.SERVICE.check_on_host_chanchable(service_description):
+                    if isolate:
+                        PIH.SERVICE.ADMIN.isolate(service_description)
+                    else:
+                        if not PIH.DATA.contains(host, service_description.host):
                             PIH.SERVICE.ADMIN.change_host_on_local(service_description)
-                        else:
-                            raise Exception("")
-                    if stop_before:
-                        if PIH.SERVICE.check_accessibility(service_description):
-                            PIH.SERVICE.ADMIN.stop(service_description)
-                def internal_start_handler(service: IService) -> None:
-                    if PIH.OS.is_linux():
-                        PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, host)
-                        PIH.PATH.mount_facade_storage_on_linux_host(host)
-                    if starts_handler is not None:
-                        if starts_handler.__code__.co_argcount == 1:
-                            starts_handler(service)
-                        else:
-                            starts_handler()
-                service: IService = RPC.create_service()
-                from inspect import signature, Signature
-                def internal_call_handler(command_name: str, parameter_list: ParameterList, context) -> Any | None:
-                    if not DataTool.is_empty(call_handler):
-                        sig: Signature = signature(call_handler)
-                        arg_count: int = len(sig.parameters) - ("self" in sig.parameters)
-                        if arg_count == 3:
-                            if DataTool.is_in(sig.parameters, "context"):
-                                return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, context) 
-                            if DataTool.is_in(sig.parameters, "subscribtion_result"):
-                                return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, PIH.DATA.EXTRACT.subscribtion_result(parameter_list))    
-                        return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list) 
-                    return None   
-                service.serve(service_description, internal_call_handler,
-                              internal_start_handler, max_workers, depends_on_list, show_output)
+                        if stop_before:
+                            if PIH.SERVICE.check_accessibility(service_description):
+                                PIH.SERVICE.ADMIN.stop(service_description)
+                    def internal_start_handler(service: IService) -> None:
+                        if PIH.OS.is_linux():
+                            PIH.PATH.make_directory_if_not_exists(PATHS.FACADE.LINUX_MOUNT_POINT_PATH, host)
+                            PIH.PATH.mount_facade_storage_on_linux_host(host)
+                        if starts_handler is not None:
+                            if starts_handler.__code__.co_argcount == 1:
+                                starts_handler(service)
+                            else:
+                                starts_handler()
+                    service: IService = RPC.create_service()
+                    from inspect import signature, Signature
+                    def internal_call_handler(command_name: str, parameter_list: ParameterList, context) -> Any | None:
+                        if not DataTool.is_empty(call_handler):
+                            sig: Signature = signature(call_handler)
+                            arg_count: int = len(sig.parameters) - ("self" in sig.parameters)
+                            if arg_count == 3:
+                                if DataTool.is_in(sig.parameters, "context"):
+                                    return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, context) 
+                                if DataTool.is_in(sig.parameters, "subscribtion_result"):
+                                    return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, PIH.DATA.EXTRACT.subscribtion_result(parameter_list))    
+                            return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list) 
+                        return None   
+                    service.serve(service_description, internal_call_handler,
+                                internal_start_handler, max_workers, depends_on_list, show_output)
+                else:
+                    PIH.ERROR.service_host_is_unchanachable(
+                        service_description.host)
 
             @staticmethod
             def stop(role_or_information: ServiceRoles | ServiceInformationBase, check_on_started: bool = True, direct_call: bool = False) -> bool:
                 description: ServiceDescription = ServiceRoles.description(role_or_information)
                 if not check_on_started or PIH.SERVICE.check_accessibility(description):
                     if PIH.SERVICE.is_service_as_listener(description) or direct_call:
                         PIH.SERVICE.call(description, ServiceCommands.stop_service)
@@ -2804,21 +2817,19 @@
                     for service_command_item in description.commands:
                         service_command_item: ServiceCommands = service_command_item
                         PIH.SERVICE.command_map[service_command_item.name] = description
             return PIH.SERVICE.command_map[value.name] if value.name in PIH.SERVICE.command_map else None
 
         @staticmethod
         def get_host(role_or_information: ServiceRoles | ServiceInformationBase) -> str:
-            def add_donain(value: str) -> str:
-                return if_else(value.endswith(AD.DOMAIN_DNS), value, lambda: j((value, AD.DOMAIN_DNS), "."))
             information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
             if isinstance(information, ServiceDescription):
                 if not DataTool.is_empty(information.port):
-                    return add_donain(information.host)
-            return add_donain((PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host)
+                    return PIH.DATA.FORMAT.donain(information.host)
+            return PIH.DATA.FORMAT.donain((PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host)
 
         @staticmethod
         def get_port(role_or_information: ServiceRoles | ServiceInformationBase) -> int | None:
             information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
             if isinstance(information, ServiceDescription):
                 if not DataTool.is_empty(information.port):
                     return information.port
@@ -2933,14 +2944,26 @@
             @staticmethod
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
+        class BACKUP:
+
+            SPLITTER: str = "::"
+
+            @staticmethod
+            def get_job_full_name(name: str, source: str, destination: str) -> str:
+                return PIH.DATA.BACKUP.SPLITTER.join([source, destination, name])
+            
+            @staticmethod
+            def get_job_status_name(name: str, source: str, destination: str) -> str:
+                return PIH.DATA.BACKUP.SPLITTER.join(["robocopy_job_status", PIH.DATA.BACKUP.get_job_full_name(name, source, destination)])
+
         @staticmethod
         def translit(value, language_code=None, reversed=False, strict=False):
             return translit(value, language_code, reversed, strict)
 
         @staticmethod
         def find_variables(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
@@ -3388,14 +3411,18 @@
                 @staticmethod
                 def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
                     return not DataTool.is_empty(value.temperature)
 
         class FORMAT:
 
             @staticmethod
+            def donain(value: str) -> str:
+                return if_else(value.endswith(AD.DOMAIN_DNS), value, lambda: j((value, AD.DOMAIN_DNS), "."))
+
+            @staticmethod
             def variable(value: str, parse: bool = True) -> str:
                 fields: list[str] | None = if_else(parse, [name for _, name, _, _ in Formatter().parse(value) if name], [value])
                 if DataTool.is_empty(fields):
                     return value
                 variable_name: str = fields[0]
                 return PIH.DATA.get_variable_value(variable_name)
 
@@ -5475,18 +5502,16 @@
             @staticmethod
             def send_message(value: str, recipient: str | Enum, flags: int | None = None) -> bool:    
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_mobile_helper_message, (value, recipient if isinstance(recipient, str) else EnumTool.get(recipient), flags)))
 
         class BACKUP:
 
             @staticmethod
-            def attach_shared_disks() -> bool:
-                output: str = str(PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
-                    [CONST.POWERSHELL.NAME, PATH_BACKUP.COMMAND.ATTACH_SHARED_DISKS], HOSTS.BACKUP_WORKER.NAME, interactive=None, run_from_system_account=True), True, True).stdout)
-                return output.strip().count("Attached          : True") == 2
+            def attach_shared_disks(name: str | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.attach_shared_disks, (name, )))
 
             @staticmethod
             def start_robocopy_job(name: str | None = None, source: str | None = None, destination: str | None = None, force: bool = False) -> bool:
                 return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.robocopy_start_job, (name, source, destination, force)))
 
             @staticmethod
             def start_robocopy_job_by_name(value: str, force: bool = False) -> bool:
@@ -5812,15 +5837,15 @@
                     break
             except KeyboardInterrupt:
                 self.output.new_line()
                 self.output.error("Повтор предыдущих действия")
                 self.output.new_line()
                 if index > 0:
                     previous_change = True
-                    # self.show_action_values()
+                    #self.show_action_values()
                     #index = index - 1
                 else:
                     continue
 
     def show_action_values(self) -> None:
         def label(item: ActionValue, _):
             return item.caption
@@ -5853,14 +5878,15 @@
     D_TN = D.TELEPHONE_NUMBER
     D_MR = D.MATERIALIZED_RESOURCES
     D_FL = D.FILTER
     D_Ex = D.EXTRACT
     D_Ex_E = D_Ex.EVENT
     D_M = D.MARK
     D_C = D.CHECK
+    D_B = D.BACKUP
     D_STAT = D.STATISTICS
     A = root.ACTION
     
     A_D = A.DOCUMENTS
     A_QR = A.QR_CODE
     A_I = A.INDICATION
     A_I_CT = A_I.CT
```

### Comparing `pih-1.48029/pih/rpc.py` & `pih-1.48030/pih/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import grpc
 from grpc import Server
 from concurrent import futures
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 import psutil
+from argparse import ArgumentParser
 
 @dataclass
 class Error(BaseException):
     details: str
     code: tuple
 
 class IService:
@@ -268,31 +269,37 @@
                 from pih import A
             else:
                 A = sys.modules["pih.pih"].A
             max_workers = max_workers or RPC.Service.MAX_WORKERS
             service_description: ServiceDescription = role_or_information if isinstance(
                 role_or_information, ServiceInformationBase) else A.CT_SR.description(role_or_information)
             self.description = service_description
-            isolate_arg: str | None = A.SE.arg(0, None)
+            A.SE.arg_parser = ArgumentParser(description="Service help")
+            A.SE.arg_parser.add_argument("--isolate", type=str, help="Service isolate flag")
+            isolate_arg: str | None = None
+            try:
+                isolate_arg = A.SE.arg_parser.parse_known_args().isolate
+            except AttributeError as error:
+                pass
             if A.D.is_not_none(isolate_arg):
                 self.description.isolated = isolate_arg.lower() in [
                     "true", "1", "yes"]
-            self.description.pih_version = A.V.local()
+            self.description.pih_version = A.V.value
             self.description.host = A.SRV.create_host(self.description)
             self.description.port = A.SRV.create_port(self.description)
             self.information = A.D.fill_data_from_source(ServiceInformation(), self.description)
             self.information.pid = A.OS.get_pid()
             if A.D_C.empty(RPC.service):
                 RPC.service_description = self.description
                 RPC.service_information = self.information
                 RPC.service = self
             if show_output:
                 A.O.init()
                 A.O.service_header(self.information)
-                A.O.good(f"Сервис был запущен!")
+                A.O.good(f"Service was started!")
             self.server = grpc.server(
                 futures.ThreadPoolExecutor(max_workers=max_workers))
             if RPC.server is None:
                 RPC.server = self.server
             pb2_grpc.add_UnaryServicer_to_server(
                 RPC.UnaryService(self, self.description, call_handler), self.server)
             try:
@@ -431,15 +438,15 @@
                     if sc == SC.ping:
                         timeout = CONST.RPC.TIMEOUT_FOR_PING
                     else:
                         timeout = CONST.RPC.TIMEOUT
             return RPC.CommandClient(service_host, service_port).call_command(sc.name, A.D.rpc_represent(parameters), timeout).data
         except grpc.RpcError as error:
             code: tuple = error.code()
-            details: str = f"Service role:{information.name}\nHost: {service_host}:{service_port}\nCommand: {sc.name}\nDetails: {error.details()}\nCode: {code}"
+            details: str = f"Service role name: {information.name}\nHost: {service_host}:{service_port}\nCommand: {sc.name}\nDetails: {error.details()}\nCode: {code}"
             A.O.init()
             A.ER.rpc_error_handler(details, code, information, sc)
 
     @staticmethod
     def call_service_command(command: SC, parameters: Any | None = None, timeout: int | None = None) -> str | None:
         return RPC.call_service(None, command, parameters, timeout)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pih-1.48029/pih/rpcCommandCall_pb2.py` & `pih-1.48030/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48030/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/rpc_collection.py` & `pih-1.48030/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/rpc_const.py` & `pih-1.48030/pih/rpc_const.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     #WORKSTATION
     reboot: int = auto()
     shutdown: int = auto()
     log_out: int = auto()
     #Robocopy::Job
     robocopy_start_job: int = auto()
     robocopy_get_job_status_list: int = auto()
+    attach_shared_disks: int = auto()
     #DataStorage::Storage value
     set_storage_value: int = auto()
     get_storage_value: int = auto()
     #Resource Manager
     get_resource_status_list: int = auto()
     send_mobile_helper_message: int = auto()
```

### Comparing `pih-1.48029/pih/service_example.py` & `pih-1.48030/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/tools.py` & `pih-1.48030/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih/widgets.py` & `pih-1.48030/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48029/pih_setup.py` & `pih-1.48030/pih_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             shutil.rmtree(file_path)
     except Exception as error:
         print("Failed to delete %s. Reason: %s" % (file_path, error))
 
 #This call to setup() does all the work
 setup(
     name=PIH.NAME,
-    version=PIH.VERSION.local(),
+    version=PIH.VERSION.value,
     description="PIH library",
     long_description_content_type="text/markdown",
     url="https://pacifichosp.com/",
     author="Nikita Karachentsev",
     author_email="it@pacifichosp.com",
     license="MIT",
     classifiers=[],
```

