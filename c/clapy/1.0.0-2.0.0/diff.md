# Comparing `tmp/clapy-1.0.0.tar.gz` & `tmp/clapy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clapy-1.0.0.tar", last modified: Sun Apr 30 03:17:59 2023, max compression
+gzip compressed data, was "/home/benny/Repos/clapy/dist/.tmp-e8x9smze/clapy-2.0.0.tar", last modified: Thu Aug  3 09:41:23 2023, max compression
```

## Comparing `clapy-1.0.0.tar` & `clapy-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-04-30 03:17:59.308412 clapy-1.0.0/
--rw-rw-r--   0 benny     (1000) benny     (1000)     1074 2023-04-14 11:40:51.000000 clapy-1.0.0/LICENCE
--rw-rw-r--   0 benny     (1000) benny     (1000)     4585 2023-04-30 03:17:59.308412 clapy-1.0.0/PKG-INFO
--rw-rw-r--   0 benny     (1000) benny     (1000)     2796 2023-04-30 01:05:44.000000 clapy-1.0.0/README.md
--rw-rw-r--   0 benny     (1000) benny     (1000)     1075 2023-04-30 02:59:04.000000 clapy-1.0.0/pyproject.toml
--rw-rw-r--   0 benny     (1000) benny     (1000)       38 2023-04-30 03:17:59.308412 clapy-1.0.0/setup.cfg
-drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-04-30 03:17:59.304411 clapy-1.0.0/src/
-drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-04-30 03:17:59.304411 clapy-1.0.0/src/clapy.egg-info/
--rw-rw-r--   0 benny     (1000) benny     (1000)     4585 2023-04-30 03:17:59.000000 clapy-1.0.0/src/clapy.egg-info/PKG-INFO
--rw-rw-r--   0 benny     (1000) benny     (1000)      333 2023-04-30 03:17:59.000000 clapy-1.0.0/src/clapy.egg-info/SOURCES.txt
--rw-rw-r--   0 benny     (1000) benny     (1000)        1 2023-04-30 03:17:59.000000 clapy-1.0.0/src/clapy.egg-info/dependency_links.txt
--rw-rw-r--   0 benny     (1000) benny     (1000)       51 2023-04-30 03:17:59.000000 clapy-1.0.0/src/clapy.egg-info/requires.txt
--rw-rw-r--   0 benny     (1000) benny     (1000)       81 2023-04-30 03:17:59.000000 clapy-1.0.0/src/clapy.egg-info/top_level.txt
--rw-rw-r--   0 benny     (1000) benny     (1000)     2941 2023-04-29 23:59:22.000000 clapy-1.0.0/src/common.py
--rw-rw-r--   0 benny     (1000) benny     (1000)    11894 2023-04-30 00:15:17.000000 clapy-1.0.0/src/dependency_injection.py
--rw-rw-r--   0 benny     (1000) benny     (1000)     7241 2023-04-30 00:07:07.000000 clapy-1.0.0/src/engine.py
--rw-rw-r--   0 benny     (1000) benny     (1000)      112 2023-04-29 23:56:23.000000 clapy-1.0.0/src/exceptions.py
--rw-rw-r--   0 benny     (1000) benny     (1000)      647 2023-04-27 10:30:51.000000 clapy-1.0.0/src/generics.py
--rw-rw-r--   0 benny     (1000) benny     (1000)     1025 2023-04-30 00:10:52.000000 clapy-1.0.0/src/outputs.py
--rw-rw-r--   0 benny     (1000) benny     (1000)     3170 2023-04-28 07:25:03.000000 clapy-1.0.0/src/pipeline.py
--rw-rw-r--   0 benny     (1000) benny     (1000)     2996 2023-04-30 00:16:41.000000 clapy-1.0.0/src/services.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-08-03 09:41:23.000000 clapy-2.0.0/
+-rw-rw-r--   0 benny     (1000) benny     (1000)     1074 2023-04-14 11:40:51.000000 clapy-2.0.0/LICENCE
+-rw-rw-r--   0 benny     (1000) benny     (1000)    18662 2023-08-03 09:41:23.000000 clapy-2.0.0/PKG-INFO
+-rw-rw-r--   0 benny     (1000) benny     (1000)    16348 2023-08-03 07:35:09.000000 clapy-2.0.0/README.md
+-rw-rw-r--   0 benny     (1000) benny     (1000)     1239 2023-07-23 11:55:47.000000 clapy-2.0.0/pyproject.toml
+-rw-rw-r--   0 benny     (1000) benny     (1000)       38 2023-08-03 09:41:23.000000 clapy-2.0.0/setup.cfg
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-08-03 09:41:23.000000 clapy-2.0.0/src/
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy/
+-rw-rw-r--   0 benny     (1000) benny     (1000)        0 2023-05-12 05:31:14.000000 clapy-2.0.0/src/clapy/__init__.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     4715 2023-07-23 12:00:02.000000 clapy-2.0.0/src/clapy/common.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     8644 2023-08-03 07:32:19.000000 clapy-2.0.0/src/clapy/dependency_injection.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)    11335 2023-07-23 11:37:40.000000 clapy-2.0.0/src/clapy/engine.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)      227 2023-06-23 15:07:56.000000 clapy-2.0.0/src/clapy/exceptions.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     3790 2023-08-03 09:13:00.000000 clapy-2.0.0/src/clapy/outputs.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     4794 2023-07-23 11:45:44.000000 clapy-2.0.0/src/clapy/pipeline.py
+-rw-rw-r--   0 benny     (1000) benny     (1000)     2621 2023-07-23 11:57:03.000000 clapy-2.0.0/src/clapy/services.py
+drwxrwxr-x   0 benny     (1000) benny     (1000)        0 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/
+-rw-rw-r--   0 benny     (1000) benny     (1000)    18662 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/PKG-INFO
+-rw-rw-r--   0 benny     (1000) benny     (1000)      381 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)        1 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)       51 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/requires.txt
+-rw-rw-r--   0 benny     (1000) benny     (1000)        6 2023-08-03 09:41:23.000000 clapy-2.0.0/src/clapy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `clapy-1.0.0/LICENCE` & `clapy-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `clapy-1.0.0/src/dependency_injection.py` & `clapy-2.0.0/src/clapy/dependency_injection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,288 +1,211 @@
 import inspect
-import os
 import re
-from abc import ABC, abstractmethod
-from typing import List, Optional, Type
+from typing import List, Tuple
 
 from dependency_injector import containers, providers
 
-from common import DIR_EXCLUSIONS, FILE_EXCLUSIONS, apply_exclusion_filter, import_class_by_namespace
-from engine import PipelineFactory, UseCaseInvoker, construct_usecase_registry
-from exceptions import DuplicateServiceError
-from generics import TServiceType
-from pipeline import IPipe
-from services import IPipelineFactory, IServiceProvider, IUseCaseInvoker
+from .common import Common
+from .engine import Engine, PipelineFactory, UseCaseInvoker
+from .exceptions import DuplicateServiceError
+from .pipeline import IPipe
+from .services import IPipelineFactory, IServiceProvider, IUseCaseInvoker
 
-class IDependencyInjectorServiceProvider(IServiceProvider, ABC):
-    '''Clapy's default service provider interface for using Clapy with dependency_injector.'''
 
-    @abstractmethod
-    def register_service(
-        self,
-        provider_method: Type,
-        concrete_type: Type[TServiceType],
-        interface_type: Optional[Type[TServiceType]] = None,
-        *args) -> None:
-        '''
-        Summary
-        -------
-        Registers a service in the dependency_injector container with its dependencies.
-        
-        Parameters
-        ----------
-        `provider_method` The lifetime of the service, defined using the providers module from dependency_injector.\n
-        `concrete_type` The concrete implementation of the service being registered. Can be registered on its own.\n
-        `interface_type` The optional interface that the concrete type implements.\n
-        `*args` Any required dependencies for this service to be constructed that are not registered in the dependency_injector container.
-        
-        '''
-        pass
-
-    
-    @abstractmethod
-    def register_usecase_services(
-        self,
-        usecase_scan_locations: Optional[List[str]] = ["."],
-        directory_exclusion_patterns: Optional[List[str]] = [],
-        file_exclusion_patterns: Optional[List[str]] = []) -> None:
-        '''
-        Summary
-        -------
-        Scans and registers use case pipes under the specified locations to the dependency_injector
-        container.
-        
-        Parameters
-        ----------
-        `usecase_scan_locations` An optional list of locations within the project where the usecase services
-        should be scanned for.\n
-        `directory_exclusion_patterns` An optional list of regular expression patterns used to exclude directories
-        from being scanned.\n
-        `file_exclusion_patterns`An optional list of regular expression patterns used to exclude files
-        from being scanned and registered.
-        
-        '''
-        pass
-
-    @abstractmethod
-    def construct_usecase_invoker(
-        self,
-        usecase_locations: Optional[List[str]] = ["."],
-        directory_exclusion_patterns: Optional[List[str]] = [],
-        file_exclusion_patterns: Optional[List[str]] = []) -> IUseCaseInvoker:
-        '''
-        Summary
-        -------
-        Builds and registers the dependencies of Clapy's use case invoker, returning the built use case
-        invoker.
-        
-        Parameters
-        ----------
-        `usecase_scan_locations` An optional list of locations within the project where the usecase services
-        should be scanned for.\n
-        `directory_exclusion_patterns` An optional list of regular expression patterns used to exclude directories
-        from being scanned.\n
-        `file_exclusion_patterns`An optional list of regular expression patterns used to exclude files
-        from being scanned and registered.
-        
-        Returns
-        -------
-        An instance of the concrete implementation for the `IUseCaseInvoker`.
-        
-        '''
-        pass
-
-
-class DependencyInjectorServiceProvider(IDependencyInjectorServiceProvider):
+class DependencyInjectorServiceProvider(IServiceProvider):
     '''
     Clapy's default service provider implementation for using Clapy with dependency_injector. Uses
-    DeclarativeContainer from dependency_injector.
+    the DeclarativeContainer from dependency_injector.
 
     '''
 
     def __init__(self):
         self._container = containers.DeclarativeContainer()
 
-
-    def get_service(self, service: Type[TServiceType]) -> TServiceType:
+    def get_service(self, service: type) -> object:
         '''
         Summary
         -------
-        Retrieves the specified service from the dependency_injectior container.
-        
+        Retrieves the specified service from the dependency_injector container.
+
         Parameters
         ----------
         `service` The service to be retrieved.
 
         Exceptions
         ----------
         Raises a `LookupError` if the service could not be resolved.
-        
+
         Returns
         -------
         An instance of the requested service type with a lifetime as defined on the container.
-        
+
         '''
-        _ServiceName = self._generate_service_name(service)
+        _ServiceName, _GenerationSuccess = self._try_generate_service_name(service)
 
-        if _Service := self._container.providers.get(_ServiceName):
-            return _Service()
-        else:
-            raise LookupError(f"Was not able to retrieve '{service.__name__}' from DI container.")
+        if _GenerationSuccess:
+            _Service = self._container.providers.get(_ServiceName)
+
+            if _Service is not None:
+                return _Service()
 
+        raise LookupError(f"Was not able to retrieve '{service.__name__}' from DI container.")
 
-    def register_service(self, provider_method: Type, concrete_type: Type[TServiceType], interface_type: Optional[Type[TServiceType]] = None, *args) -> None:
+    def register_service(
+            self,
+            provider_method: type,
+            concrete_type: type,
+            interface_type: type = None, # type: ignore
+            *args) -> None:
         '''
         Summary
         -------
         Registers a service in the dependency_injector container with its dependencies. If dependencies of the service
-        are detected to be registered in the container, they will be linked to the service automatically.
-        
+        are detected to be registered in the container, they will be linked to the service automatically. Dependencies
+        are detected via the type hints of the service's constructor's parameters.
+
         Parameters
         ----------
         `provider_method` The lifetime of the service, defined using the providers module from dependency_injector.\n
         `concrete_type` The concrete implementation of the service being registered. Can be registered on its own.\n
         `interface_type` The optional interface that the concrete type implements.\n
-        `*args` Any required dependencies for this service to be constructed that are not registered in the dependency_injector container.
-        
+        `*args` Any required dependencies for this service to be constructed that are not registered in the
+        dependency_injector container.
+
         Exceptions
         ----------
-        Raises `DuplicateServiceError` if the dependency_injector container already contains a service of the same type.
-        
+        Raises `DuplicateServiceError` if the dependency_injector container already contains a service of the same type.\n
+        Raises `ValueError` if unable to generate a service name for the service.
+
         '''
-        _DependencyName = self._generate_service_name(interface_type if interface_type is not None else concrete_type)
+        _DependencyName, _GenerationSuccess = self._try_generate_service_name(interface_type or concrete_type)
+
+        if not _GenerationSuccess:
+            raise ValueError(f"Failed to generate service name for {interface_type or concrete_type}.")
 
         if hasattr(self._container, _DependencyName):
-            raise DuplicateServiceError(f"An already registered service is conflicting with {interface_type if interface_type is not None else concrete_type}.")
+            raise DuplicateServiceError(f"An already registered service is conflicting with {interface_type or concrete_type}.")
 
-        _ConstructorDependencies = [_Param for _Param in inspect.signature(concrete_type.__init__).parameters.values()
-                                        if _Param.annotation != inspect.Parameter.empty and self._has_service(_Param.annotation)]
+        _ConstructorDependencies = [_Param for _Param in inspect.signature(concrete_type.__init__).parameters.values() # type: ignore
+                                    if _Param.annotation != inspect.Parameter.empty
+                                    and self._has_service(_Param.annotation)]
 
         if not _ConstructorDependencies:
             setattr(self._container, _DependencyName, provider_method(concrete_type, *args))
         else:
             _SubDependencies = []
             for _Dependency in _ConstructorDependencies:
-                _SubDependencyName = self._generate_service_name(_Dependency.annotation)
+                _SubDependencyName, _ = self._try_generate_service_name(_Dependency.annotation)
                 _SubDependencies.append(getattr(self._container, _SubDependencyName))
 
             setattr(self._container, _DependencyName, provider_method(concrete_type, *_SubDependencies, *args))
 
-
-    def register_usecase_services(
-        self,
-        usecase_scan_locations: Optional[List[str]] = ["."],
-        directory_exclusion_patterns: Optional[List[str]] = [],
-        file_exclusion_patterns: Optional[List[str]] = []) -> None:
+    def register_pipe_services(
+            self,
+            usecase_scan_locations: List[str] = ["."],
+            directory_exclusion_patterns: List[str] = [],
+            file_exclusion_patterns: List[str] = []) -> None:
         '''
         Summary
         -------
         Scans and registers use case pipes under the specified locations to the dependency_injector
-        container. There must be a class within the file that matches by name. For this class to be
-        registered, it must also implement the IPipe interface. Registered using providers.Factory. 
-        
+        container. For this class to be registered, it must implement the IPipe interface. Registered
+        using `providers.Factory`.
+
         Parameters
         ----------
         `usecase_scan_locations` An optional list of locations within the project where the usecase services
         should be scanned for. If none are provided, the entire project will be scanned.\n
         `directory_exclusion_patterns` An optional list of regular expression patterns used to exclude directories
         from being scanned.\n
         `file_exclusion_patterns`An optional list of regular expression patterns used to exclude files
         from being scanned and registered.
-        
-        '''
-        directory_exclusion_patterns = directory_exclusion_patterns + DIR_EXCLUSIONS
-        file_exclusion_patterns = file_exclusion_patterns + FILE_EXCLUSIONS
 
+        '''
         for _Location in usecase_scan_locations:
-            for _Root, _Directories, _Files in os.walk(_Location):
+            _ClassesWithNamespaces = Common.get_all_classes(_Location, directory_exclusion_patterns, file_exclusion_patterns)
 
-                apply_exclusion_filter(_Directories, directory_exclusion_patterns)
-                apply_exclusion_filter(_Files, file_exclusion_patterns)
-
-                for _File in _Files:
-                    _Namespace = _Root.replace('/', '.') + "." + _File[:-3]
-                    _Class = import_class_by_namespace(_Namespace)
-
-                    if issubclass(_Class, IPipe):
-                        self.register_service(providers.Factory, _Class)
-
-
-    def construct_usecase_invoker(
-        self,
-        usecase_scan_locations: Optional[List[str]] = ["."],
-        directory_exclusion_patterns: Optional[List[str]] = [],
-        file_exclusion_patterns: Optional[List[str]] = []) -> IUseCaseInvoker:
+            for _ClassNamespace in _ClassesWithNamespaces:
+                if issubclass(_ClassNamespace[0], IPipe):
+                    self.register_service(providers.Factory, _ClassNamespace[0])
+
+    def configure_clapy_services(
+            self,
+            usecase_scan_locations: List[str] = ["."],
+            directory_exclusion_patterns: List[str] = [],
+            file_exclusion_patterns: List[str] = []) -> None:
         '''
         Summary
         -------
         Builds and registers the dependencies of Clapy's use case invoker, returning the built use case
         invoker. Will scan for use cases under the specified locations, or the entire project if
         locations are not provided.
-        
+
         Parameters
         ----------
         `usecase_scan_locations` An optional list of locations within the project where the usecase services
         should be scanned for. If none are provided, the entire project will be scanned.\n
         `directory_exclusion_patterns` An optional list of regular expression patterns used to exclude directories
         from being scanned.\n
         `file_exclusion_patterns`An optional list of regular expression patterns used to exclude files
         from being scanned and registered.
-        
+
         Returns
         -------
         An instance of the concrete implementation for the `IUseCaseInvoker`.
-        
+
         '''
-        _UsecaseRegistry = construct_usecase_registry(usecase_scan_locations, directory_exclusion_patterns, file_exclusion_patterns)
+        self.register_pipe_services(usecase_scan_locations,
+                                    directory_exclusion_patterns,
+                                    file_exclusion_patterns)
+
+        _UsecaseRegistry = Engine.construct_usecase_registry(usecase_scan_locations,
+                                                             directory_exclusion_patterns,
+                                                             file_exclusion_patterns)
+
         self.register_service(providers.Singleton, PipelineFactory, IPipelineFactory, self, _UsecaseRegistry)
         self.register_service(providers.Factory, UseCaseInvoker, IUseCaseInvoker)
-        return self.get_service(IUseCaseInvoker)
-
 
-    def _generate_service_name(self, service: Type[TServiceType]) -> str:
+    def _try_generate_service_name(self, service: type) -> Tuple[str, bool]:
         '''
         Summary
         -------
         Generates a service name from a given service type by extracting the fully qualified
         name of the service, then replacing dots with underscores.
-        
+
         Parameters
         ----------
-        `service` The service to generate a name for.
+        `service` The service to generate a name for and true on success, otherwise empty string and false.
 
-        Exceptions
-        ----------
-        Raises a `ValueError` if the method fails to extract the fully qualified name of the service.
-        
         Returns
         -------
         The generated name of the service.
-        
+
         '''
         _TypeMatch = re.search(r"(?<=')[^']+(?=')", str(service))
 
         if not _TypeMatch:
-            raise ValueError(f"Could not generate name from fully qualified name of {service}.")
-
-        return _TypeMatch.group().replace('.', '_')
+            return "", False
 
+        return _TypeMatch.group().replace('.', '_'), True
 
-    def _has_service(self, service: Type[TServiceType]) -> bool:
+    def _has_service(self, service: type) -> bool:
         '''
         Summary
         -------
         Checks if a service exists in the dependency_injector container.
-        
+
         Parameters
         ----------
         `service` The service that is being checked for existence in the container.
 
         Returns
         -------
         True if the service could be found, false otherwise.
-        
+
         '''
-        try:
-            return hasattr(self._container, self._generate_service_name(service))
-        except:
-            pass
+        _ServiceName, _GenerationSuccess = self._try_generate_service_name(service)
+
+        if _GenerationSuccess:
+            return hasattr(self._container, _ServiceName)
+
+        return False
```

### Comparing `clapy-1.0.0/src/services.py` & `clapy-2.0.0/src/clapy/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,85 @@
 from abc import ABC, abstractmethod
 from typing import List, Type
 
-from generics import TInputPort, TOutputPort, TServiceType
-from pipeline import IPipe
+from .outputs import IOutputPort
+from .pipeline import IPipe, InputPort, PipeConfiguration
 
 
 class IPipelineFactory(ABC):
     '''Responsible for creating the pipeline for the use case invoker to execute.'''
 
     @abstractmethod
-    async def create_pipeline_async(self, input_port: TInputPort) -> List[Type[IPipe]]:
+    async def create_pipeline_async(
+            self,
+            input_port: InputPort,
+            pipeline_configuration: List[PipeConfiguration]) -> List[Type[IPipe]]:
         '''
         Summary
         -------
-        Creates a list of IPipe objects, sorted by priority, for a use case based on the input port provided.
-        
+        Creates a sorted list of IPipe objects based on the use case input port and pipeline
+        configuration provided.
+
         Parameters
         ----------
-        `input_port` The input port of the use case to construct the pipeline for
-        
+        `input_port` The input port of the use case to construct the pipeline for\n
+        `pipeline_configuration` The configuration used to determine order and inclusion of pipes
+
         Returns
         -------
         The pipeline consisting of the use case pipes ordered by their priority.
-        
+
         '''
         pass
 
 
 class IServiceProvider(ABC):
     '''A generic interface for getting services from a dependency injection container.'''
 
     @abstractmethod
-    def get_service(self, service: Type[TServiceType]) -> TServiceType:
+    def get_service(self, service: type) -> object:
         '''
         Summary
         -------
         Retrieves the specified service from the dependency_injectior container.
-        
+
         Parameters
         ----------
         `service` The service to be retrieved.
 
         Returns
         -------
         An instance of the requested service type with a lifetime as defined on the container.
-        
+
         '''
         pass
 
 
 class IUseCaseInvoker(ABC):
-    '''The main engine of Clapy. Handles the invocation of use case pipelines and the execution of resulting actions.'''
+    '''The main engine of Clapy. Handles the invocation of use case pipelines.'''
 
     @abstractmethod
-    async def can_invoke_usecase_async(self, input_port: TInputPort, output_port: TOutputPort) -> bool:
+    async def invoke_usecase_async(
+            self,
+            input_port: InputPort,
+            output_port: IOutputPort,
+            pipeline_configuration: List[PipeConfiguration]) -> bool:
         '''
         Summary
         -------
-        Checks if a use case can be successfully invoked based on provided input and output ports,
-        without performing the interactor execution. Useful for situations such as proactively disabling
-        a UI button based on whether or not a use case's interactor can be successfully invoked.
-        
+        Performs the invocation of a use case with the provided input and output ports. Will stop
+        the pipeline if the pipeline's pipes are exhausted, or on pipe failure unless configured to ignore.
+
         Parameters
         ----------
         `input_port` The input port of the use case to be invoked\n
-        `output_port` The output port of the use case to be invoked
-        
+        `output_port` The output port of the use case to be invoked\n
+        `pipeline_configuration` The configuration used to determine priority and inclusion of
+        use case pipes.
+
         Returns
         -------
-        `True` if all pipes were successfully invoked without error responses and the interactor was reached, otherwise `false`.
-        
-        '''
-        pass
+        True if pipes exhausted and no pipe failures occurred. Does not check failure override from
+        pipe configurations.
 
-    @abstractmethod
-    async def invoke_usecase_async(self, input_port: TInputPort, output_port: TOutputPort) -> None:
-        '''
-        Summary
-        -------
-        Performs the invocation of a use case with the provided input and output ports. Will stop
-        invocation on receival of a coroutine result, or if the pipeline's pipes are exhausted.
-        
-        Parameters
-        ----------
-        `input_port` The input port of the use case to be invoked\n
-        `output_port` The output port of the use case to be invoked
-        
         '''
         pass
```

