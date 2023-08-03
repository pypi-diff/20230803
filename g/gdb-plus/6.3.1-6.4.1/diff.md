# Comparing `tmp/gdb_plus-6.3.1.tar.gz` & `tmp/gdb_plus-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.3.1.tar", last modified: Thu Jun  1 20:50:43 2023, max compression
+gzip compressed data, was "gdb_plus-6.4.1.tar", last modified: Thu Aug  3 07:45:27 2023, max compression
```

## Comparing `gdb_plus-6.3.1.tar` & `gdb_plus-6.4.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.824262 gdb_plus-6.3.1/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.3.1/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:50:43.823979 gdb_plus-6.3.1/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13367 2023-06-01 20:44:31.000000 gdb_plus-6.3.1/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.819652 gdb_plus-6.3.1/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    12472 2023-05-31 21:09:49.000000 gdb_plus-6.3.1/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-06-01 20:03:48.000000 gdb_plus-6.3.1/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    99855 2023-06-01 20:48:40.000000 gdb_plus-6.3.1/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    99228 2023-06-01 20:05:39.000000 gdb_plus-6.3.1/gdb_plus/gdb_plus_arm_dev.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     5125 2023-05-22 18:36:02.000000 gdb_plus-6.3.1/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.822570 gdb_plus-6.3.1/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      321 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      657 2023-06-01 20:50:24.000000 gdb_plus-6.3.1/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-06-01 20:50:43.824361 gdb_plus-6.3.1/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.823163 gdb_plus-6.3.1/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    20197 2023-06-01 16:55:57.000000 gdb_plus-6.3.1/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-08-03 07:45:27.374046 gdb_plus-6.4.1/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.4.1/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    15339 2023-08-03 07:45:27.373670 gdb_plus-6.4.1/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    14846 2023-07-28 18:33:33.000000 gdb_plus-6.4.1/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-08-03 07:45:27.352647 gdb_plus-6.4.1/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12741 2023-07-31 21:55:44.000000 gdb_plus-6.4.1/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      214 2023-08-03 07:44:52.000000 gdb_plus-6.4.1/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)   142868 2023-08-03 07:44:12.000000 gdb_plus-6.4.1/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13147 2023-07-28 20:17:41.000000 gdb_plus-6.4.1/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-08-03 07:45:27.371858 gdb_plus-6.4.1/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    15339 2023-08-03 07:45:27.000000 gdb_plus-6.4.1/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-08-03 07:45:27.000000 gdb_plus-6.4.1/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-08-03 07:45:27.000000 gdb_plus-6.4.1/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-08-03 07:45:27.000000 gdb_plus-6.4.1/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-08-03 07:45:27.000000 gdb_plus-6.4.1/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      631 2023-08-03 07:44:46.000000 gdb_plus-6.4.1/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-08-03 07:45:27.374184 gdb_plus-6.4.1/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-08-03 07:45:27.372564 gdb_plus-6.4.1/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    28424 2023-08-03 07:38:29.000000 gdb_plus-6.4.1/tests/test.py
```

### Comparing `gdb_plus-6.3.1/LICENSE` & `gdb_plus-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.1/PKG-INFO` & `gdb_plus-6.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.3.1
+Version: 6.4.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -80,15 +80,15 @@
 
 Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
 
 **Note**  
 Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
 
 **Warning**  
-Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
+Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped. Letting `from_start=True` may also cause problems if the environment variables are important to your exploit since they will be mixed with some set up by gdbserver.
 
 ## Control Flow
 
 The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
 
 ```py
 dbg.jump() # set instruction pointer to specific address
@@ -183,24 +183,44 @@
 dbg.cont(until="main+0x534")
 
 # Read the data set by the breakpoint
 print(pointer_to_secret.get())
 dbg.delete_breakpoint("main+0x124")
 ```
 
-## Memory access
-
-All registers are accessible as properties
+**Warning**
+You can script anything inside your callbacks, but be careful not to break the execution flow of your script. A putting a callback with `finish()` inside a function you are stepping over with `ni()` may cause problems. The alternative would be to set a second callback on the return_pointer of your function.  
 
 ```py
-dbg.rax = 0xdeadbeefdeadbeef
-dbg.eax = 0xfafafafa
-dbg.ax  = 0xbabe
-dbg.ah = 0x90
-assert dbg.rax == 0xdeadbeeffafa90be
+from gdb_plus import *
+from queue import Queue
+
+# I let the process run in this example to reinforce the need for the interrupt later
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
+
+# Does work, but you may lose control of your script if you try to step over a call to waitpid
+def dangerous_callback(dbg):
+    status = dbg.args[1]
+    dbg.finish()
+    log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+    return False
+
+def safe_callback(dbg):
+    status = dbg.args[1]
+    def second_callback(dbg):
+        log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+        return False
+    dbg.b(dbg.return_pointer, callback=second_callback, temporary=True)
+    return False
+
+dbg.b("waitpid", callback=safe_callback)
 ```
 
 You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
 
 ```py
 pointer = dbg.alloc(8)
 dbg.write(pointer, p64(0xdeadbeef))
@@ -290,20 +310,29 @@
 
 When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
 
 Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
 You can install it manually:
 `pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
 
-# TODO
+## AARCH64
+Arm binaries ar now partially supported. The problem running them in qemu is that we can't access the pid of the process from gdb and we can't catch when the process forks. This limits the feature we can use, but the rest is working fine.
 
+**Note**
+* set context.arch == "aarch64" at the beggining of your script
+* pwndbg may be better than GEF when using qemu. In particular if you find gdb always debugging qemu instead of your process and you are sure you set the correct context you may want to try switching to pwndbg for this part.
+
+# TODO
+* Distinguish between process running and dead
 * Identify actions performed manually in gdb (overwrite finish and ni)
-* Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
-    * register waitpid return value
-* Stack multiple callbacks on the same breakpoint
-* handle Hardware breakpoint
-* support ARM binaries
+    * handle waitpid(-1) with multiple slaves
+    * emulate waitid too
+* improve support ARM binaries
+    * how to specify libraries ? (-L /usr/aarch64-linux-gnu)
+    * features for native arch
+    * arm 32 bit
 * support multithread applications
-* setup gdbinit for forked processes
 * catch sigsegv as an exit instead of user interaction
 * enable signal() with libdebug
+* force parent or child to stop tracing
+* wrap follow-child
```

### Comparing `gdb_plus-6.3.1/README.md` & `gdb_plus-6.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,295 +1,324 @@
-# GDB+
-*Python library to automate gdb debugging* 
-
-GDB+ is a wrapper around gdb powered by pwntools. The goal is automate your interactions with gdb and add some extra features.
-
-## Main features
-
-* Include a python function as callback when you set a breakpoint.
-* Read the canary instead of bruteforcing it every time you need it while testing your exploit.
-* Test a specific function of a binary with the parameters you want at any time.
-* Log the code of a self modifying function.
-* Backup parts of your memory and restore it during future executions.
-* Don't waste time commenting your code. The arguments `NOPTRACE` and `REMOTE` make the exploit skip any action related to gdb.
-
-## Installation
-
-stable
-```
-pip3 install gdb_plus
-```
-or dev branch
-```
-pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
-```
-
-**Warning for pwndbg users:**  
-Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork, making it almost impossible to use features such as the emulation of ptrace.   
-you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
-
-## Debugging
-
-You can debug a program using the path to the binary.   
-If you really have to you can also use a process or even just his pid. 
-For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
-
-```py
-from gdb_plus import *
-
-gdbinit = """
-handle SIGALRM nopass
-"""
-
-dbg = Debugger("./rev_challenge", script=gdbinit, aslr=False)
-dbg = Debugger("./pwn_challenge", script=gdbinit).remote("10.10.0.1", 1337)
-
-
-p = process("./challenge", aslr=False)
-dbg = Debugger(p, script=gdbinit)
-
-#pidof process : 3134
-dbg = Debugger(3134, script=gdbinit, binary="./challenge")
-```
-
-By default your process will be analysed from the first instruction of the loader. If the process you are debugging has some checks you want to avoid use `Debugger(..., debug_from=<address>)` to attach with gdb at a specific address.  
-This will block you script until you reach you address. If you need to execute code in between you can use the non blocking alternative: 
-
-```py
-Im_done = Event()
-dbg = Debugger("./challenge").debug_from("main+0x34", event=Im_done)
-dbg.p.sendline("this is my input")
-Im_done.set()
-dbg.debug_from_done.wait()
-```
-
-This should pass any check for a debugger, even searches for INT3, exept a full check that the memory hasn't been edited.
-
-Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
-
-**Note**  
-Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
-
-**Warning**  
-Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
-
-## Control Flow
-
-The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
-
-```py
-dbg.jump() # set instruction pointer to specific address
-dbg.step() # Single instruction (will enter function calls)
-dbg.next() # Next instruction (will jump over function calls)
-dbg.cont() # Continue execution
-dbg.continue_until() # Continue until you reach a specific location
-dbg.finish() # Finish current function
-dbg.interrupt() # Stop the execution of your process
-dbg.wait() # Wait until you have control of gdb
-```
-
-In the cases where you have to interact with the process before reaching the address you want or if you would like to put some more breakpoints on the way to play manually with gdb you can use wait=False
-
-```py
-...
-dbg.breakpoint("main+0x12", temporary=True)
-dbg.breakpoint(0x23, temporary=True)
-done = dbg.continue_until("main+0x43", wait=False)
-dbg.p.recvline()
-dbg.p.sendline(b"4")
-done.wait()
-# Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
-...
-```
-
-**Warning**  
-* `finish` can only work if the stack frame hasn't been corrupted. With libdebug it will fail if the function doesn't use the base pointer.
-* Try avoiding `interrupt` as much as possible. 
-* You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
-
-If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
-
-```py
-def MyCallback(dbg):
-    if dbg.next_inst.mnemonic == "int3":
-        dbg.step()
-        dbg.signal("SIGINT")
-    print(dbg.next_inst.toString())
-
-dbg.step_until_ret(MyCallback)
-```
-
-In this example at each step the callback will be executed decrypting the next function chunk by chunk and logging the instructions. See [this example](./examples/debug_self_modifying_function.py) for more details solving a real challenge.
-
-You could also use `dbg.step_until_address(<address>, <callback=None>)` if you just want to execute a limited area of code or `dbg.step_until_condition(<check>)` if you are not sure where to stop.  
-
-## Breakpoints
-
-Breakpoints have three main features:
-* if the address is smaller than 0x10000 the address will immediately be interpreted as relative for PIE binaries
-* you can use a symbol name instead of an address such as `"main"` or `"main+0x12"`
-* you can set callbacks to be executed when the breakpoint is reach and may choose to let the process continue after the execution.
-
-The callback is a function that takes the debugger as parameter and returns a boolean to tell gdb if it should stop or not.
-The callbacks shouldn't be limited in what you can code. If you find problems raise an issue.
-If you want to pass data from your callback function to your exploit you can use pointers (lists, dictionaries or queues)
-
-**Note**  
-Setting a breakpoint requires the process to be interrupted.
-
-```py
-from gdb_plus import *
-from queue import Queue
-
-# I let the process run in this example to reinforce the need for the interrupt later
-gdbinit = """
-handle SIGALRM nopass
-"""
-
-dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
-pointer = Queue()
-
-# step over an hypothetical call to a function, overwrite the return value and save it in a queue
-def MyCallback(dbg):
-    dbg.next()
-    log.info(f"I tried to return {dbg.rax}")
-    pointer.put(dbg.rax)
-    dbg.rax = 0
-    # Return False to let the process run after executing the callback
-    return False
-
-def SecondCallback(dbg):
-    log.info("now you can play around with gdb")
-    log.info("once you are done execute continue in gdb and your script will resume once we reach main+0x534")
-    # Return True to interrupt the process
-    return True
-
-# You can not set a breakpoint while the process is running
-dbg.breakpoint("main+0x42", callback=MyCallback, temporary = True)
-dbg.breakpoint("main+0x124", callback=SecondCallback)
-dbg.cont(until="main+0x534")
-
-# Read the data set by the breakpoint
-print(pointer_to_secret.get())
-dbg.delete_breakpoint("main+0x124")
-```
-
-## Memory access
-
-All registers are accessible as properties
-
-```py
-dbg.rax = 0xdeadbeefdeadbeef
-dbg.eax = 0xfafafafa
-dbg.ax  = 0xbabe
-dbg.ah = 0x90
-assert dbg.rax == 0xdeadbeeffafa90be
-```
-
-You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
-
-```py
-pointer = dbg.alloc(8)
-dbg.write(pointer, p64(0xdeadbeef))
-secret = dbg.read(dbg.elf.symbols["secret"], 0x10)
-canary = dbg.canary
-```
-
-**Note**  
-While you can access the registers only when the process is at a stop, remember that you can read and write on the memory at any time
-
-Pwntools let you access the address where each library is loaded with `p.libs()[<path_to_library>]`
-We have two wrapper for the main ones:
-* `dbg.base_elf`
-* `dbg.base_libc`
-
-from gdb_plus >= 5.4.0 dbg.elf.address is already set to the correct address even with ASLR on, so you may need dbg.base_elf only if you debug a process for wich you don't have the binary
-
-We can also use capstone to know what is the next instruction that will be executed
-```py
-print(dbg.next_inst.toString()) # "mov rax, r12"
-print(dbg.next_inst.mnemonic)   # "mov"
-```
-
-## Fork
-You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`. The child will stop as soon as the process is created by fork, but will wait for the debugger to stop before creating the new object
-
-```py
-dbg = Debugger("http_server").set_split_on_fork()
-done = dbg.continue_until(0x40233)
-dbg.p.sendline("input")
-done.wait()
-# Now that the process stopped at address 0x40233 a new debugger will attach to the child
-pid_child = dbg.wait_split()
-
-# all children have their debugger saved in dbg.children and can be accessed by the pid
-child = dbg.children[pid_child]
-```
-
-If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
-
-```py
-child.emulate_ptrace_slave(dbg)
-dbg.emulate_ptrace_master(child)
-```
-
-This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them. To help you a bit we print "Slave can continue" every time the tracer tries to send a continue to the tracee
-
-**Warning**
-* If the tracee stopped with a SIGSTOP gdb may bug a bit and you may need `force=True` to make it continue correctly
-* pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
-* Handleling multiple processes in the same debugger instead of splitting them may cause problems whith the waits
-
-## Call functions
-
-If you want to test the effects of a specific function you can directly call it with the parameters you want
-
-```py
-pointer = dbg.alloc(100)
-# Initialize data
-dbg.write(pointer, bytes([i for i in range(100)]))
-dbg.call(dbg.p.symbols["obfuscated_pbox"], [pointer, "user_1", 1])
-dbg.read(pointer, 100)
-```
-
-See [this example](./examples/black_box_analysis_of_function.py) for more details
-
-**Note**  
-You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
-
-**Warning**  
-If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
-
-## Libdebug
-By default GDB+ uses a gdbserver to debug the process. This is verry usefull when you also have to check manually gdb while you are writing a script, but can be verry slow. For this reason we now support libdebug (from version >= 0.4) as an alternative debugger. It is lacking a lot of features but can do the job for most tasks and it can be 50 times faster. 
-
-The debugger will always start with dbg, but you can switch back and forth
-
-```py
-dbg = Debugger(<binary>)
-# switch to libdebug
-dbg.migrate(libdebug=True)
-# switch to gdb
-dbg.migrate(gdb=True)
-```
-
-To access properties of libdebug that haven't been wrapped you can simply use `dbg.libdebug` as you would with `dbg.gdb`.
-
-When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
-
-Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
-You can install it manually:
-`pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
-
-# TODO
-
-* Identify actions performed manually in gdb (overwrite finish and ni)
-* Handle fork and ptrace from syscall instead of libc
-* Improve ptrace emulation
-    * register waitpid return value
-* Stack multiple callbacks on the same breakpoint
-* handle Hardware breakpoint
-* support ARM binaries
-* support multithread applications
-* setup gdbinit for forked processes
-* catch sigsegv as an exit instead of user interaction
-* enable signal() with libdebug
+# GDB+
+*Python library to automate gdb debugging* 
+
+GDB+ is a wrapper around gdb powered by pwntools. The goal is automate your interactions with gdb and add some extra features.
+
+## Main features
+
+* Include a python function as callback when you set a breakpoint.
+* Read the canary instead of bruteforcing it every time you need it while testing your exploit.
+* Test a specific function of a binary with the parameters you want at any time.
+* Log the code of a self modifying function.
+* Backup parts of your memory and restore it during future executions.
+* Don't waste time commenting your code. The arguments `NOPTRACE` and `REMOTE` make the exploit skip any action related to gdb.
+
+## Installation
+
+stable
+```
+pip3 install gdb_plus
+```
+or dev branch
+```
+pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
+```
+
+**Warning for pwndbg users:**  
+Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork, making it almost impossible to use features such as the emulation of ptrace.   
+you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
+
+## Debugging
+
+You can debug a program using the path to the binary.   
+If you really have to you can also use a process or even just his pid. 
+For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
+
+```py
+from gdb_plus import *
+
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./rev_challenge", script=gdbinit, aslr=False)
+dbg = Debugger("./pwn_challenge", script=gdbinit).remote("10.10.0.1", 1337)
+
+
+p = process("./challenge", aslr=False)
+dbg = Debugger(p, script=gdbinit)
+
+#pidof process : 3134
+dbg = Debugger(3134, script=gdbinit, binary="./challenge")
+```
+
+By default your process will be analysed from the first instruction of the loader. If the process you are debugging has some checks you want to avoid use `Debugger(..., debug_from=<address>)` to attach with gdb at a specific address.  
+This will block you script until you reach you address. If you need to execute code in between you can use the non blocking alternative: 
+
+```py
+Im_done = Event()
+dbg = Debugger("./challenge").debug_from("main+0x34", event=Im_done)
+dbg.p.sendline("this is my input")
+Im_done.set()
+dbg.debug_from_done.wait()
+```
+
+This should pass any check for a debugger, even searches for INT3, exept a full check that the memory hasn't been edited.
+
+Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
+
+**Note**  
+Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
+
+**Warning**  
+Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped. Letting `from_start=True` may also cause problems if the environment variables are important to your exploit since they will be mixed with some set up by gdbserver.
+
+## Control Flow
+
+The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
+
+```py
+dbg.jump() # set instruction pointer to specific address
+dbg.step() # Single instruction (will enter function calls)
+dbg.next() # Next instruction (will jump over function calls)
+dbg.cont() # Continue execution
+dbg.continue_until() # Continue until you reach a specific location
+dbg.finish() # Finish current function
+dbg.interrupt() # Stop the execution of your process
+dbg.wait() # Wait until you have control of gdb
+```
+
+In the cases where you have to interact with the process before reaching the address you want or if you would like to put some more breakpoints on the way to play manually with gdb you can use wait=False
+
+```py
+...
+dbg.breakpoint("main+0x12", temporary=True)
+dbg.breakpoint(0x23, temporary=True)
+done = dbg.continue_until("main+0x43", wait=False)
+dbg.p.recvline()
+dbg.p.sendline(b"4")
+done.wait()
+# Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
+...
+```
+
+**Warning**  
+* `finish` can only work if the stack frame hasn't been corrupted. With libdebug it will fail if the function doesn't use the base pointer.
+* Try avoiding `interrupt` as much as possible. 
+* You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
+
+If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
+
+```py
+def MyCallback(dbg):
+    if dbg.next_inst.mnemonic == "int3":
+        dbg.step()
+        dbg.signal("SIGINT")
+    print(dbg.next_inst.toString())
+
+dbg.step_until_ret(MyCallback)
+```
+
+In this example at each step the callback will be executed decrypting the next function chunk by chunk and logging the instructions. See [this example](./examples/debug_self_modifying_function.py) for more details solving a real challenge.
+
+You could also use `dbg.step_until_address(<address>, <callback=None>)` if you just want to execute a limited area of code or `dbg.step_until_condition(<check>)` if you are not sure where to stop.  
+
+## Breakpoints
+
+Breakpoints have three main features:
+* if the address is smaller than 0x10000 the address will immediately be interpreted as relative for PIE binaries
+* you can use a symbol name instead of an address such as `"main"` or `"main+0x12"`
+* you can set callbacks to be executed when the breakpoint is reach and may choose to let the process continue after the execution.
+
+The callback is a function that takes the debugger as parameter and returns a boolean to tell gdb if it should stop or not.
+The callbacks shouldn't be limited in what you can code. If you find problems raise an issue.
+If you want to pass data from your callback function to your exploit you can use pointers (lists, dictionaries or queues)
+
+**Note**  
+Setting a breakpoint requires the process to be interrupted.
+
+```py
+from gdb_plus import *
+from queue import Queue
+
+# I let the process run in this example to reinforce the need for the interrupt later
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
+pointer = Queue()
+
+# step over an hypothetical call to a function, overwrite the return value and save it in a queue
+def MyCallback(dbg):
+    dbg.next()
+    log.info(f"I tried to return {dbg.rax}")
+    pointer.put(dbg.rax)
+    dbg.rax = 0
+    # Return False to let the process run after executing the callback
+    return False
+
+def SecondCallback(dbg):
+    log.info("now you can play around with gdb")
+    log.info("once you are done execute continue in gdb and your script will resume once we reach main+0x534")
+    # Return True to interrupt the process
+    return True
+
+# You can not set a breakpoint while the process is running
+dbg.breakpoint("main+0x42", callback=MyCallback, temporary = True)
+dbg.breakpoint("main+0x124", callback=SecondCallback)
+dbg.cont(until="main+0x534")
+
+# Read the data set by the breakpoint
+print(pointer_to_secret.get())
+dbg.delete_breakpoint("main+0x124")
+```
+
+**Warning**
+You can script anything inside your callbacks, but be careful not to break the execution flow of your script. A putting a callback with `finish()` inside a function you are stepping over with `ni()` may cause problems. The alternative would be to set a second callback on the return_pointer of your function.  
+
+```py
+from gdb_plus import *
+from queue import Queue
+
+# I let the process run in this example to reinforce the need for the interrupt later
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
+
+# Does work, but you may lose control of your script if you try to step over a call to waitpid
+def dangerous_callback(dbg):
+    status = dbg.args[1]
+    dbg.finish()
+    log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+    return False
+
+def safe_callback(dbg):
+    status = dbg.args[1]
+    def second_callback(dbg):
+        log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+        return False
+    dbg.b(dbg.return_pointer, callback=second_callback, temporary=True)
+    return False
+
+dbg.b("waitpid", callback=safe_callback)
+```
+
+You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
+
+```py
+pointer = dbg.alloc(8)
+dbg.write(pointer, p64(0xdeadbeef))
+secret = dbg.read(dbg.elf.symbols["secret"], 0x10)
+canary = dbg.canary
+```
+
+**Note**  
+While you can access the registers only when the process is at a stop, remember that you can read and write on the memory at any time
+
+Pwntools let you access the address where each library is loaded with `p.libs()[<path_to_library>]`
+We have two wrapper for the main ones:
+* `dbg.base_elf`
+* `dbg.base_libc`
+
+from gdb_plus >= 5.4.0 dbg.elf.address is already set to the correct address even with ASLR on, so you may need dbg.base_elf only if you debug a process for wich you don't have the binary
+
+We can also use capstone to know what is the next instruction that will be executed
+```py
+print(dbg.next_inst.toString()) # "mov rax, r12"
+print(dbg.next_inst.mnemonic)   # "mov"
+```
+
+## Fork
+You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`. The child will stop as soon as the process is created by fork, but will wait for the debugger to stop before creating the new object
+
+```py
+dbg = Debugger("http_server").set_split_on_fork()
+done = dbg.continue_until(0x40233)
+dbg.p.sendline("input")
+done.wait()
+# Now that the process stopped at address 0x40233 a new debugger will attach to the child
+pid_child = dbg.wait_split()
+
+# all children have their debugger saved in dbg.children and can be accessed by the pid
+child = dbg.children[pid_child]
+```
+
+If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
+
+```py
+child.emulate_ptrace_slave(dbg)
+dbg.emulate_ptrace_master(child)
+```
+
+This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them. To help you a bit we print "Slave can continue" every time the tracer tries to send a continue to the tracee
+
+**Warning**
+* If the tracee stopped with a SIGSTOP gdb may bug a bit and you may need `force=True` to make it continue correctly
+* pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* Handleling multiple processes in the same debugger instead of splitting them may cause problems whith the waits
+
+## Call functions
+
+If you want to test the effects of a specific function you can directly call it with the parameters you want
+
+```py
+pointer = dbg.alloc(100)
+# Initialize data
+dbg.write(pointer, bytes([i for i in range(100)]))
+dbg.call(dbg.p.symbols["obfuscated_pbox"], [pointer, "user_1", 1])
+dbg.read(pointer, 100)
+```
+
+See [this example](./examples/black_box_analysis_of_function.py) for more details
+
+**Note**  
+You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
+
+**Warning**  
+If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
+
+## Libdebug
+By default GDB+ uses a gdbserver to debug the process. This is verry usefull when you also have to check manually gdb while you are writing a script, but can be verry slow. For this reason we now support libdebug (from version >= 0.4) as an alternative debugger. It is lacking a lot of features but can do the job for most tasks and it can be 50 times faster. 
+
+The debugger will always start with dbg, but you can switch back and forth
+
+```py
+dbg = Debugger(<binary>)
+# switch to libdebug
+dbg.migrate(libdebug=True)
+# switch to gdb
+dbg.migrate(gdb=True)
+```
+
+To access properties of libdebug that haven't been wrapped you can simply use `dbg.libdebug` as you would with `dbg.gdb`.
+
+When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
+
+Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
+You can install it manually:
+`pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
+
+## AARCH64
+Arm binaries ar now partially supported. The problem running them in qemu is that we can't access the pid of the process from gdb and we can't catch when the process forks. This limits the feature we can use, but the rest is working fine.
+
+**Note**
+* set context.arch == "aarch64" at the beggining of your script
+* pwndbg may be better than GEF when using qemu. In particular if you find gdb always debugging qemu instead of your process and you are sure you set the correct context you may want to try switching to pwndbg for this part.
+
+# TODO
+* Distinguish between process running and dead
+* Identify actions performed manually in gdb (overwrite finish and ni)
+* Improve ptrace emulation
+    * handle waitpid(-1) with multiple slaves
+    * emulate waitid too
+* improve support ARM binaries
+    * how to specify libraries ? (-L /usr/aarch64-linux-gnu)
+    * features for native arch
+    * arm 32 bit
+* support multithread applications
+* catch sigsegv as an exit instead of user interaction
+* enable signal() with libdebug
+* force parent or child to stop tracing
+* wrap follow-child
```

### Comparing `gdb_plus-6.3.1/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.4.1/gdb_plus/Inner_Debugger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,324 +1,338 @@
-from gdb_plus import *
-from os import kill
-from time import sleep
-from functools import partial
-from capstone import Cs, CS_ARCH_X86
-from gdb_plus.utils import Inner_Breakpoint
-
-#import logging
-#log = logging.getLogger("gdb_plus-inner_debugger")
-
-INT3 = b"\xcc"
-constants.PTRACE_GETREGS = 0xc
-constants.PTRACE_SETREGS = 0xd
-
-# Only work if parent is tracing child (otherwise why would you need this class ?) and if the child is at a stop [02/03/23]
-class Inner_Debugger:
-    def __init__(self, dbg: Debugger, pid: int):
-        self.dbg = dbg
-        self.pid = pid
-        self._mem_file = None # instead of opening it every time
-        self.breakpoints = {}
-        # We can not cache the registers because we don't know if the child continues due to the parrent [31/05/23]
-        # We could change the ptrace emulation too, but for know we are going fast enough [31/05/23]
-        #self.__registers = None
-        self.__pointer_registers = None
-
-        self.dbg.restore_arch()
-
-    def get_regs(self):
-        registers = user_regs_struct()
-        if self.__pointer_registers is None:
-            self.__pointer_registers = self.dbg.alloc(registers.size)
-        res = self.dbg.call("ptrace", [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
-        assert res != 2**context.bits - 1
-        #self.dbg.syscall(constants.SYS_ptrace, [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
-        registers.set(self.dbg.read(self.__pointer_registers, registers.size))
-        return registers
-
-    def set_regs(self, registers):
-        self.dbg.write(self.__pointer_registers, registers.get())
-        self.dbg.call("ptrace", [constants.PTRACE_SETREGS, self.pid, 0, self.__pointer_registers])
-        return registers
-    
-    def read_memory(self, addr, size) -> bytes:
-        buffer = self.dbg.alloc(size)
-        self.dbg.syscall(constants.SYS_lseek.real, [self.mem_file, addr, constants.SEEK_SET.real])
-        self.dbg.syscall(constants.SYS_read.real, [self.mem_file, buffer, size])
-        data = self.dbg.read(buffer, size)
-        self.dbg.dealloc(buffer)
-        return data
-        
-    read = read_memory
-
-    # Maybe it's faster to write a single shellcode and execute that one
-    def write_memory(self, addr: int, data: bytes):
-        size = len(data)
-        buffer = self.dbg.alloc(size)
-        self.dbg.write(buffer, data)
-        self.dbg.syscall(constants.SYS_lseek, [self.mem_file, addr, constants.SEEK_SET])
-        self.dbg.syscall(constants.SYS_write, [self.mem_file, buffer, size])
-        self.dbg.dealloc(buffer)
-        
-    write = write_memory
-
-    # This part should be useless
-    #def peek(self, address: int, small = True) -> bytes:
-    #    log.debug(f"peeking {hex(address)}")
-    #    data = pack(self.dbg.call("ptrace", [constants.PTRACE_PEEKDATA, self.pid, address, 0]))
-    #    if not small:
-    #        data += pack(self.dbg.call("ptrace", [constants.PTRACE_PEEKDATA, self.pid, address+self.dbg.elf.bytes, 0]))
-    #    return data
-    #    
-    #def poke(self, address: int, data: bytes) -> None:
-    #    log.debug(f"poking {hex(address)} -> {data}")
-    #    pack(self.dbg.call("ptrace", [constants.PTRACE_POKEDATA, self.pid, address, unpack(data)]))
-        
-    def view_code(self, n=3) -> None:
-        ip = self.instruction_pointer
-        print("next instructions:")
-        data = self.read_memory(ip, 7*n)
-        for inst in self.capstone.disasm(data, ip):
-            print(f"{hex(inst.address)}: {inst.mnemonic} {inst.op_str}")
-
-    def view_stack(self, n=10) -> None:
-        # Sarebbe da fare _disable e _enable dei breakpoint per non averli in mezzo
-        sp = self.stack_pointer
-        data = self.read_memory(sp, n*context.bytes)
-        print("stack :")
-        for i in range(n):
-            print(f"{hex(sp)}: {hex(unpack(data[i*context.bytes:(i+1)*context.bytes]))}")
-            sp += context.bytes
-
-    # Per evitare chiamate ciclice provando a gestire i breakpoints
-    def _cont(self, wait = False):
-        self.dbg.call("ptrace", [constants.PTRACE_CONT, self.pid, 0, 0])
-        if wait:
-            self.wait()
-
-    # Please, never ever put two breakpoints next to each others as a user (using next is fine) [03/03/23] # Maybe not needed anymore
-    # Clear last_breakpoint ?
-    def cont(self, *, wait=False, until=None) -> None:
-        if until is not None:
-            log.warn_once("dbg.cont(until=ADDRESS) is deprecated, use dbg.continue_until(ADDRESS) instead!")  
-            self.continue_until(until)  
-        self.step()
-        # Wait, handle the case where breakpoints are temporary!! [26/05/23]
-        # This can't work with libdebug...
-        #if self._stop_reason != "SINGLE STEP":
-        #    if "BREAKPOINT" not in self._stop_reason:
-        #        if DEBUG:
-        #            log.warn(f"unknown interuption! {self._stop_reason}")
-        #    if DEBUG:
-        #        log.debug(f"step in continue already reached the breakpoint")
-        #    return
-        if self.instruction_pointer not in self.breakpoints: # Add last deleted breakpoint ?    
-            self._cont(wait)
-
-    c = cont
-
-    def continue_until(self, location, loop=False):
-        ip = self.instruction_pointer
-        address = self.dbg.parse_address(location)
-        if address == ip:
-            if not loop:
-                if DEBUG:
-                    log.debug(f"I'm already at {self.dbg.reverse_lookup(address)}")
-                    log.warn_once("Be careful that the default behaviour changed. Use loop=True if you want to continue anyway")
-            else:
-                self.step()
-        self.b(address, temporary=True)
-        self.cont(wait=True)
-        if address != self.instruction_pointer:
-            log.critical(f"couldn't reach address {hex(address)}. Stopped at address {hex(self.instruction_pointer)} instead")
-
-    until = continue_until
-
-    def interrupt(self) -> None:
-        # PTRACE_INTERRUPT may not work
-        #self.dbg.call(self.dbg.symbols["ptrace"], [constants.PTRACE_INTERRUPT.real, self.pid, 0, 0])
-        kill(self.pid, signal.SIGINT)
-        self.wait() # Necessario ? [03/03/23]
-
-    def _set_breakpoint(self, address, temporary=False):
-        self.breakpoints[address] = Inner_Breakpoint(b"", temporary)
-        self._restore_breakpoint(address)
-    
-    b = _set_breakpoint
-
-    breakpoint = b
-
-    def _restore_breakpoint(self, address):
-        if address in self.breakpoints:
-            byte = self.read_memory(address, 1)
-            if byte == 0xcc:
-                print("breakpoint already present")
-            self.breakpoints[address].byte = byte
-            self.write_memory(address, INT3)
-
-
-    def _disable_breakpoint(self, address):
-        if address in self.breakpoints:
-            self.write_memory(address, self.breakpoints[address].byte)
-    
-    def _disable_breakpoints(self):
-        for address, breakpoint in self.breakpoints.items():
-            self.write_memory(address, breakpoint.byte)
-
-    def _enable_breakpoints(self):
-        for address, breakpoint in self.breakpoints.items():
-            byte = self.read_memory(address, 1)
-            if byte != INT3:
-                breakpoint.byte = byte
-
-    def step(self):
-        constants.PTRACE_SINGLESTEP = 0x9
-        ip = self.instruction_pointer
-        self._disable_breakpoint(ip)
-        self.dbg.call("ptrace", [constants.PTRACE_SINGLESTEP, self.pid, 0, 0])
-        self.wait()
-        self._restore_breakpoint(ip)
-
-    def next(self):
-        ip = self.instruction_pointer
-        inst = self.next_inst
-        if inst.mnemonic == "call":
-            self._disable_breakpoint(ip)
-            self.until(ip + inst.size)
-            self._restore_breakpoint(ip)
-        else:
-            self.step()
-
-    def wait(self):
-        status_pointer = self.dbg.alloc(4)
-        self.dbg.call("waitpid", [self.pid, status_pointer, 0x40000000, 0])
-        
-        log.debug(f"wait finished with status: {hex(u32(self.dbg.read(status_pointer, 4)))}")
-        self.dbg.dealloc(status_pointer)
-        
-        # be carefull that INT3 is executed as an instruction! You have to back down if you did hit a breakpoint
-        ip = self.instruction_pointer - 1
-        breakpoint = self.breakpoints.get(ip)
-        
-        if breakpoint is None:
-            return
-
-        # What happens if I step over a breakpoint on an instruction of size 1 ?
-        self.instruction_pointer = ip
-
-        if breakpoint.temporary:
-            self._disable_breakpoint(ip)
-            del self.breakpoints[ip]
-
-    def detach(self):
-        self.dbg.call("ptrace", [constants.PTRACE_DETACH, self.pid, 0, 0])
-
-    @property
-    def next_inst(self):
-        ip = self.instruction_pointer # avoid calling it twice
-        inst = next(self.capstone.disasm(self.read_memory(ip, 16), ip))
-        inst.toString = partial(lambda self: f"{self.mnemonic} {self.op_str}".strip(), inst)
-        return inst
-
-    # Find a way to cache registers while you don't move [21/04/23] but be carefull if the parent uses SETREGS
-    @property
-    def registers(self):
-        return self.get_regs()
-
-    @registers.setter
-    def registers(self, registers: user_regs_struct):
-        self.set_regs(registers)
-
-    @property
-    def return_value(self):
-        if context.bits == 32:
-            return self.eax
-        else:
-            return self.rax
-
-    @return_value.setter
-    def return_value(self, value):
-        if context.bits == 32:
-            self.eax = value
-        else:
-            self.rax = value
-
-    @property
-    def stack_pointer(self):
-        if context.bits == 32:
-            return self.esp
-        else:
-            return self.rsp
-
-    # issue: setting $sp is not allowed when other stack frames are selected... https://sourceware.org/gdb/onlinedocs/gdb/Registers.html [04/03/23]
-    @stack_pointer.setter
-    def stack_pointer(self, value):
-        if context.bits == 32:
-            self.esp = value
-        else:
-            self.rsp = value
-
-    @property
-    def base_pointer(self):
-        if context.bits == 32:
-            return self.ebp
-        else:
-            return self.rbp
-    
-    @base_pointer.setter
-    def base_pointer(self, value):
-        if context.bits == 32:
-            self.ebp = value
-        else:
-            self.rbp = value
-
-    # Prevent null pointers
-    @property
-    def instruction_pointer(self):
-        if context.bits == 32:
-            ans = self.eip
-        else:
-            ans = self.rip
-        return ans
-
-    @instruction_pointer.setter
-    def instruction_pointer(self, value):
-        if context.bits == 32:
-            self.eip = value
-        else:
-            self.rip = value
-
-    @property
-    def capstone(self):
-        if self.dbg._capstone is None:
-            self.dbg._capstone = Cs(CS_ARCH_X86, context.bytes)
-        return self.dbg._capstone
-
-    @property
-    def mem_file(self):
-        if self._mem_file is None: # I wait to know how to move back and forth in the file [02/03/23] There are no problems, even if the data changes ! [03/03/23]
-            if "open" in self.dbg.symbols:
-                self._mem_file = self.dbg.call("open", [f"/proc/{self.pid}/mem".encode(), constants.O_RDWR])
-            else: 
-                self._mem_file = self.dbg.syscall(constants.SYS_open, [f"/proc/{self.pid}/mem".encode(), constants.O_RDWR])
-        return self._mem_file
-
-    def __getattr__(self, name):
-    
-        if name in ["dbg"]: #If __getattr__ is called with dbg it means I haven't finished initializing the class so I shouldn't call self.registers in __setattr__
-            return False
-        
-        if name in self.dbg.special_registers + self.dbg.registers:
-            return getattr(self.registers, name)
-
-        else:
-            # Get better errors when can't resolve properties
-            self.__getattribute__(name)
-
-    def __setattr__(self, name, value):
-        if self.dbg and name in self.dbg.special_registers + self.dbg.registers:
-            registers = self.registers
-            setattr(registers, name, value)
-            self.registers = registers
-        else:
+from gdb_plus import *
+from os import kill
+from time import sleep
+from functools import partial
+from capstone import Cs, CS_ARCH_X86
+from gdb_plus.utils import Inner_Breakpoint
+
+#import logging
+#log = logging.getLogger("gdb_plus-inner_debugger")
+
+INT3 = b"\xcc"
+constants.PTRACE_GETREGS = 0xc
+constants.PTRACE_SETREGS = 0xd
+
+# Only work if parent is tracing child (otherwise why would you need this class ?) and if the child is at a stop [02/03/23]
+# Only works for amd64 binaries.
+class Inner_Debugger:
+    def __init__(self, dbg: Debugger, pid: int):
+        self.dbg = dbg
+        self.pid = pid
+        self._mem_file = None # instead of opening it every time
+        self.breakpoints = {}
+        # We can not cache the registers because we don't know if the child continues due to the parrent [31/05/23]
+        # We could change the ptrace emulation too, but for know we are going fast enough [31/05/23]
+        #self.__registers = None
+        self.__pointer_registers = None
+        self._status_pointer = None #self.dbg.alloc(4)
+
+        self.dbg.restore_arch()
+
+        assert context.arch == "amd64", f"{context.arch} is not supported for Inner_Debugger"
+
+    def get_regs(self):
+        registers = user_regs_struct()
+        if self.__pointer_registers is None:
+            self.__pointer_registers = self.dbg.alloc(registers.size)
+        res = self.dbg.call("ptrace", [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
+        assert res != 2**context.bits - 1
+        #self.dbg.syscall(constants.SYS_ptrace, [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
+        registers.set(self.dbg.read(self.__pointer_registers, registers.size))
+        return registers
+
+    def set_regs(self, registers):
+        self.dbg.write(self.__pointer_registers, registers.get())
+        self.dbg.call("ptrace", [constants.PTRACE_SETREGS, self.pid, 0, self.__pointer_registers])
+        return registers
+    
+    def read_memory(self, address: int, size: int) -> bytes:
+        #buffer = self.dbg.alloc(size)
+        #self.dbg.syscall(constants.SYS_lseek.real, [self.mem_file, addr, constants.SEEK_SET.real])
+        #self.dbg.syscall(constants.SYS_read.real, [self.mem_file, buffer, size])
+        #data = self.dbg.read(buffer, size)
+        #self.dbg.dealloc(buffer)
+        #return data
+
+        with open(f"/proc/{self.pid}/mem", "r+b") as fd:
+            fd.seek(address)
+            return fd.read(size)
+        
+    read = read_memory
+
+    # Maybe it's faster to write a single shellcode and execute that one
+    def write_memory(self, address: int, data: bytes):
+        #size = len(data)
+        #buffer = self.dbg.alloc(size)
+        #self.dbg.write(buffer, data)
+        #self.dbg.syscall(constants.SYS_lseek, [self.mem_file, addr, constants.SEEK_SET])
+        #self.dbg.syscall(constants.SYS_write, [self.mem_file, buffer, size])
+        #self.dbg.dealloc(buffer)
+
+        with open(f"/proc/{self.pid}/mem", "r+b") as fd:
+            fd.seek(address)
+            fd.write(data)
+        
+    write = write_memory
+
+    # This part should be useless
+    #def peek(self, address: int, small = True) -> bytes:
+    #    log.debug(f"peeking {hex(address)}")
+    #    data = pack(self.dbg.call("ptrace", [constants.PTRACE_PEEKDATA, self.pid, address, 0]))
+    #    if not small:
+    #        data += pack(self.dbg.call("ptrace", [constants.PTRACE_PEEKDATA, self.pid, address+self.dbg.elf.bytes, 0]))
+    #    return data
+    #    
+    #def poke(self, address: int, data: bytes) -> None:
+    #    log.debug(f"poking {hex(address)} -> {data}")
+    #    pack(self.dbg.call("ptrace", [constants.PTRACE_POKEDATA, self.pid, address, unpack(data)]))
+        
+    def view_code(self, n=3) -> None:
+        ip = self.instruction_pointer
+        print("next instructions:")
+        data = self.read_memory(ip, 7*n)
+        for inst in self.capstone.disasm(data, ip):
+            print(f"{hex(inst.address)}: {inst.mnemonic} {inst.op_str}")
+
+    def view_stack(self, n=10) -> None:
+        # Sarebbe da fare _disable e _enable dei breakpoint per non averli in mezzo
+        sp = self.stack_pointer
+        data = self.read_memory(sp, n*context.bytes)
+        print("stack :")
+        for i in range(n):
+            print(f"{hex(sp)}: {hex(unpack(data[i*context.bytes:(i+1)*context.bytes]))}")
+            sp += context.bytes
+
+    # Per evitare chiamate ciclice provando a gestire i breakpoints
+    def _cont(self, wait = False):
+        self.dbg.call("ptrace", [constants.PTRACE_CONT, self.pid, 0, 0])
+        if wait:
+            self.wait()
+
+    # Please, never ever put two breakpoints next to each others as a user (using next is fine) [03/03/23] # Maybe not needed anymore
+    # Clear last_breakpoint ?
+    def cont(self, *, wait=False, until=None) -> None:
+        if until is not None:
+            log.warn_once("dbg.cont(until=ADDRESS) is deprecated, use dbg.continue_until(ADDRESS) instead!")  
+            self.continue_until(until)  
+        self.step()
+        # Wait, handle the case where breakpoints are temporary!! [26/05/23]
+        # This can't work with libdebug...
+        #if self._stop_reason != "SINGLE STEP":
+        #    if "BREAKPOINT" not in self._stop_reason:
+        #        if DEBUG:
+        #            log.warn(f"unknown interuption! {self._stop_reason}")
+        #    if DEBUG:
+        #        log.debug(f"step in continue already reached the breakpoint")
+        #    return
+        if self.instruction_pointer not in self.breakpoints: # Add last deleted breakpoint ?    
+            self._cont(wait)
+
+    c = cont
+
+    def continue_until(self, location, loop=False):
+        ip = self.instruction_pointer
+        address = self.dbg.parse_address(location)
+        if address == ip:
+            if not loop:
+                if DEBUG:
+                    log.debug(f"I'm already at {self.dbg.reverse_lookup(address)}")
+                    log.warn_once("Be careful that the default behaviour changed. Use loop=True if you want to continue anyway")
+            else:
+                self.step()
+        self.b(address, temporary=True)
+        self.cont(wait=True)
+        if address != self.instruction_pointer:
+            log.critical(f"couldn't reach address {hex(address)}. Stopped at address {hex(self.instruction_pointer)} instead")
+
+    until = continue_until
+
+    def interrupt(self) -> None:
+        # PTRACE_INTERRUPT may not work
+        #self.dbg.call(self.dbg.symbols["ptrace"], [constants.PTRACE_INTERRUPT.real, self.pid, 0, 0])
+        kill(self.pid, signal.SIGINT)
+        self.wait() # Necessario ? [03/03/23]
+
+    def _set_breakpoint(self, address, temporary=False):
+        self.breakpoints[address] = Inner_Breakpoint(b"", temporary)
+        self._restore_breakpoint(address)
+    
+    b = _set_breakpoint
+
+    breakpoint = b
+
+    def _restore_breakpoint(self, address):
+        if address in self.breakpoints:
+            byte = self.read_memory(address, 1)
+            if byte == 0xcc:
+                print("breakpoint already present")
+            self.breakpoints[address].byte = byte
+            self.write_memory(address, INT3)
+
+
+    def _disable_breakpoint(self, address):
+        if address in self.breakpoints:
+            self.write_memory(address, self.breakpoints[address].byte)
+    
+    def _disable_breakpoints(self):
+        for address, breakpoint in self.breakpoints.items():
+            self.write_memory(address, breakpoint.byte)
+
+    def _enable_breakpoints(self):
+        for address, breakpoint in self.breakpoints.items():
+            byte = self.read_memory(address, 1)
+            if byte != INT3:
+                breakpoint.byte = byte
+
+    def step(self):
+        constants.PTRACE_SINGLESTEP = 0x9
+        ip = self.instruction_pointer
+        self._disable_breakpoint(ip)
+        self.dbg.call("ptrace", [constants.PTRACE_SINGLESTEP, self.pid, 0, 0])
+        # For some reason any call with dbg will just step and wait indefinitely [31/07/23]
+        self.wait()
+        self._restore_breakpoint(ip)
+
+    def next(self):
+        ip = self.instruction_pointer
+        inst = self.next_inst
+        if inst.mnemonic == "call":
+            self._disable_breakpoint(ip)
+            self.until(ip + inst.size)
+            self._restore_breakpoint(ip)
+        else:
+            self.step()
+
+    def wait(self):
+        if self._status_pointer is None:
+            self.status_pointer = self.dbg.alloc(4)
+        status_pointer = self._status_pointer
+        self.dbg.call("waitpid", [self.pid, status_pointer, 0x40000000, 0])
+        
+        log.debug(f"wait finished with status: {hex(u32(self.dbg.read(status_pointer, 4)))}")
+        
+        # be carefull that INT3 is executed as an instruction! You have to back down if you did hit a breakpoint
+        ip = self.instruction_pointer - 1
+        breakpoint = self.breakpoints.get(ip)
+        
+        if breakpoint is None:
+            return
+
+        # What happens if I step over a breakpoint on an instruction of size 1 ?
+        self.instruction_pointer = ip
+
+        if breakpoint.temporary:
+            self._disable_breakpoint(ip)
+            del self.breakpoints[ip]
+
+    def detach(self):
+        self.dbg.call("ptrace", [constants.PTRACE_DETACH, self.pid, 0, 0])
+
+    @property
+    def next_inst(self):
+        ip = self.instruction_pointer # avoid calling it twice
+        inst = next(self.capstone.disasm(self.read_memory(ip, 16), ip))
+        inst.toString = partial(lambda self: f"{self.mnemonic} {self.op_str}".strip(), inst)
+        return inst
+
+    # Find a way to cache registers while you don't move [21/04/23] but be carefull if the parent uses SETREGS
+    @property
+    def registers(self):
+        return self.get_regs()
+
+    @registers.setter
+    def registers(self, registers: user_regs_struct):
+        self.set_regs(registers)
+
+    @property
+    def return_value(self):
+        if context.bits == 32:
+            return self.eax
+        else:
+            return self.rax
+
+    @return_value.setter
+    def return_value(self, value):
+        if context.bits == 32:
+            self.eax = value
+        else:
+            self.rax = value
+
+    @property
+    def stack_pointer(self):
+        if context.bits == 32:
+            return self.esp
+        else:
+            return self.rsp
+
+    # issue: setting $sp is not allowed when other stack frames are selected... https://sourceware.org/gdb/onlinedocs/gdb/Registers.html [04/03/23]
+    @stack_pointer.setter
+    def stack_pointer(self, value):
+        if context.bits == 32:
+            self.esp = value
+        else:
+            self.rsp = value
+
+    @property
+    def base_pointer(self):
+        if context.bits == 32:
+            return self.ebp
+        else:
+            return self.rbp
+    
+    @base_pointer.setter
+    def base_pointer(self, value):
+        if context.bits == 32:
+            self.ebp = value
+        else:
+            self.rbp = value
+
+    # Prevent null pointers
+    @property
+    def instruction_pointer(self):
+        if context.bits == 32:
+            ans = self.eip
+        else:
+            ans = self.rip
+        return ans
+
+    @instruction_pointer.setter
+    def instruction_pointer(self, value):
+        if context.bits == 32:
+            self.eip = value
+        else:
+            self.rip = value
+
+    @property
+    def capstone(self):
+        if self.dbg._capstone is None:
+            self.dbg._capstone = Cs(CS_ARCH_X86, context.bytes)
+        return self.dbg._capstone
+
+    @property
+    def mem_file(self):
+        if self._mem_file is None: # I wait to know how to move back and forth in the file [02/03/23] There are no problems, even if the data changes ! [03/03/23]
+            if "open" in self.dbg.symbols:
+                self._mem_file = self.dbg.call("open", [f"/proc/{self.pid}/mem".encode(), constants.O_RDWR])
+            else: 
+                self._mem_file = self.dbg.syscall(constants.SYS_open, [f"/proc/{self.pid}/mem".encode(), constants.O_RDWR])
+        return self._mem_file
+
+    def __getattr__(self, name):
+    
+        if name in ["dbg"]: #If __getattr__ is called with dbg it means I haven't finished initializing the class so I shouldn't call self.registers in __setattr__
+            return False
+        
+        if name in self.dbg.special_registers + self.dbg.registers:
+            return getattr(self.registers, name)
+
+        else:
+            # Get better errors when can't resolve properties
+            self.__getattribute__(name)
+
+    def __setattr__(self, name, value):
+        if self.dbg and name in self.dbg.special_registers + self.dbg.registers:
+            registers = self.registers
+            setattr(registers, name, value)
+            self.registers = registers
+        else:
             super().__setattr__(name, value)
```

### Comparing `gdb_plus-6.3.1/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.4.1/gdb_plus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.3.1
+Version: 6.4.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -80,15 +80,15 @@
 
 Calling your script with pwntools arguments `NOPTRACE` or `REMOTE` will allow you to disable all actions related to gdb and test your exploit localy or attack the remote target without having to comment anything. If you want a finer control you can use `ìf dbg.debugging` to discriminate the code that should be executed when gdb is opened or not.
 
 **Note**  
 Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
 
 **Warning**  
-Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
+Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped. Letting `from_start=True` may also cause problems if the environment variables are important to your exploit since they will be mixed with some set up by gdbserver.
 
 ## Control Flow
 
 The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
 
 ```py
 dbg.jump() # set instruction pointer to specific address
@@ -183,24 +183,44 @@
 dbg.cont(until="main+0x534")
 
 # Read the data set by the breakpoint
 print(pointer_to_secret.get())
 dbg.delete_breakpoint("main+0x124")
 ```
 
-## Memory access
-
-All registers are accessible as properties
+**Warning**
+You can script anything inside your callbacks, but be careful not to break the execution flow of your script. A putting a callback with `finish()` inside a function you are stepping over with `ni()` may cause problems. The alternative would be to set a second callback on the return_pointer of your function.  
 
 ```py
-dbg.rax = 0xdeadbeefdeadbeef
-dbg.eax = 0xfafafafa
-dbg.ax  = 0xbabe
-dbg.ah = 0x90
-assert dbg.rax == 0xdeadbeeffafa90be
+from gdb_plus import *
+from queue import Queue
+
+# I let the process run in this example to reinforce the need for the interrupt later
+gdbinit = """
+handle SIGALRM nopass
+"""
+
+dbg = Debugger("./challenge", script=gdbinit).remote("leet.pwn.com", 31337)
+
+# Does work, but you may lose control of your script if you try to step over a call to waitpid
+def dangerous_callback(dbg):
+    status = dbg.args[1]
+    dbg.finish()
+    log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+    return False
+
+def safe_callback(dbg):
+    status = dbg.args[1]
+    def second_callback(dbg):
+        log.info(f"Child stopped with status : {hex(u32(dbg.read(status, 4)))}")
+        return False
+    dbg.b(dbg.return_pointer, callback=second_callback, temporary=True)
+    return False
+
+dbg.b("waitpid", callback=safe_callback)
 ```
 
 You can allocate chunks on the heap (or the bss if you don't have the libc), write and read in the ram and read the canary from anywhere.
 
 ```py
 pointer = dbg.alloc(8)
 dbg.write(pointer, p64(0xdeadbeef))
@@ -290,20 +310,29 @@
 
 When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
 
 Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
 You can install it manually:
 `pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
 
-# TODO
+## AARCH64
+Arm binaries ar now partially supported. The problem running them in qemu is that we can't access the pid of the process from gdb and we can't catch when the process forks. This limits the feature we can use, but the rest is working fine.
 
+**Note**
+* set context.arch == "aarch64" at the beggining of your script
+* pwndbg may be better than GEF when using qemu. In particular if you find gdb always debugging qemu instead of your process and you are sure you set the correct context you may want to try switching to pwndbg for this part.
+
+# TODO
+* Distinguish between process running and dead
 * Identify actions performed manually in gdb (overwrite finish and ni)
-* Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
-    * register waitpid return value
-* Stack multiple callbacks on the same breakpoint
-* handle Hardware breakpoint
-* support ARM binaries
+    * handle waitpid(-1) with multiple slaves
+    * emulate waitid too
+* improve support ARM binaries
+    * how to specify libraries ? (-L /usr/aarch64-linux-gnu)
+    * features for native arch
+    * arm 32 bit
 * support multithread applications
-* setup gdbinit for forked processes
 * catch sigsegv as an exit instead of user interaction
 * enable signal() with libdebug
+* force parent or child to stop tracing
+* wrap follow-child
```

