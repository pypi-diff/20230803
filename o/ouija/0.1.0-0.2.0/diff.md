# Comparing `tmp/ouija-0.1.0.tar.gz` & `tmp/ouija-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ouija-0.1.0.tar", last modified: Sun Jul 30 01:01:50 2023, max compression
+gzip compressed data, was "ouija-0.2.0.tar", last modified: Thu Aug  3 18:02:00 2023, max compression
```

## Comparing `ouija-0.1.0.tar` & `ouija-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-07-30 01:01:50.864427 ouija-0.1.0/
--rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-0.1.0/LICENSE
--rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-0.1.0/MANIFEST.in
--rw-r--r--   0 embali     (501) staff       (20)     1541 2023-07-30 01:01:50.863732 ouija-0.1.0/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)     1043 2023-07-30 00:28:41.000000 ouija-0.1.0/README.rst
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-07-30 01:01:50.854990 ouija-0.1.0/ouija/
--rw-r--r--   0 embali     (501) staff       (20)      172 2023-07-30 00:14:53.000000 ouija-0.1.0/ouija/__init__.py
--rw-r--r--   0 embali     (501) staff       (20)     3080 2023-07-30 00:18:10.000000 ouija-0.1.0/ouija/interface.py
--rw-r--r--   0 embali     (501) staff       (20)     8665 2023-07-30 00:18:26.000000 ouija-0.1.0/ouija/link.py
--rw-r--r--   0 embali     (501) staff       (20)     1374 2023-07-29 23:39:45.000000 ouija-0.1.0/ouija/packet.py
--rw-r--r--   0 embali     (501) staff       (20)      311 2023-07-29 23:39:45.000000 ouija-0.1.0/ouija/primitives.py
--rw-r--r--   0 embali     (501) staff       (20)     2226 2023-07-30 00:18:46.000000 ouija-0.1.0/ouija/proxy.py
--rw-r--r--   0 embali     (501) staff       (20)     9602 2023-07-30 00:18:53.000000 ouija-0.1.0/ouija/relay.py
--rw-r--r--   0 embali     (501) staff       (20)     1249 2023-07-29 23:39:45.000000 ouija-0.1.0/ouija/telemetry.py
--rw-r--r--   0 embali     (501) staff       (20)      638 2023-07-29 23:39:45.000000 ouija-0.1.0/ouija/tuning.py
--rw-r--r--   0 embali     (501) staff       (20)     1127 2023-07-29 23:39:45.000000 ouija-0.1.0/ouija/utils.py
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-07-30 01:01:50.862797 ouija-0.1.0/ouija.egg-info/
--rw-r--r--   0 embali     (501) staff       (20)     1541 2023-07-30 01:01:50.000000 ouija-0.1.0/ouija.egg-info/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)      350 2023-07-30 01:01:50.000000 ouija-0.1.0/ouija.egg-info/SOURCES.txt
--rw-r--r--   0 embali     (501) staff       (20)        1 2023-07-30 01:01:50.000000 ouija-0.1.0/ouija.egg-info/dependency_links.txt
--rw-r--r--   0 embali     (501) staff       (20)       36 2023-07-30 01:01:50.000000 ouija-0.1.0/ouija.egg-info/requires.txt
--rw-r--r--   0 embali     (501) staff       (20)        6 2023-07-30 01:01:50.000000 ouija-0.1.0/ouija.egg-info/top_level.txt
--rw-r--r--   0 embali     (501) staff       (20)       38 2023-07-30 01:01:50.864740 ouija-0.1.0/setup.cfg
--rw-r--r--   0 embali     (501) staff       (20)      875 2023-07-30 00:28:36.000000 ouija-0.1.0/setup.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.804327 ouija-0.2.0/
+-rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-0.2.0/LICENSE
+-rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-0.2.0/MANIFEST.in
+-rw-r--r--   0 embali     (501) staff       (20)     1723 2023-08-03 18:02:00.803565 ouija-0.2.0/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)     1225 2023-08-03 17:58:40.000000 ouija-0.2.0/README.rst
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.798403 ouija-0.2.0/ouija/
+-rw-r--r--   0 embali     (501) staff       (20)      376 2023-08-03 17:15:57.000000 ouija-0.2.0/ouija/__init__.py
+-rw-r--r--   0 embali     (501) staff       (20)     2955 2023-08-03 17:34:25.000000 ouija-0.2.0/ouija/interface.py
+-rw-r--r--   0 embali     (501) staff       (20)     1864 2023-08-03 17:34:34.000000 ouija-0.2.0/ouija/link.py
+-rw-r--r--   0 embali     (501) staff       (20)     9311 2023-08-03 17:34:10.000000 ouija-0.2.0/ouija/ouija.py
+-rw-r--r--   0 embali     (501) staff       (20)     1815 2023-08-03 17:36:30.000000 ouija-0.2.0/ouija/packet.py
+-rw-r--r--   0 embali     (501) staff       (20)      367 2023-08-03 17:18:48.000000 ouija-0.2.0/ouija/primitives.py
+-rw-r--r--   0 embali     (501) staff       (20)     2287 2023-08-03 17:36:40.000000 ouija-0.2.0/ouija/proxy.py
+-rw-r--r--   0 embali     (501) staff       (20)     2882 2023-08-03 17:36:51.000000 ouija-0.2.0/ouija/relay.py
+-rw-r--r--   0 embali     (501) staff       (20)     1475 2023-08-03 14:13:25.000000 ouija-0.2.0/ouija/telemetry.py
+-rw-r--r--   0 embali     (501) staff       (20)      910 2023-08-03 17:27:40.000000 ouija-0.2.0/ouija/tuning.py
+-rw-r--r--   0 embali     (501) staff       (20)     1127 2023-07-29 23:39:45.000000 ouija-0.2.0/ouija/utils.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.802664 ouija-0.2.0/ouija.egg-info/
+-rw-r--r--   0 embali     (501) staff       (20)     1723 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)      365 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/SOURCES.txt
+-rw-r--r--   0 embali     (501) staff       (20)        1 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/dependency_links.txt
+-rw-r--r--   0 embali     (501) staff       (20)       36 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/requires.txt
+-rw-r--r--   0 embali     (501) staff       (20)        6 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/top_level.txt
+-rw-r--r--   0 embali     (501) staff       (20)       38 2023-08-03 18:02:00.804546 ouija-0.2.0/setup.cfg
+-rw-r--r--   0 embali     (501) staff       (20)      875 2023-08-03 17:22:34.000000 ouija-0.2.0/setup.py
```

### Comparing `ouija-0.1.0/LICENSE` & `ouija-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ouija-0.1.0/PKG-INFO` & `ouija-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ouija
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for building and accessing UDP-relayed TCP proxies
 Home-page: https://github.com/neurophant/ouija/
 Author: Anton Smolin
 Author-email: smolin.anton@gmail.com
 License: MIT
 Keywords: async https tcp udp proxy relay
 Classifier: Development Status :: 3 - Alpha
@@ -17,30 +17,33 @@
 =====
 
 Python library for building and accessing UDP-relayed TCP proxies
 
 Features
 --------
 
-Objects:
+Classes:
 
-* Interface - basic HTTPS proxy server
 * Tuning - Relay-Proxy settings
+* Interface - basic HTTPS proxy server
 * Relay - HTTPS proxy interface, which communicates with Proxy via encrypted UDP
+* Link - Relay link within Proxy
 * Proxy - UDP server, which gets requests from Relay and sends back responses from target TCP servers
 
 Tuning:
 
 * fernet - Fernet instance with provided secret key - use Fernet.generate_key()
 * token - your secret token - UUID4 or anything else
-* serving - timeout per worker
-* timeout - TCP stream/UDP awaiting timeout
-* payload - UDP payload size
-* retries - UDP max retry count per interaction
-* capacity - UDP read/write buffer capacity
+* serving_timeout - total timeout per worker, seconds
+* tcp_buffer - TCP buffer size, bytes
+* tcp_timeout - TCP awaiting timeout, seconds
+* udp_payload - UDP payload size, bytes
+* udp_timeout - UDP awaiting timeout, seconds
+* udp_retries - UDP max retry count per interaction
+* udp_capacity - UDP send/receive buffer capacity - max packet count
 
 Requirements
 ------------
 
 * Python 3.11+
 * pbjson 1.18.0+
 * cryptography 41.0.2+
```

### Comparing `ouija-0.1.0/README.rst` & `ouija-0.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 =====
 
 Python library for building and accessing UDP-relayed TCP proxies
 
 Features
 --------
 
-Objects:
+Classes:
 
-* Interface - basic HTTPS proxy server
 * Tuning - Relay-Proxy settings
+* Interface - basic HTTPS proxy server
 * Relay - HTTPS proxy interface, which communicates with Proxy via encrypted UDP
+* Link - Relay link within Proxy
 * Proxy - UDP server, which gets requests from Relay and sends back responses from target TCP servers
 
 Tuning:
 
 * fernet - Fernet instance with provided secret key - use Fernet.generate_key()
 * token - your secret token - UUID4 or anything else
-* serving - timeout per worker
-* timeout - TCP stream/UDP awaiting timeout
-* payload - UDP payload size
-* retries - UDP max retry count per interaction
-* capacity - UDP read/write buffer capacity
+* serving_timeout - total timeout per worker, seconds
+* tcp_buffer - TCP buffer size, bytes
+* tcp_timeout - TCP awaiting timeout, seconds
+* udp_payload - UDP payload size, bytes
+* udp_timeout - UDP awaiting timeout, seconds
+* udp_retries - UDP max retry count per interaction
+* udp_capacity - UDP send/receive buffer capacity - max packet count
 
 Requirements
 ------------
 
 * Python 3.11+
 * pbjson 1.18.0+
 * cryptography 41.0.2+
```

### Comparing `ouija-0.1.0/ouija/interface.py` & `ouija-0.2.0/ouija/interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,94 @@
 import asyncio
 import logging
 import os
-from contextlib import closing
 from typing import Dict
 
 from .tuning import Tuning
 from .relay import Relay
 from .telemetry import Telemetry
 from .utils import RawParser
 
 
-logging.basicConfig()
+logging.basicConfig(
+    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
+    datefmt='%Y-%m-%d:%H:%M:%S',
+    level=logging.ERROR,
+)
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.ERROR)
 
 
 class Interface:
     telemetry: Telemetry
     __tuning: Tuning
     __proxy_host: str
     __proxy_port: int
     __index: int
     __sessions: Dict[int, asyncio.Task]
 
     def __init__(self, *, telemetry: Telemetry, tuning: Tuning, proxy_host: str, proxy_port: int) -> None:
         self.telemetry = telemetry
-        self.__tuning = tuning
-        self.__proxy_host = proxy_host
-        self.__proxy_port = proxy_port
-        self.__index = 0
-        self.__sessions = dict()
+        self.tuning = tuning
+        self.proxy_host = proxy_host
+        self.proxy_port = proxy_port
+        self.index = 0
+        self.sessions = dict()
 
-    async def __https_handler(
+    async def https_handler(
             self,
             *,
             reader: asyncio.StreamReader,
             writer: asyncio.StreamWriter,
             remote_host: str,
             remote_port: int,
     ) -> None:
         relay = Relay(
             telemetry=self.telemetry,
-            tuning=self.__tuning,
+            tuning=self.tuning,
             reader=reader,
             writer=writer,
-            proxy_host=self.__proxy_host,
-            proxy_port=self.__proxy_port,
+            proxy_host=self.proxy_host,
+            proxy_port=self.proxy_port,
             remote_host=remote_host,
             remote_port=remote_port,
         )
-        await relay.stream()
-
-    async def __session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
-        with closing(writer):
-            data = await reader.readuntil(b'\r\n\r\n')
-            addr = writer.get_extra_info('peername')
-
-            request = RawParser(data=data)
-
-            if request.error:
-                logger.error('Parse error')
-            elif request.method == 'CONNECT':  # https
-                await self.__https_handler(
-                    reader=reader,
-                    writer=writer,
-                    remote_host=request.host,
-                    remote_port=request.port,
-                )
-            else:
-                logger.error(f'{request.method} method is not supported')
+        await relay.serve()
 
     async def _session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+        data = await reader.readuntil(b'\r\n\r\n')
+        request = RawParser(data=data)
+
+        if request.error:
+            logger.error('Parse error')
+        elif request.method == 'CONNECT':
+            await self.https_handler(
+                reader=reader,
+                writer=writer,
+                remote_host=request.host,
+                remote_port=request.port,
+            )
+        else:
+            logger.error(f'{request.method} method is not supported')
+
+    async def session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         try:
-            await asyncio.wait_for(self.__session(reader=reader, writer=writer), self.__tuning.serving)
+            await asyncio.wait_for(self._session(reader=reader, writer=writer), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
             logger.error('Timeout')
 
     async def serve(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
-        loop = asyncio.get_event_loop()
-        self.__sessions[self.__index] = loop.create_task(self._session(reader=reader, writer=writer))
-        self.__index += 1
+        self.sessions[self.index] = asyncio.create_task(self._session(reader=reader, writer=writer))
+        self.index += 1
 
     async def cleanup(self) -> None:
         while True:
             await asyncio.sleep(1)
-            for index in sorted(self.__sessions.keys()):
-                if self.__sessions[index].done():
-                    self.__sessions.pop(index)
-            self.telemetry.links = len(self.__sessions)
+            for index in sorted(self.sessions.keys()):
+                if self.sessions[index].done():
+                    self.sessions.pop(index)
+            self.telemetry.links = len(self.sessions)
 
     async def monitor(self) -> None:
         while True:
             await asyncio.sleep(1)
             os.system('clear')
             print(self.telemetry)
```

### Comparing `ouija-0.1.0/ouija/link.py` & `ouija-0.2.0/ouija/ouija.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,232 +1,289 @@
 import asyncio
-import time
-from typing import Dict, Tuple, Optional
 import logging
+import time
+from typing import Optional, Dict
 
-from .packet import Packet, PacketType
-from .primitives import Sent, Received
 from .telemetry import Telemetry
 from .tuning import Tuning
-
-from typing import TYPE_CHECKING
-if TYPE_CHECKING:
-    from proxy import Proxy
+from .primitives import Sent, Received
+from .packet import Phase, Packet
 
 
-logging.basicConfig()
+logging.basicConfig(
+    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
+    datefmt='%Y-%m-%d:%H:%M:%S',
+    level=logging.ERROR,
+)
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.ERROR)
 
 
-class Link:
+class Ouija:
     telemetry: Telemetry
-    __proxy: 'Proxy'
-    __addr: Tuple[str, int]
-    __tuning: Tuning
-    __reader: Optional[asyncio.StreamReader]
-    __writer: Optional[asyncio.StreamWriter]
-    __remote_host: Optional[str]
-    __remote_port: Optional[int]
-    __connected: asyncio.Event
-    __sent_buf: Dict[int, Sent]
-    __sent_seq: int
-    __recv_buf: Dict[int, Received]
-    __recv_seq: int
-    __stream_task: Optional[asyncio.Task]
-    __finish_task: Optional[asyncio.Task]
-    __disconnected: asyncio.Event
-
-    def __init__(self,  *, telemetry: Telemetry,  proxy: 'Proxy', addr: Tuple[str, int], tuning: Tuning) -> None:
-        self.telemetry = telemetry
-        self.__proxy = proxy
-        self.__addr = addr
-        self.__tuning = tuning
-        self.__reader = None
-        self.__writer = None
-        self.__remote_host = None
-        self.__remote_port = None
-        self.__connected = asyncio.Event()
-        self.__sent_buf = dict()
-        self.__sent_seq = 0
-        self.__recv_buf = dict()
-        self.__recv_seq = 0
-        self.__stream_task = None
-        self.__finish_task = None
-        self.__disconnected = asyncio.Event()
+    tuning: Tuning
+    reader: Optional[asyncio.StreamReader]
+    writer: Optional[asyncio.StreamWriter]
+    remote_host: Optional[str]
+    remote_port: Optional[int]
+    opened: asyncio.Event
+    sent_buf: Dict[int, Sent]
+    sent_seq: int
+    read_closed: asyncio.Event
+    recv_buf: Dict[int, Received]
+    recv_seq: int
+    write_closed: asyncio.Event
+
+    async def sendto(self, *, data: bytes) -> None:
+        raise NotImplementedError
+
+    async def send(self, *, data: bytes) -> None:
+        await self.sendto(data=data)
 
-    async def __sendto(self, *, data: bytes) -> None:
-        self.__proxy.transport.sendto(data, self.__addr)
         self.telemetry.packets_sent += 1
         self.telemetry.bytes_sent += len(data)
+        if len(data) > self.telemetry.max_packet_size:
+            self.telemetry.max_packet_size = len(data)
 
-    async def __sendto_retry(self, *, data: bytes, event: asyncio.Event) -> bool:
-        for _ in range(0, self.__tuning.retries):
-            await self.__sendto(data=data)
+    async def send_retry(self, *, data: bytes, event: asyncio.Event) -> bool:
+        for _ in range(self.tuning.udp_retries):
+            await self.send(data=data)
             try:
-                await asyncio.wait_for(event.wait(), self.__tuning.timeout)
+                await asyncio.wait_for(event.wait(), self.tuning.udp_timeout)
             except asyncio.TimeoutError:
+                self.telemetry.resent += 1
                 continue
             else:
                 return True
         else:
             return False
 
-    async def __process(self, *, packet: Packet) -> None:
-        if packet.token != self.__tuning.token:
-            await self.__stop()
-            self.telemetry.token_errors += 1
-            return
+    async def read(self) -> bytes:
+        return await self.reader.read(self.tuning.tcp_buffer)
 
-        match packet.packet_type:
-            case PacketType.CONNECT:
-                if not self.__connected.is_set():
-                    self.__remote_host = packet.host
-                    self.__remote_port = packet.port
-
-                    self.__reader, self.__writer = await asyncio.open_connection(self.__remote_host, self.__remote_port)
-                    self.__connected.set()
-                    self.__proxy.links[self.__addr] = self
-                    loop = asyncio.get_event_loop()
-                    self.__stream_task = loop.create_task(self._stream())
-                    self.__finish_task = loop.create_task(self._finish())
-
-                connect_ack_packet = Packet(
-                    token=self.__tuning.token,
-                    packet_type=PacketType.CONNECT,
-                    ack=True,
-                    data=b'HTTP/1.1 200 Connection Established\r\n\r\n',
-                )
-                await self.__sendto(data=await connect_ack_packet.binary(fernet=self.__tuning.fernet))
-                self.telemetry.connections += 1
-            case PacketType.DATA:
-                if not self.__connected.is_set():
-                    await self.__stop()
+    async def write(self, *, data: bytes, drain: bool) -> None:
+        self.writer.write(data)
+        if drain:
+            await self.writer.drain()
+
+    async def recv(self, *, seq: int, data: bytes, drain: bool) -> None:
+        if seq >= self.recv_seq:
+            self.recv_buf[seq] = Received(data=data, drain=drain)
+
+        for seq in sorted(self.recv_buf.keys()):
+            if seq < self.recv_seq:
+                self.recv_buf.pop(seq)
+            if seq == self.recv_seq:
+                recv = self.recv_buf.pop(seq)
+                await self.write(data=recv.data, drain=recv.drain)
+                self.recv_seq += 1
+
+        await self.send_ack_data(seq=seq)
+
+        if len(self.recv_buf) >= self.tuning.udp_capacity:
+            await self.close()
+            self.telemetry.recv_buf_overloads += 1
+
+    async def enqueue_send(self, *, data: bytes, drain: bool) -> None:
+        data_packet = Packet(
+            phase=Phase.DATA,
+            ack=False,
+            seq=self.sent_seq,
+            data=data,
+            drain=drain,
+        )
+        data_ = await data_packet.binary(fernet=self.tuning.fernet)
+        self.sent_buf[self.sent_seq] = Sent(data=data_)
+        await self.send(data=data_)
+        self.sent_seq += 1
+
+        if len(self.sent_buf) >= self.tuning.udp_capacity:
+            await self.close()
+            self.telemetry.sent_buf_overloads += 1
+
+    async def dequeue_send(self, *, seq: int) -> None:
+        self.sent_buf.pop(seq, None)
+
+    async def send_open(self) -> bool:
+        open_packet = Packet(
+            phase=Phase.OPEN,
+            ack=False,
+            token=self.tuning.token,
+            host=self.remote_host,
+            port=self.remote_port,
+        )
+        if not await self.send_retry(
+                data=await open_packet.binary(fernet=self.tuning.fernet),
+                event=self.opened,
+        ):
+            return False
+
+        return True
+
+    async def send_ack_open(self) -> None:
+        open_ack_packet = Packet(
+            phase=Phase.OPEN,
+            ack=True,
+            token=self.tuning.token,
+        )
+        await self.send(data=await open_ack_packet.binary(fernet=self.tuning.fernet))
+
+    async def check_token(self, *, token: str) -> bool:
+        if token == self.tuning.token:
+            return True
+
+        await self.close()
+        self.telemetry.token_errors += 1
+        return False
+
+    async def send_ack_data(self, *, seq: int) -> None:
+        data_ack_packet = Packet(
+            phase=Phase.DATA,
+            ack=True,
+            seq=seq,
+        )
+        await self.send(data=await data_ack_packet.binary(fernet=self.tuning.fernet))
+
+    async def send_close(self) -> None:
+        close_packet = Packet(
+            phase=Phase.CLOSE,
+            ack=False,
+        )
+        await self.send_retry(
+            data=await close_packet.binary(fernet=self.tuning.fernet),
+            event=self.read_closed,
+        )
+
+    async def send_ack_close(self) -> None:
+        close_ack_packet = Packet(
+            phase=Phase.CLOSE,
+            ack=True,
+        )
+        await self.send(data=await close_ack_packet.binary(fernet=self.tuning.fernet))
+
+    async def on_open(self, packet: Packet) -> bool:
+        raise NotImplementedError
+
+    async def process_packet(self, *, packet: Packet) -> None:
+        match packet.phase:
+            case Phase.OPEN:
+                if not await self.check_token(token=packet.token):
+                    return
+
+                if not await self.on_open(packet=packet):
+                    return
+
+                self.telemetry.opened += 1
+            case Phase.DATA:
+                if not self.opened.is_set() or self.write_closed.is_set():
                     return
 
                 if packet.ack:
-                    self.__sent_buf.pop(packet.seq, None)
+                    await self.dequeue_send(seq=packet.seq)
                 else:
-                    if packet.seq >= self.__recv_seq:
-                        self.__recv_buf[packet.seq] = Received(data=packet.data)
-
-                    for seq in sorted(self.__recv_buf.keys()):
-                        if seq < self.__recv_seq:
-                            self.__recv_buf.pop(seq)
-                        if seq == self.__recv_seq:
-                            self.__writer.write(self.__recv_buf.pop(seq).data)
-                            self.__recv_seq += 1
-                        await self.__writer.drain()
-
-                    if len(self.__recv_buf) >= self.__tuning.capacity:
-                        await self.__stop()
-                        self.telemetry.recv_buf_overloads += 1
-                        return
-
-                    data_ack_packet = Packet(
-                        token=self.__tuning.token,
-                        packet_type=PacketType.DATA,
-                        ack=True,
-                        seq=packet.seq,
-                    )
-                    await self.__sendto(data=await data_ack_packet.binary(fernet=self.__tuning.fernet))
-            case PacketType.DISCONNECT:
-                await self.__stop()
-                if not packet.ack:
-                    disconnect_ack_packet = Packet(
-                        token=self.__tuning.token,
-                        packet_type=PacketType.DISCONNECT,
-                        ack=True,
-                    )
-                    await self.__sendto(data=await disconnect_ack_packet.binary(fernet=self.__tuning.fernet))
-                self.__disconnected.set()
+                    await self.recv(seq=packet.seq, data=packet.data, drain=packet.drain)
+            case Phase.CLOSE:
+                if packet.ack:
+                    self.read_closed.set()
+                else:
+                    await self.send_ack_close()
+                    self.write_closed.set()
             case _:
-                await self.__stop()
                 self.telemetry.type_errors += 1
 
     async def process(self, *, packet: Packet) -> None:
         try:
-            await self.__process(packet=packet)
+            await self.process_packet(packet=packet)
+        except ConnectionError as e:
+            logger.error(e)
+            self.telemetry.connection_errors += 1
         except Exception as e:
-            await self.__stop()
+            await self.close()
             logger.error(e)
             self.telemetry.processing_errors += 1
 
-    async def __finish(self) -> None:
-        while self.__connected.is_set() or self.__sent_buf:
-            await asyncio.sleep(self.__tuning.timeout)
-            for seq in sorted(self.__sent_buf.keys()):
-                delta = int(time.time()) - self.__sent_buf[seq].timestamp
-                if delta >= self.__tuning.timeout:
-                    await self.__sendto(data=self.__sent_buf[seq].data)
-                    self.__sent_buf[seq].retries += 1
-                if delta >= self.__tuning.serving or self.__sent_buf[seq].retries >= self.__tuning.retries:
-                    self.__sent_buf.pop(seq, None)
-
-        disconnect_packet = Packet(
-            token=self.__tuning.token,
-            packet_type=PacketType.DISCONNECT,
-            ack=False,
-        )
-        await self.__sendto_retry(
-            data=await disconnect_packet.binary(fernet=self.__tuning.fernet),
-            event=self.__disconnected,
-        )
+    async def resend_packets(self) -> None:
+        while self.opened.is_set() or self.sent_buf:
+            await asyncio.sleep(self.tuning.udp_timeout)
+
+            for seq in sorted(self.sent_buf.keys()):
+                delta = int(time.time()) - self.sent_buf[seq].timestamp
+
+                if delta >= self.tuning.serving_timeout or self.sent_buf[seq].retries >= self.tuning.udp_retries:
+                    await self.close()
+                    self.telemetry.unfinished += 1
+                    break
+
+                if delta >= self.tuning.udp_timeout:
+                    await self.send(data=self.sent_buf[seq].data)
+                    self.sent_buf[seq].retries += 1
+                    self.telemetry.resent += 1
+
+        await self.send_close()
 
-    async def _finish(self) -> None:
         try:
-            await asyncio.wait_for(self.__finish(), self.__tuning.serving)
+            await asyncio.wait_for(self.write_closed.wait(), self.tuning.serving_timeout)
+        except asyncio.TimeoutError:
+            pass
+
+    async def resend(self) -> None:
+        try:
+            await asyncio.wait_for(self.resend_packets(), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
             self.telemetry.timeout_errors += 1
         except Exception as e:
             logger.error(e)
-            self.telemetry.finishing_errors += 1
+            self.telemetry.resending_errors += 1
         finally:
-            await self.__stop()
-            await self.__close()
+            await self.close()
+
+    async def on_serve(self) -> bool:
+        raise NotImplementedError
+
+    async def serve_stream(self) -> None:
+        if not await self.on_serve():
+            return
 
-    async def __stream(self) -> None:
-        while self.__connected.is_set():
+        asyncio.create_task(self.resend())
+
+        while self.opened.is_set():
             try:
-                data = await asyncio.wait_for(self.__reader.read(self.__tuning.payload), self.__tuning.timeout)
-            except asyncio.TimeoutError:
+                data = await asyncio.wait_for(self.read(), self.tuning.tcp_timeout)
+            except TimeoutError:
                 continue
 
-            if data == b'':
+            if not data:
                 break
 
-            data_packet = Packet(
-                token=self.__tuning.token,
-                packet_type=PacketType.DATA,
-                ack=False,
-                seq=self.__sent_seq,
-                data=data,
-            )
-            binary = await data_packet.binary(fernet=self.__tuning.fernet)
-            self.__sent_buf[self.__sent_seq] = Sent(data=binary)
-            await self.__sendto(data=binary)
-            self.__sent_seq += 1
-
-            if len(self.__sent_buf) >= self.__tuning.capacity:
-                await self.__stop()
-                self.telemetry.sent_buf_overloads += 1
-                break
+            for idx in range(0, len(data), self.tuning.udp_payload):
+                await self.enqueue_send(
+                    data=data[idx:idx + self.tuning.udp_payload],
+                    drain=True if len(data) - idx <= self.tuning.udp_payload else False,
+                )
 
-    async def _stream(self) -> None:
+    async def serve(self) -> None:
         try:
-            await asyncio.wait_for(self.__stream(), self.__tuning.serving)
+            await asyncio.wait_for(self.serve_stream(), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
             self.telemetry.timeout_errors += 1
+        except ConnectionError as e:
+            logger.error(e)
+            self.telemetry.connection_errors += 1
         except Exception as e:
             logger.error(e)
-            self.telemetry.streaming_errors += 1
+            self.telemetry.serving_errors += 1
+
+    async def on_close(self) -> None:
+        raise NotImplementedError
+
+    async def close(self) -> None:
+        if self.opened.is_set():
+            self.telemetry.closed += 1
+
+        self.opened.clear()
+        self.read_closed.set()
+        self.write_closed.set()
+
+        if isinstance(self.writer, asyncio.StreamWriter) and not self.writer.is_closing():
+            self.writer.close()
+            await self.writer.wait_closed()
 
-    async def __stop(self) -> None:
-        self.__connected.clear()
-        if isinstance(self.__writer, asyncio.StreamWriter) and not self.__writer.is_closing():
-            self.__writer.close()
-            await self.__writer.wait_closed()
-
-    async def __close(self) -> None:
-        self.__disconnected.set()
-        self.__proxy.links.pop(self.__addr, None)
-        self.telemetry.disconnections += 1
+        await self.on_close()
```

### Comparing `ouija-0.1.0/ouija/proxy.py` & `ouija-0.2.0/ouija/proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,64 +5,66 @@
 
 from .packet import Packet
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .link import Link
 
 
-logging.basicConfig()
+logging.basicConfig(
+    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
+    datefmt='%Y-%m-%d:%H:%M:%S',
+    level=logging.ERROR,
+)
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.ERROR)
 
 
 class Proxy(asyncio.DatagramProtocol):
     transport: asyncio.DatagramTransport
     telemetry: Telemetry
     links: Dict[Tuple[str, int], Link]
-    __tuning: Tuning
-    __proxy_host: str
-    __proxy_port: int
+    tuning: Tuning
+    proxy_host: str
+    proxy_port: int
 
     def __init__(self, *, telemetry: Telemetry, tuning: Tuning, proxy_host: str, proxy_port: int) -> None:
         self.links = dict()
         self.telemetry = telemetry
-        self.__tuning = tuning
-        self.__proxy_host = proxy_host
-        self.__proxy_port = proxy_port
+        self.tuning = tuning
+        self.proxy_host = proxy_host
+        self.proxy_port = proxy_port
 
     def connection_made(self, transport) -> None:
         self.transport = transport
 
-    def datagram_received(self, data, addr) -> None:
-        loop = asyncio.get_event_loop()
-        loop.create_task(self.__datagram_received_async(data=data, addr=addr))
-
-    def error_received(self, exc) -> None:
-        logger.error(exc)
-
-    def connection_lost(self, exc) -> None:
-        self.transport.close()
-        logger.error(exc)
-
-    async def __datagram_received_async(self, *, data, addr) -> None:
+    async def _datagram_received_async(self, *, data, addr) -> None:
         self.telemetry.packets_received += 1
         self.telemetry.bytes_received += len(data)
         try:
-            packet = await Packet.packet(data=data, fernet=self.__tuning.fernet)
+            packet = await Packet.packet(data=data, fernet=self.tuning.fernet)
         except Exception as e:
             logger.error(e)
             self.telemetry.decoding_errors += 1
             return
 
-        link = self.links.get(addr, Link(telemetry=self.telemetry, proxy=self, addr=addr, tuning=self.__tuning))
+        link = self.links.get(addr, Link(telemetry=self.telemetry, proxy=self, addr=addr, tuning=self.tuning))
         await link.process(packet=packet)
 
+    def datagram_received(self, data, addr) -> None:
+        asyncio.create_task(self._datagram_received_async(data=data, addr=addr))
+
+    def error_received(self, exc) -> None:
+        logger.error(exc)
+
+    def connection_lost(self, exc) -> None:
+        self.transport.close()
+        logger.error(exc)
+
     async def serve(self) -> None:
         loop = asyncio.get_event_loop()
-        await loop.create_datagram_endpoint(lambda: self, local_addr=(self.__proxy_host, self.__proxy_port))
+        await loop.create_datagram_endpoint(lambda: self, local_addr=(self.proxy_host, self.proxy_port))
 
     async def cleanup(self) -> None:
         while True:
             await asyncio.sleep(1)
             self.telemetry.links = len(self.links)
 
     async def monitor(self) -> None:
```

### Comparing `ouija-0.1.0/ouija/utils.py` & `ouija-0.2.0/ouija/utils.py`

 * *Files identical despite different names*

### Comparing `ouija-0.1.0/ouija.egg-info/PKG-INFO` & `ouija-0.2.0/ouija.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ouija
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for building and accessing UDP-relayed TCP proxies
 Home-page: https://github.com/neurophant/ouija/
 Author: Anton Smolin
 Author-email: smolin.anton@gmail.com
 License: MIT
 Keywords: async https tcp udp proxy relay
 Classifier: Development Status :: 3 - Alpha
@@ -17,30 +17,33 @@
 =====
 
 Python library for building and accessing UDP-relayed TCP proxies
 
 Features
 --------
 
-Objects:
+Classes:
 
-* Interface - basic HTTPS proxy server
 * Tuning - Relay-Proxy settings
+* Interface - basic HTTPS proxy server
 * Relay - HTTPS proxy interface, which communicates with Proxy via encrypted UDP
+* Link - Relay link within Proxy
 * Proxy - UDP server, which gets requests from Relay and sends back responses from target TCP servers
 
 Tuning:
 
 * fernet - Fernet instance with provided secret key - use Fernet.generate_key()
 * token - your secret token - UUID4 or anything else
-* serving - timeout per worker
-* timeout - TCP stream/UDP awaiting timeout
-* payload - UDP payload size
-* retries - UDP max retry count per interaction
-* capacity - UDP read/write buffer capacity
+* serving_timeout - total timeout per worker, seconds
+* tcp_buffer - TCP buffer size, bytes
+* tcp_timeout - TCP awaiting timeout, seconds
+* udp_payload - UDP payload size, bytes
+* udp_timeout - UDP awaiting timeout, seconds
+* udp_retries - UDP max retry count per interaction
+* udp_capacity - UDP send/receive buffer capacity - max packet count
 
 Requirements
 ------------
 
 * Python 3.11+
 * pbjson 1.18.0+
 * cryptography 41.0.2+
```

### Comparing `ouija-0.1.0/setup.py` & `ouija-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ouija',
-    version='0.1.0',
+    version='0.2.0',
     description='Python library for building and accessing UDP-relayed TCP proxies',
     long_description=long_description,
     url='https://github.com/neurophant/ouija/',
     author='Anton Smolin',
     author_email='smolin.anton@gmail.com',
     license='MIT',
     classifiers=[
```

