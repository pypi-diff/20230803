# Comparing `tmp/tkintertools-2.6.8.dev0.tar.gz` & `tmp/tkintertools-2.6.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.8.dev0.tar", last modified: Thu Jul 20 10:07:05 2023, max compression
+gzip compressed data, was "tkintertools-2.6.8.dev1.tar", last modified: Fri Jul 28 11:43:33 2023, max compression
```

## Comparing `tkintertools-2.6.8.dev0.tar` & `tkintertools-2.6.8.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.409236 tkintertools-2.6.8.dev0/
--rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.8.dev0/LICENSE.txt
--rw-rw-rw-   0        0        0     9305 2023-07-20 10:07:05.408236 tkintertools-2.6.8.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     8671 2023-07-20 10:05:47.000000 tkintertools-2.6.8.dev0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 10:07:05.409236 tkintertools-2.6.8.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-07-20 10:01:22.000000 tkintertools-2.6.8.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.390222 tkintertools-2.6.8.dev0/tkintertools/
--rw-rw-rw-   0        0        0     2237 2023-07-20 10:00:58.000000 tkintertools-2.6.8.dev0/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    67589 2023-07-20 09:49:55.000000 tkintertools-2.6.8.dev0/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2580 2023-07-20 07:07:46.000000 tkintertools-2.6.8.dev0/tkintertools/constants.py
--rw-rw-rw-   0        0        0    24186 2023-07-06 15:11:02.000000 tkintertools-2.6.8.dev0/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-07-20 10:07:05.405235 tkintertools-2.6.8.dev0/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     9305 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-20 10:07:05.000000 tkintertools-2.6.8.dev0/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.805291 tkintertools-2.6.8.dev1/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.8.dev1/LICENSE.txt
+-rw-rw-rw-   0        0        0     9451 2023-07-28 11:43:33.804288 tkintertools-2.6.8.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     8817 2023-07-28 11:41:26.000000 tkintertools-2.6.8.dev1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:43:33.806291 tkintertools-2.6.8.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-28 11:43:01.000000 tkintertools-2.6.8.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.763293 tkintertools-2.6.8.dev1/tkintertools/
+-rw-rw-rw-   0        0        0     2250 2023-07-28 11:42:30.000000 tkintertools-2.6.8.dev1/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    67848 2023-07-20 16:33:47.000000 tkintertools-2.6.8.dev1/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2580 2023-07-20 07:07:46.000000 tkintertools-2.6.8.dev1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    24186 2023-07-06 15:11:02.000000 tkintertools-2.6.8.dev1/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-07-28 11:43:33.802288 tkintertools-2.6.8.dev1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9451 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-28 11:43:33.000000 tkintertools-2.6.8.dev1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.8.dev0/LICENSE.txt` & `tkintertools-2.6.8.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.8.dev0/PKG-INFO` & `tkintertools-2.6.8.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.8.dev0
+Version: 2.6.8.dev1
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,15 +23,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/28-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -54,23 +54,23 @@
 
 ```
 pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/07/20 (UTC+08)
+* Version/最新版本 : `2.6.8.dev1` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/28 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.8.dev0
+pip install tkintertools==2.6.8.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -91,31 +91,33 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.8.dev0`**
+**最新版本: `tkintertools-v2.6.8.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev1`）的更新内容条目：
 
 - [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
 新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
 - [X] Added constant `CONTROL`  
 新增常量 `CONTROL`
 - [X] Modified the name of the constant `FRAMES` to `FPS`  
 修改常量 `FRAMES` 的名称为 `FPS`
 - [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
 函数 `move` 即将被弃用，请用新类 `Animation` 来代替
 - [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
 类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
+- [X] The class `Animation` adds the parameter `callback` to extend the functionality  
+类 `Animation` 新增参数 `callback` 来扩展功能
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

### Comparing `tkintertools-2.6.8.dev0/README.md` & `tkintertools-2.6.8.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/28-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -36,23 +36,23 @@
 
 ```
 pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/07/20 (UTC+08)
+* Version/最新版本 : `2.6.8.dev1` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/28 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.8.dev0
+pip install tkintertools==2.6.8.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -73,31 +73,33 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.8.dev0`**
+**最新版本: `tkintertools-v2.6.8.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev1`）的更新内容条目：
 
 - [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
 新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
 - [X] Added constant `CONTROL`  
 新增常量 `CONTROL`
 - [X] Modified the name of the constant `FRAMES` to `FPS`  
 修改常量 `FRAMES` 的名称为 `FPS`
 - [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
 函数 `move` 即将被弃用，请用新类 `Animation` 来代替
 - [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
 类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
+- [X] The class `Animation` adds the parameter `callback` to extend the functionality  
+类 `Animation` 新增参数 `callback` 来扩展功能
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

### Comparing `tkintertools-2.6.8.dev0/setup.py` & `tkintertools-2.6.8.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 9. 删除多余文件
 """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.8.dev0',
+    version='2.6.8.dev1',
     description='An auxiliary module of the tkinter module.',
     long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
     author_email='2951256653@qq.com',
     maintainer='Xiaokang2022',
     maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
```

### Comparing `tkintertools-2.6.8.dev0/tkintertools/__init__.py` & `tkintertools-2.6.8.dev1/tkintertools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 if sys.version_info < (3, 8):  # Version Check
     raise RuntimeError('Python version is too low (>=3.8)')
 
 from .__main__ import *
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.8.dev0'
+__version__ = '2.6.8.dev1'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
-    'PhotoImage', 'Singleton',
+    'PhotoImage', 'Singleton', 'Animation',
     # Tool Functions
     'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
 ] + all_constants
```

### Comparing `tkintertools-2.6.8.dev0/tkintertools/__main__.py` & `tkintertools-2.6.8.dev1/tkintertools/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1393,40 +1393,43 @@
         control=CONTROL,  # type: tuple[Callable[[float], float], float, float]
         translation=None,  # type: Iterable[float, float] | None
         color=None,  # type: tuple[Callable[[str], None], str, str] | None
         fps=FPS,  # type: int
         start=None,  # type: Callable | None
         step=None,  # type: Callable | None
         stop=None,  # type: Callable | None
+        callback=None,  # type: Callable[[float]] | None
         canvas=None  # type: tkinter.Canvas | None
     ):  # type: (...) -> None
         """
         `widget`: 进行动画的控件 \ 
         `ms`: 动画总时长（单位：毫秒） \ 
         `control`: 控制函数，为元组 (函数, 起始值, 终止值) 的形式 \ 
         `translation`: 平移运动 \ 
         `color`: 颜色变换 \ 
         `fps`: 每秒帧数 \ 
         `start`: 动画开始前执行的函数 \ 
         `step`: 动画每一帧结束后执行的函数（包括开始和结束）\ 
         `stop`: 动画结束后执行的函数 \ 
+        `callback`: 回调函数，每一帧调用一次，传入参数为单帧占比 \ 
         `canvas`: 当 widget 是画布中的绘制对象时，应指定 canvas
         """
         self.widget = widget
         self.master = canvas if isinstance(widget, int) else widget.master if isinstance(
             widget, tkinter.Widget) else widget
         self.start = start
         self.step = step
         self.stop = stop
         self.translation = translation
         self.color = color
         self.sec = 1000 // fps  # 单帧间隔时间
         self.count = ms * fps // 1000  # 总帧数
         if self.count == 0:
             self.count = 1  # 至少一帧
+        self.callback = callback
         self.parts = self._parts(*control)
 
     def _parts(self, control, up, down):
         # type: (Callable[[float], float], float, float) -> list[float]
         """ 部分比率 """
         key = (down - up) / self.count
         parts = [control(key * value) for value in range(1, self.count + 1)]
@@ -1442,14 +1445,15 @@
         if self.translation is not None:
             self._translate(*[value * self.parts[_ind]
                             for value in self.translation])
         if self.color is not None:
             self.color[0](color(self.color[1:], sum(self.parts[:_ind + 1])))
 
         None if self.step is None else self.step()
+        None if self.callback is None else self.callback(self.parts[_ind])
 
     def _translate(self, dx, dy):  # type: (int, int) -> None
         """ 平移 """
         if isinstance(self.widget, tkinter.Tk | tkinter.Toplevel):  # 窗口
             size, x, y = self.widget.geometry().split('+')
             self.widget.geometry('%s+%d+%d' % (size, int(x)+dx, int(y)+dy))
         elif isinstance(self.widget, tkinter.Widget):  # tkinter 控件
```

### Comparing `tkintertools-2.6.8.dev0/tkintertools/constants.py` & `tkintertools-2.6.8.dev1/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.8.dev0/tkintertools/tools_3d.py` & `tkintertools-2.6.8.dev1/tkintertools/tools_3d.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.8.dev0/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.8.dev1/tkintertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.8.dev0
+Version: 2.6.8.dev1
 Summary: An auxiliary module of the tkinter module.
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 Maintainer: Xiaokang2022
 Maintainer-email: 2951256653@qq.com
 License: MulanPSL-2.0
@@ -23,15 +23,15 @@
 <img src="tkt.png" style="height: 128px" alt="Logo" />
 
 `tkintertools` 模块是 `tkinter` 模块的一个辅助模块\
 The `tkintertools` module is an auxiliary module of the `tkinter` module
 
 [![Version](https://img.shields.io/pypi/v/tkintertools?label=Version)](.)
 [![License](https://img.shields.io/pypi/l/tkintertools?label=License)](LICENSE.txt)
-[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/20-orange)](CHANGELOG.md)
+[![ChangeLog](https://img.shields.io/badge/ChangeLog-2023/07/28-orange)](CHANGELOG.md)
 [![ToDo](https://img.shields.io/badge/ToDo-16-yellow)](TODO.md)
 [![Size](https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size)](tkintertools)
 [![Wiki](https://img.shields.io/badge/Wiki-14-purple)](https://github.com/Xiaokang2022/tkintertools/wiki)\
 [![Downloads](https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi)](https://pypistats.org/packages/tkintertools)
 [![Owner](https://img.shields.io/badge/Owner-Xiaokang2022-white)](https://github.com/Xiaokang2022)
 [![Blog](https://img.shields.io/badge/Blog-小康2022@CSDN-red)](https://xiaokang2022.blog.csdn.net)
 [![Email](https://img.shields.io/badge/Email-2951256653@qq.com-cyan)](mailto:2951256653@qq.com)
@@ -54,23 +54,23 @@
 
 ```
 pip install tkintertools==2.6.7
 ```
 
 ### Development Version/开发版本
 
-* Version/最新版本 : `2.6.8.dev0` (第 1 个预发布版本)
-* Release/发布日期 : 2023/07/20 (UTC+08)
+* Version/最新版本 : `2.6.8.dev1` (第 1 个预发布版本)
+* Release/发布日期 : 2023/07/28 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 可能会比较多，但也可能会比原来的版本更加稳定。开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 **PIP Cmd/安装命令：**
 
 ```
-pip install tkintertools==2.6.8.dev0
+pip install tkintertools==2.6.8.dev1
 ```
 
 > **Warning**  
 > 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！  
 > 若不指定具体的版本号，则会下载最新的稳定版本，也就是说，开发版本只能通过指定的版本号获取！
 
 ### Requirements/环境需求
@@ -91,31 +91,33 @@
 ![Python3.12.*](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 News/最新功能👇
 --------------
 
 ### Release Notes/版本说明
 
-**最新版本: `tkintertools-v2.6.8.dev0`**
+**最新版本: `tkintertools-v2.6.8.dev1`**
 
 > **Note**   
 > tkintertools 的介绍、使用教程和开发文档均在 [Wiki](https://github.com/Xiaokang2022/tkintertools/wiki) 中，大家可前往查阅
 
-下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev0`）的更新内容条目：
+下面是本次开发版本（`v2.6.7` -> `v2.6.8.dev1`）的更新内容条目：
 
 - [X] Added class `Animation` to achieve more efficient, convenient and functional animation effects  
 新增类 `Animation` 来实现更加高效、更加方便和功能性更强的动画效果
 - [X] Added constant `CONTROL`  
 新增常量 `CONTROL`
 - [X] Modified the name of the constant `FRAMES` to `FPS`  
 修改常量 `FRAMES` 的名称为 `FPS`
 - [X] The function `move` is about to be deprecated, please replace it with the new class `Animation`  
 函数 `move` 即将被弃用，请用新类 `Animation` 来代替
 - [X] The class `Singleton` is about to be deprecated and singleton mode classes will no longer be available in subsequent releases  
 类 `Singleton` 即将被弃用，后续版本中将不再提供单例模式类
+- [X] The class `Animation` adds the parameter `callback` to extend the functionality  
+类 `Animation` 新增参数 `callback` 来扩展功能
 
 ### Template Demo/模板演示
 
 下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
```

