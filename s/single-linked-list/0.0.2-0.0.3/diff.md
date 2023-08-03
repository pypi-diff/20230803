# Comparing `tmp/single-linked-list-0.0.2.tar.gz` & `tmp/single-linked-list-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "single-linked-list-0.0.2.tar", last modified: Wed Jul  5 19:15:26 2023, max compression
+gzip compressed data, was "single-linked-list-0.0.3.tar", last modified: Thu Aug  3 00:15:56 2023, max compression
```

## Comparing `single-linked-list-0.0.2.tar` & `single-linked-list-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:15:26.211504 single-linked-list-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-05 19:15:26.211504 single-linked-list-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-05 19:15:16.000000 single-linked-list-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:15:26.211504 single-linked-list-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-05 19:15:16.000000 single-linked-list-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:15:26.211504 single-linked-list-0.0.2/single_linked_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-05 19:15:26.000000 single-linked-list-0.0.2/single_linked_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 19:15:26.000000 single-linked-list-0.0.2/single_linked_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:15:26.000000 single-linked-list-0.0.2/single_linked_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-05 19:15:26.000000 single-linked-list-0.0.2/single_linked_list.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:15:26.211504 single-linked-list-0.0.2/slll/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:15:16.000000 single-linked-list-0.0.2/slll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-05 19:15:16.000000 single-linked-list-0.0.2/slll/slll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/single_linked_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-08-03 00:15:56.000000 single-linked-list-0.0.3/single_linked_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-03 00:15:56.000000 single-linked-list-0.0.3/single_linked_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:15:56.000000 single-linked-list-0.0.3/single_linked_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 00:15:56.000000 single-linked-list-0.0.3/single_linked_list.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/slll/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/slll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/slll/csll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/slll/slll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:15:56.786174 single-linked-list-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/test/test_csll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-03 00:15:46.000000 single-linked-list-0.0.3/test/test_sll.py
```

### Comparing `single-linked-list-0.0.2/README.md` & `single-linked-list-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,175 +9,190 @@
 This is a Python implementation of a singly linked list.
 
 ## Installation
 
 Install the `SingleLinkedList` package from PyPI using `pip`:
 
 ```bash
-pip install single-linked-list==0.0.1
+pip install single-linked-list==0.0.3
 ````
 
-then, import the `SingleLinkedList` class
+then, import the `SingleLinkedList` class or `CicruleSingeLinkedList`
 
 ```python
 from slll.slll import SingleLinkedList
+from slll.csll import CicruleSingeLinkedList
 ```
 
 Initialize a Singly Linked List
 
 ```python
 single_linked_list = SingleLinkedList()
+cicrule_single_list = CicruleSingeLinkedList()
 ```
 
 ## Methods
 
 ### * Append 
 - inserts a new node at the end of the linked list.
 
 #### Method: 
 - append(data)
 
 `data(any)` : The data to be stored in the new node.
 ```python
 single_linked_list.append(1)
 single_linked_list.append(2)
+cicrule_single_list.append(1)
+cicrule_single_list.append(2)
 ```
 
 ### * Preappend
 - inserts a new node at the beginning of the linked list.
 
 #### Method: 
-- preappend(data)
+- pre_append(data)
 
 `data(any)` : The data to be stored in the new node.
 
 ```python
-single_linked_list.preappend(0)
+single_linked_list.pre_append(0)
+cicrule_single_list.pre_append(0)
 ```
 
 ### * Insert
 - inserts a new node at the specified index in the linked list.
 
 #### Method: 
-- insert(index, data)
+- insert(data, index)
 
 `index(int)` : The index where the new node should be inserted.
 `data(any)` : The data to be stored in the new node.
 
 ```python
 single_linked_list.insert(2, 3)
+cicrule_single_list.insert(2, 3)
 ```
 
 ### * Find
 - returns the index of the first node containing the specified data.
 
 #### Method: 
 - find(data)
 
 `data(any)`: The data to search for.
 
 ```python
 index = single_linked_list.find(2)
+index = cicrule_single_list.find(2)
 print(index)  # Output: 1
 ```
 
 ### * Get
 - returns the node at the specified index.
 
 #### Method: 
 - get(index)
 
 `index(int)` : The index of the desired node.
 
 ```python
 node = single_linked_list.get(2)
+node = cicrule_single_list.get(2)
 print(node.data)  # Output: 3
 ```
 
 ### * Set
 - updates the data of the node at the specified index.
 
 #### Method: 
 - set(index, data)
 
 `index(int)` : The index of the node to be updated.
 `data(any)` : The new data to be stored in the node.
 
 ```python
 single_linked_list.set(0, 9000)
+cicrule_single_list.set(0, 9000)
 ```
 
 ### * Pop
 - removes and returns the last node in the linked list.
 
 #### Method: 
 - pop()
 
 ```python
 last_node = single_linked_list.pop()
+last_node = cicrule_single_list.pop()
 print(last_node)  # Output: 3
 ```
 
 ### * Pop First
 - removes and returns the first node in the linked list.
 
 #### Method: 
 - pop_first()
 
 ```python
 first_node = single_linked_list.pop_first()
+first_node = cicrule_single_list.pop_first()
 print(first_node)  # Output: 0
 ```
 
 ### * Remove
 - removes the node at the specified index from the linked list.
 
 #### Method: 
 - remove(index)
 
 `index(int)` : The index of the node to be removed.
 
 ```python
 single_linked_list.remove(2)
+cicrule_single_list.remove(2)
 ```
 
 ### * Clear
 - clears all nodes in the linked list.
 
 #### Method: 
 - clear()
 
 ```python
 single_linked_list.clear()
+cicrule_single_list.clear()
 ```
 
 ### * Get Length
 - returns the current size (length) of the linked list.
 
 #### Method:
 -  __len__()
 
 ```python
 length = len(single_linked_list)
+length = len(cicrule_single_list)
 print(length)  # Output: 1
 ```
 
 ### * Traverse and print
 - traverses the linked list and prints the data of each node.
 
 #### Method: 
 - traverse()
 
 ```python
 single_linked_list.traverse()
+cicrule_single_list.traverse()
 # Output: 0 -> 1 -> 3
 ``` 
 
 ### * String representation
 - returns a string representation of the linked list.
 
 #### Method: 
 - __str__()
 
 ```python
 linked_list_str
-```
+```
```

### Comparing `single-linked-list-0.0.2/slll/slll.py` & `single-linked-list-0.0.3/slll/slll.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,172 +1,161 @@
 class Node:
     def __init__(self, data):
         self.data = data
         self.next = None
 
 
-
 class SingleLinkedList:
-
     def __init__(self):
         self.head = None
         self.tail = None
         self.length = 0
 
-    
     def __len__(self):
         """
         return SLLL size
         """
         return self.length
 
-
     def treaves(self):
         """
         treaves through nodes in SLLL
         """
         node = self.head
         while node is not None:
             print(node.data)
             node = node.next
 
-
     def __str__(self) -> str:
         """
         return node in SLLL
         """
         node = self.head
-        result = ''
+        result = ""
         while node is not None:
             result += str(node.data)
             if node.next is not None:
-                result += ' ---> '
+                result += " --> "
             node = node.next
         return result
 
-
     def append(self, data):
         """
         insert node in SLLL
         """
         node = Node(data=data)
         if self.head is None:
             self.head = node
             self.tail = node
         else:
             self.tail.next = node
             self.tail = node
         self.length += 1
 
-
-    def preappend(self, data):
+    def pre_append(self, data):
         """
         insert node at the beginning of SLLL
         """
         node = Node(data=data)
         if self.head is None:
             self.head = node
             self.tail = node
         else:
-            node.next =  self.head
+            node.next = self.head
             self.head = node
         self.length += 1
 
-
     def insert(self, index, data):
         """
         insert a node at given index in SLLL
         """
         node = Node(data=data)
-        if index < 0 or index > self.length:
+        if index > self.length:
             return None
         if self.length == 0:
             self.tail = self.head = node
-        if index == 0:
+        elif index == -1:
+            self.tail.next = node
+            self.tail = node
+        elif index == 0:
             node.next = self.head
             self.head = node
         else:
+            temp_node = self.head
             for _ in range(index - 1):
-                temp_node = self.head
                 temp_node = temp_node.next
             node.next = temp_node.next
             temp_node.next = node
         self.length += 1
 
-
     def find(self, data):
         """
         return node index from SLLL which contain data
         """
         node = self.head
         index = 0
         while node is not None:
             if node.data == data:
                 return index
             node = node.next
             index += 1
         return None
 
-
     def get(self, index):
         """
         return node from SLLL by index
         """
         if index == -1:
             return self.tail.data
         if index < -1 or index > self.length:
             return None
         node = self.head
         for _ in range(index):
             node = node.next
         return node.data
-    
+
     def _get(self, index):
         """
         return node from SLLL by index
         """
         if index == -1:
             return self.tail
         if index < -1 or index > self.length:
             return None
         node = self.head
         for _ in range(index):
             node = node.next
         return node
 
-
-
     def set(self, index, data):
         """
         set node in SLLL by index and value
         """
         node = self._get(index=index)
         if node:
             node.data = data
         return node.data
 
-
     def pop(self):
         """
         remove and return last node in SLLL
         """
         node = self.tail
         if self.length == 0:
             return None
-        if self.length == 1:
-            self.tail = self.head =  None
+        elif self.length == 1:
+            self.tail = self.head = None
             return node.data
         else:
             temp = self.head
             while temp.next is not self.tail:
                 temp = temp.next
             temp.next = None
             self.tail = temp
         return node.data
-    
 
     def pop_first(self):
         """
         remove and return first node in SLLL
         """
         if self.head is None:
             return None
@@ -176,15 +165,14 @@
             return node.data
         else:
             self.head = self.head.next
             node.next = None
         self.length -= 1
         return node.data
 
-    
     def remove(self, index):
         """
         remove node at given index from SLLL
         """
         if index < 0 or index >= self.length:
             return None
         if index == 0:
@@ -194,14 +182,13 @@
         else:
             prev_node = self._get(index=index - 1)
             node = prev_node.next
             prev_node.next = node.next
             node.next = None
         self.length -= 1
 
-
     def clear(self):
         """
         clear all nodes in SLLl
         """
         self.head = self.tail = None
         self.length = 0
```

