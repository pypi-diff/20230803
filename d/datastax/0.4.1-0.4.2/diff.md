# Comparing `tmp/datastax-0.4.1.tar.gz` & `tmp/datastax-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastax-0.4.1.tar", last modified: Wed Jul 12 09:39:13 2023, max compression
+gzip compressed data, was "datastax-0.4.2.tar", last modified: Thu Aug  3 18:23:21 2023, max compression
```

## Comparing `datastax-0.4.1.tar` & `datastax-0.4.2.tar`

### file list

```diff
@@ -1,69 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.885777 datastax-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 09:39:04.000000 datastax-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-12 09:39:13.885777 datastax-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-07-12 09:39:04.000000 datastax-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax/Arrays/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Arrays/AbstractArrays/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/Stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/AbstractArrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/PriorityQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/Stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Arrays/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Lists/AbstractLists/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/CircularLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyCircularList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/DoublyNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/AbstractLists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/CircularLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyCircularList.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyLinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/DoublyNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/LRUCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/LinkedList.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Utils/Commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.881777 datastax-0.4.1/datastax/trees/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/avl_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/expression_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/fibonacci_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/min_heap_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/min_segment_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.885777 datastax-0.4.1/datastax/trees/private_trees/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/huffman_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/private_trees/threaded_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/red_black_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/splay_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/sum_segment_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 09:39:04.000000 datastax-0.4.1/datastax/trees/threaded_binary_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:39:13.877777 datastax-0.4.1/datastax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 09:39:13.000000 datastax-0.4.1/datastax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:39:13.885777 datastax-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-12 09:39:04.000000 datastax-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.181516 datastax-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 18:23:02.000000 datastax-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-03 18:23:21.181516 datastax-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-08-03 18:23:02.000000 datastax-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.161516 datastax-0.4.2/datastax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.161516 datastax-0.4.2/datastax/Arrays/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.161516 datastax-0.4.2/datastax/Arrays/AbstractArrays/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/AbstractArrays/Array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/AbstractArrays/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/AbstractArrays/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/AbstractArrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/PriorityQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Arrays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.165516 datastax-0.4.2/datastax/Lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.165516 datastax-0.4.2/datastax/Lists/AbstractLists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/AbstractLists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/CircularLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/DoublyCircularList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/DoublyLinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/LRUCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/LinkedList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Lists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.169516 datastax-0.4.2/datastax/Nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AVLNode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.169516 datastax-0.4.2/datastax/Nodes/AbstractNodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/HuffmanNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/RedBlackNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/SegmentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/ThreadedNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/TreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/AbstractNodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/DoublyNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/HeapNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/HuffmanNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/RedBlackNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/SegmentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/SplayNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/ThreadedNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/TreeNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.169516 datastax-0.4.2/datastax/Tables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.169516 datastax-0.4.2/datastax/Tables/AbstractTables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Tables/AbstractTables/HuffmanTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Tables/AbstractTables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Tables/HuffmanTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.177516 datastax-0.4.2/datastax/Trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AVLTree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.177516 datastax-0.4.2/datastax/Trees/AbstractTrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/BinaryTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/HuffmanTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/RedBlackTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/SegmentTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/ThreadedBinaryTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/AbstractTrees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/BinarySearchTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/BinaryTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/ExpressionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/FibonacciTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/HeapTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/HuffmanTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/MinHeapTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/MinSegmentTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/RedBlackTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/SegmentTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/SplayTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/SumSegmentTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/ThreadedBinaryTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Trees/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.177516 datastax-0.4.2/datastax/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/ColorCodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.181516 datastax-0.4.2/datastax/Utils/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/DatastaxException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/InvalidExpressionException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/OverflowException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/PathNotFoundException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/PathNotGivenException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/UnderflowException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/UnmatchedBracketPairException.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.181516 datastax-0.4.2/datastax/Utils/Warnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Warnings/DatastaxWarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/Warnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 18:23:02.000000 datastax-0.4.2/datastax/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:23:21.161516 datastax-0.4.2/datastax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-08-03 18:23:21.000000 datastax-0.4.2/datastax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 18:23:21.000000 datastax-0.4.2/datastax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:23:21.000000 datastax-0.4.2/datastax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-03 18:23:21.000000 datastax-0.4.2/datastax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:23:21.181516 datastax-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-08-03 18:23:02.000000 datastax-0.4.2/setup.py
```

### Comparing `datastax-0.4.1/LICENSE` & `datastax-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datastax-0.4.1/PKG-INFO` & `datastax-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datastax
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python library to handle dataStructures
 Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax
 Author: Pritam K
 Author-email: pritamkundu771@gmail.com
 Maintainer: Pritam Kundu
 License: MIT
@@ -19,31 +19,27 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed
-Requires-Python: >=3.11
+Requires-Python: >3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-    updated: Wednesday, 12th July 2023
+    updated: Thursday, 03rd August 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -68,28 +64,37 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored Array Contents
-- Added AbstractArray SubModule to abstract print logic
-- Added more test cases for Queues
-- Type Checked Arrays and Lists with mypy
+- Refactored Trees
+- Added Nodes SubPackage
+- Separated TreeNodes into Nodes
+- Added Tables SubPackage
+- Added Colors and ColorCodes in Utils
+- Refactored Lists
+- Removed `__repr__` overrides
+- Added Exceptions in Utils
+- Added Warnings in Utils
+- Added new workflows
+- Added datastax.Wiki
 
 ## Table of Contents
 
+- [What's New](#whats-new)
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
-- [What's Next](#whats-next)
+- [Documentation](#documentation)
+- [License](#license)
 
 ## Introduction
 
 - This library offers a simple yet powerful solution for implementing common abstract data structures.
 - With a pure Python implementation, it provides representations of tree, linked list, and array-based data structures
   accessible through a basic command prompt interface.
 - The package includes visualization features that enhance the understanding of each data structure.
@@ -149,15 +154,15 @@
   1. LinkedLists
   2. Trees
   3. Arrays
   
   Usage
   > py datastax <data-structure> [data]
   Data Structures:
-  ->  trees          Hierarchical DS
+  ->  Trees          Hierarchical DS
   ->  linkedlists    Linear DS
   ->  arrays         Fixed Size Linear DS
 
   ```
 - Then follow as the instruction guides
 
 ```bash
@@ -179,20 +184,19 @@
   ...
 ```
 
 ### Practical Usage
 
 - **Queue**
 
-![queue](https://github.com/warmachine028/datastax/assets/75939390/0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409)
+![queue](https://github.com/warmachine028/datastax/assets/75939390/e62ba451-f499-45dc-bcb9-9e29ebfe6dbd)
 
 ![queue_output](https://github.com/warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde)
 
-------------------------------------
----------------
+---------------------------------------------------
 
 - **BinaryTree**
 
 ![binaryTree](https://github.com/warmachine028/datastax/assets/75939390/7228c4b4-def7-4c6b-9e29-e6e244c2c4c1)
 
 ![binaryTree_output](https://github.com/warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c)
 
@@ -220,25 +224,33 @@
 
 ![sst_output](https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-88c7-40e4dcc11215)
 
 ---------------------------------------------------
 
 - **HuffmanTree**
 
-![hft](https://github.com/warmachine028/datastax/assets/75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e)
+![hft](https://github.com/warmachine028/datastax/assets/75939390/bab7da94-624f-40ac-b746-463157e84cdf)
 
 ![hft_output](https://github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-8dbf91c008a2)
 
 ---------------------------------------------------
 
 - **RedBlackTree**
 
 ![rbt](https://github.com/warmachine028/datastax/assets/75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba)
 
 ![rbt_output](https://github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-db84dbf274f0)
 
-## What's Next
+## Documentation
+
+- For detailed documentation. See [documentation](https://github.com/warmachine028/datastax/wiki)
+- (Still in progress) 
+
+## License
+
+- see [LICENSE]
+
+**Pritam, 2023**
+
+[license]: https://github.com/warmachine028/datastax/blob/main/LICENSE
 
-- Enhanced Documentation
-- Better TestCases for Huffman Tree
-- Better TestCases for Segment Trees
-- Test Cases for Fibonacci Tree
+<!-- 03/08/23 -->
```

#### html2text {}

```diff
@@ -1,93 +1,94 @@
-Metadata-Version: 2.1 Name: datastax Version: 0.4.1 Summary: A python library
+Metadata-Version: 2.1 Name: datastax Version: 0.4.2 Summary: A python library
 to handle dataStructures Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax Author: Pritam K Author-
 email: pritamkundu771@gmail.com Maintainer: Pritam Kundu License: MIT Project-
 URL: Bug Tracker, https://github.com/warmachine028/datastax/issues Project-URL:
 Documentation, https://github.com/warmachine028/datastax#readme Project-URL:
 Source Code, https://github.com/warmachine028/datastax Platform: Windows
 Platform: Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Documentation
-Classifier: Topic :: Education :: Testing Classifier: Topic :: Scientific/
-Engineering :: Visualization Classifier: Topic :: Software Development ::
-Documentation Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Testing :: Unit
-Classifier: Typing :: Typed Requires-Python: >=3.11 Description-Content-Type:
-text/markdown License-File: LICENSE updated: Wednesday, 12th July 2023
+Independent Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Documentation Classifier: Topic :: Education :: Testing Classifier:
+Topic :: Scientific/Engineering :: Visualization Classifier: Topic :: Software
+Development :: Documentation Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Testing :: Unit Classifier: Typing :: Typed Requires-Python: >3.11 Description-
+Content-Type: text/markdown License-File: LICENSE updated: Thursday, 03rd
+August 2023
                                   [datastax]
                          Simplicity meets intelligence
                            [PyPI] [PyPI_Downloads]
             [https://img.shields.io/github/v/release/warmachine028/
      datastax?color=brightgreen] [https://img.shields.io/github/v/release/
                                 warmachine028/
       datastax?color=lightgreen&include_prereleases&label=pre%20release]
     [https://img.shields.io/github/stars/warmachine028/datastax] [https://
  img.shields.io/github/license/warmachine028/datastax?color=orange] [https://
         img.shields.io/github/forks/warmachine028/datastax?color=cyan]
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored Array Contents - Added AbstractArray SubModule to abstract print
-logic - Added more test cases for Queues - Type Checked Arrays and Lists with
-mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
-(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
-[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
-Introduction - This library offers a simple yet powerful solution for
-implementing common abstract data structures. - With a pure Python
-implementation, it provides representations of tree, linked list, and array-
-based data structures accessible through a basic command prompt interface. -
-The package includes visualization features that enhance the understanding of
-each data structure. - Students can greatly benefit from utilizing this package
-for their learning and educational purposes. - Please note that this project is
-currently a work in progress and undergoing active development. ## Problem
-Statement - Many CS students encounter difficulties in comprehending the
-intricate internal architecture of complex Abstract Data Types (ADTs) during
-the initial stages of their B.Tech course. - When attempting to solve coding
-challenges that involve writing test cases using these ADTs, it becomes
-excessively burdensome to manually create these data structures from scratch. -
-Furthermore, while developing programs that implement these ADTs, numerous
-errors are encountered due to the inability to visualize and understand the
-underlying processes of these data structures. ## Benefits - Swift installation
-process - Efficient and prompt updates - Minimal disk space usage due to its
-small size - No additional modules or dependencies needed - Developed entirely
-from scratch - Upcoming user-friendly documentation - Command line
-demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
-(Suggesting you to always update to the latest python version) ## Installation
-1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
-install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
-demo of the library use the following command - **Windows**: ```bash > py -
-m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
-_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
-> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
-Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
-guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
-Singly Linked List: HEAD TAIL âââââââ¥âââââ
+Refactored Trees - Added Nodes SubPackage - Separated TreeNodes into Nodes -
+Added Tables SubPackage - Added Colors and ColorCodes in Utils - Refactored
+Lists - Removed `__repr__` overrides - Added Exceptions in Utils - Added
+Warnings in Utils - Added new workflows - Added datastax.Wiki ## Table of
+Contents - [What's New](#whats-new) - [Introduction](#introduction) - [Problem
+Statement](#problem-statement) - [Benefits](#benefits) - [Requirements]
+(#requirements) - [Installation](#installation) - [Usage](#usage) -
+[Documentation](#documentation) - [License](#license) ## Introduction - This
+library offers a simple yet powerful solution for implementing common abstract
+data structures. - With a pure Python implementation, it provides
+representations of tree, linked list, and array-based data structures
+accessible through a basic command prompt interface. - The package includes
+visualization features that enhance the understanding of each data structure. -
+Students can greatly benefit from utilizing this package for their learning and
+educational purposes. - Please note that this project is currently a work in
+progress and undergoing active development. ## Problem Statement - Many CS
+students encounter difficulties in comprehending the intricate internal
+architecture of complex Abstract Data Types (ADTs) during the initial stages of
+their B.Tech course. - When attempting to solve coding challenges that involve
+writing test cases using these ADTs, it becomes excessively burdensome to
+manually create these data structures from scratch. - Furthermore, while
+developing programs that implement these ADTs, numerous errors are encountered
+due to the inability to visualize and understand the underlying processes of
+these data structures. ## Benefits - Swift installation process - Efficient and
+prompt updates - Minimal disk space usage due to its small size - No additional
+modules or dependencies needed - Developed entirely from scratch - Upcoming
+user-friendly documentation - Command line demonstration for easy usage ##
+Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
+to the latest python version) ## Installation 1. Use the python package manager
+[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
+datastax ``` ## Usage ### Demo - To get a demo of the library use the following
+command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
+```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
+LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
+> Trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
+``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
+1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
------>â 4 â -----> NULL âââââââ¨âââââ
+âââââââ¥âââââ âââââââ¥âââââ â 1
+â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ âââââââ¨âââââ 2.
+Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ ... ``` ### Practical Usage
 - **Queue** ![queue](https://github.com/warmachine028/datastax/assets/75939390/
-0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409) ![queue_output](https://github.com/
+e62ba451-f499-45dc-bcb9-9e29ebfe6dbd) ![queue_output](https://github.com/
 warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde) --
----------------------------------- --------------- - **BinaryTree** !
+------------------------------------------------- - **BinaryTree** !
 [binaryTree](https://github.com/warmachine028/datastax/assets/75939390/
 7228c4b4-def7-4c6b-9e29-e6e244c2c4c1) ![binaryTree_output](https://github.com/
 warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c) --
 ------------------------------------------------- - **MinHeapTree** ![mht]
 (https://github.com/warmachine028/datastax/assets/75939390/1c00a207-9ea0-4965-
 898f-29e37883fac5) ![mht_output](https://github.com/warmachine028/datastax/
 assets/75939390/fcfe24d9-6b80-4b16-873c-3f5c3d808d70) -------------------------
@@ -96,16 +97,17 @@
 [tbt_output](https://github.com/warmachine028/datastax/assets/75939390/
 9e77c5dc-082c-471b-90d5-33792673bdf3) -----------------------------------------
 ---------- - **SumSegmentTree** ![sst](https://github.com/warmachine028/
 datastax/assets/75939390/7bdcfd6e-37ac-4421-b6d2-acd59cf4976c) ![sst_output]
 (https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-
 88c7-40e4dcc11215) --------------------------------------------------- -
 **HuffmanTree** ![hft](https://github.com/warmachine028/datastax/assets/
-75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e) ![hft_output](https://
+75939390/bab7da94-624f-40ac-b746-463157e84cdf) ![hft_output](https://
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
-db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
-Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree
+db84dbf274f0) ## Documentation - For detailed documentation. See
+[documentation](https://github.com/warmachine028/datastax/wiki) - (Still in
+progress) ## License - see [LICENSE] **Pritam, 2023** [license]: https://
+github.com/warmachine028/datastax/blob/main/LICENSE
```

### Comparing `datastax-0.4.1/README.md` & `datastax-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-    updated: Wednesday, 12th July 2023
+    updated: Thursday, 03rd August 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -27,28 +27,37 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored Array Contents
-- Added AbstractArray SubModule to abstract print logic
-- Added more test cases for Queues
-- Type Checked Arrays and Lists with mypy
+- Refactored Trees
+- Added Nodes SubPackage
+- Separated TreeNodes into Nodes
+- Added Tables SubPackage
+- Added Colors and ColorCodes in Utils
+- Refactored Lists
+- Removed `__repr__` overrides
+- Added Exceptions in Utils
+- Added Warnings in Utils
+- Added new workflows
+- Added datastax.Wiki
 
 ## Table of Contents
 
+- [What's New](#whats-new)
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
-- [What's Next](#whats-next)
+- [Documentation](#documentation)
+- [License](#license)
 
 ## Introduction
 
 - This library offers a simple yet powerful solution for implementing common abstract data structures.
 - With a pure Python implementation, it provides representations of tree, linked list, and array-based data structures
   accessible through a basic command prompt interface.
 - The package includes visualization features that enhance the understanding of each data structure.
@@ -108,15 +117,15 @@
   1. LinkedLists
   2. Trees
   3. Arrays
   
   Usage
   > py datastax <data-structure> [data]
   Data Structures:
-  ->  trees          Hierarchical DS
+  ->  Trees          Hierarchical DS
   ->  linkedlists    Linear DS
   ->  arrays         Fixed Size Linear DS
 
   ```
 - Then follow as the instruction guides
 
 ```bash
@@ -138,20 +147,19 @@
   ...
 ```
 
 ### Practical Usage
 
 - **Queue**
 
-![queue](https://github.com/warmachine028/datastax/assets/75939390/0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409)
+![queue](https://github.com/warmachine028/datastax/assets/75939390/e62ba451-f499-45dc-bcb9-9e29ebfe6dbd)
 
 ![queue_output](https://github.com/warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde)
 
-------------------------------------
----------------
+---------------------------------------------------
 
 - **BinaryTree**
 
 ![binaryTree](https://github.com/warmachine028/datastax/assets/75939390/7228c4b4-def7-4c6b-9e29-e6e244c2c4c1)
 
 ![binaryTree_output](https://github.com/warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c)
 
@@ -179,25 +187,33 @@
 
 ![sst_output](https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-88c7-40e4dcc11215)
 
 ---------------------------------------------------
 
 - **HuffmanTree**
 
-![hft](https://github.com/warmachine028/datastax/assets/75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e)
+![hft](https://github.com/warmachine028/datastax/assets/75939390/bab7da94-624f-40ac-b746-463157e84cdf)
 
 ![hft_output](https://github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-8dbf91c008a2)
 
 ---------------------------------------------------
 
 - **RedBlackTree**
 
 ![rbt](https://github.com/warmachine028/datastax/assets/75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba)
 
 ![rbt_output](https://github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-db84dbf274f0)
 
-## What's Next
+## Documentation
+
+- For detailed documentation. See [documentation](https://github.com/warmachine028/datastax/wiki)
+- (Still in progress) 
+
+## License
+
+- see [LICENSE]
+
+**Pritam, 2023**
+
+[license]: https://github.com/warmachine028/datastax/blob/main/LICENSE
 
-- Enhanced Documentation
-- Better TestCases for Huffman Tree
-- Better TestCases for Segment Trees
-- Test Cases for Fibonacci Tree
+<!-- 03/08/23 -->
```

#### html2text {}

```diff
@@ -1,72 +1,75 @@
- updated: Wednesday, 12th July 2023
+ updated: Thursday, 03rd August 2023
                                   [datastax]
                          Simplicity meets intelligence
                            [PyPI] [PyPI_Downloads]
             [https://img.shields.io/github/v/release/warmachine028/
      datastax?color=brightgreen] [https://img.shields.io/github/v/release/
                                 warmachine028/
       datastax?color=lightgreen&include_prereleases&label=pre%20release]
     [https://img.shields.io/github/stars/warmachine028/datastax] [https://
  img.shields.io/github/license/warmachine028/datastax?color=orange] [https://
         img.shields.io/github/forks/warmachine028/datastax?color=cyan]
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored Array Contents - Added AbstractArray SubModule to abstract print
-logic - Added more test cases for Queues - Type Checked Arrays and Lists with
-mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
-(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
-[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
-Introduction - This library offers a simple yet powerful solution for
-implementing common abstract data structures. - With a pure Python
-implementation, it provides representations of tree, linked list, and array-
-based data structures accessible through a basic command prompt interface. -
-The package includes visualization features that enhance the understanding of
-each data structure. - Students can greatly benefit from utilizing this package
-for their learning and educational purposes. - Please note that this project is
-currently a work in progress and undergoing active development. ## Problem
-Statement - Many CS students encounter difficulties in comprehending the
-intricate internal architecture of complex Abstract Data Types (ADTs) during
-the initial stages of their B.Tech course. - When attempting to solve coding
-challenges that involve writing test cases using these ADTs, it becomes
-excessively burdensome to manually create these data structures from scratch. -
-Furthermore, while developing programs that implement these ADTs, numerous
-errors are encountered due to the inability to visualize and understand the
-underlying processes of these data structures. ## Benefits - Swift installation
-process - Efficient and prompt updates - Minimal disk space usage due to its
-small size - No additional modules or dependencies needed - Developed entirely
-from scratch - Upcoming user-friendly documentation - Command line
-demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
-(Suggesting you to always update to the latest python version) ## Installation
-1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
-install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
-demo of the library use the following command - **Windows**: ```bash > py -
-m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
-_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
-> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
-Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
-guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
-Singly Linked List: HEAD TAIL âââââââ¥âââââ
+Refactored Trees - Added Nodes SubPackage - Separated TreeNodes into Nodes -
+Added Tables SubPackage - Added Colors and ColorCodes in Utils - Refactored
+Lists - Removed `__repr__` overrides - Added Exceptions in Utils - Added
+Warnings in Utils - Added new workflows - Added datastax.Wiki ## Table of
+Contents - [What's New](#whats-new) - [Introduction](#introduction) - [Problem
+Statement](#problem-statement) - [Benefits](#benefits) - [Requirements]
+(#requirements) - [Installation](#installation) - [Usage](#usage) -
+[Documentation](#documentation) - [License](#license) ## Introduction - This
+library offers a simple yet powerful solution for implementing common abstract
+data structures. - With a pure Python implementation, it provides
+representations of tree, linked list, and array-based data structures
+accessible through a basic command prompt interface. - The package includes
+visualization features that enhance the understanding of each data structure. -
+Students can greatly benefit from utilizing this package for their learning and
+educational purposes. - Please note that this project is currently a work in
+progress and undergoing active development. ## Problem Statement - Many CS
+students encounter difficulties in comprehending the intricate internal
+architecture of complex Abstract Data Types (ADTs) during the initial stages of
+their B.Tech course. - When attempting to solve coding challenges that involve
+writing test cases using these ADTs, it becomes excessively burdensome to
+manually create these data structures from scratch. - Furthermore, while
+developing programs that implement these ADTs, numerous errors are encountered
+due to the inability to visualize and understand the underlying processes of
+these data structures. ## Benefits - Swift installation process - Efficient and
+prompt updates - Minimal disk space usage due to its small size - No additional
+modules or dependencies needed - Developed entirely from scratch - Upcoming
+user-friendly documentation - Command line demonstration for easy usage ##
+Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
+to the latest python version) ## Installation 1. Use the python package manager
+[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
+datastax ``` ## Usage ### Demo - To get a demo of the library use the following
+command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
+```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
+LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
+> Trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
+``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
+1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
------>â 4 â -----> NULL âââââââ¨âââââ
+âââââââ¥âââââ âââââââ¥âââââ â 1
+â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ âââââââ¨âââââ 2.
+Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ ... ``` ### Practical Usage
 - **Queue** ![queue](https://github.com/warmachine028/datastax/assets/75939390/
-0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409) ![queue_output](https://github.com/
+e62ba451-f499-45dc-bcb9-9e29ebfe6dbd) ![queue_output](https://github.com/
 warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde) --
----------------------------------- --------------- - **BinaryTree** !
+------------------------------------------------- - **BinaryTree** !
 [binaryTree](https://github.com/warmachine028/datastax/assets/75939390/
 7228c4b4-def7-4c6b-9e29-e6e244c2c4c1) ![binaryTree_output](https://github.com/
 warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c) --
 ------------------------------------------------- - **MinHeapTree** ![mht]
 (https://github.com/warmachine028/datastax/assets/75939390/1c00a207-9ea0-4965-
 898f-29e37883fac5) ![mht_output](https://github.com/warmachine028/datastax/
 assets/75939390/fcfe24d9-6b80-4b16-873c-3f5c3d808d70) -------------------------
@@ -75,16 +78,17 @@
 [tbt_output](https://github.com/warmachine028/datastax/assets/75939390/
 9e77c5dc-082c-471b-90d5-33792673bdf3) -----------------------------------------
 ---------- - **SumSegmentTree** ![sst](https://github.com/warmachine028/
 datastax/assets/75939390/7bdcfd6e-37ac-4421-b6d2-acd59cf4976c) ![sst_output]
 (https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-
 88c7-40e4dcc11215) --------------------------------------------------- -
 **HuffmanTree** ![hft](https://github.com/warmachine028/datastax/assets/
-75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e) ![hft_output](https://
+75939390/bab7da94-624f-40ac-b746-463157e84cdf) ![hft_output](https://
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
-db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
-Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree
+db84dbf274f0) ## Documentation - For detailed documentation. See
+[documentation](https://github.com/warmachine028/datastax/wiki) - (Still in
+progress) ## License - see [LICENSE] **Pritam, 2023** [license]: https://
+github.com/warmachine028/datastax/blob/main/LICENSE
```

### Comparing `datastax-0.4.1/datastax/Arrays/AbstractArrays/Array.py` & `datastax-0.4.2/datastax/Arrays/AbstractArrays/Array.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.1/datastax/Arrays/AbstractArrays/Queue.py` & `datastax-0.4.2/datastax/Arrays/AbstractArrays/Queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,7 +75,10 @@
     @abstractmethod
     def dequeue(self) -> Any:
         ...
 
     @abstractmethod
     def peek(self) -> Any:
         ...
+
+    def __len__(self):
+        return len(self.array)
```

### Comparing `datastax-0.4.1/datastax/Arrays/AbstractArrays/Stack.py` & `datastax-0.4.2/datastax/Arrays/AbstractArrays/Stack.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.1/datastax/Arrays/AbstractArrays/__init__.py` & `datastax-0.4.2/datastax/Arrays/AbstractArrays/__init__.py`

 * *Files identical despite different names*

### Comparing `datastax-0.4.1/datastax/Arrays/PriorityQueue.py` & `datastax-0.4.2/datastax/Arrays/PriorityQueue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Priority Queue implementation using Lists (Pseudo Arrays)
 from typing import Any, Callable, Optional
 
 from datastax.Arrays.Queue import Queue
-from datastax.errors import OverFlowError, UnderFlowError
+from datastax.Utils.Exceptions import OverflowException, UnderflowException
 
 
 class PriorityQueue(Queue):
     comparator: Callable
 
     def __init__(self, *, capacity: Optional[int] = None,
                  custom_comparator: Optional[Callable] = None):
@@ -34,26 +34,26 @@
         if root == index:
             return
         self.swap(root, index)
         self.heapify(root, length)
 
     def dequeue(self) -> Any:
         if self.is_empty():
-            raise UnderFlowError(self)
+            raise UnderflowException(self)
 
         deleted_item = self._array[self._front]
         self._array[self._front] = self._array[-1]
         self._array.pop()
         self._rear -= 1
         self.heapify(0, len(self.array))
         return deleted_item
 
     def enqueue(self, item: Any) -> int:
         if self.is_full():
-            raise OverFlowError(self)
+            raise OverflowException(self)
 
         self._array.append(item)
         self._rear += 1
         n = len(self.array)
         for i in range(n // 2 - 1, -1, -1):
             try:
                 self.heapify(i, n)
```

### Comparing `datastax-0.4.1/datastax/Arrays/Queue.py` & `datastax-0.4.2/datastax/Arrays/Queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Queue Implementation using Lists (Pseudo Arrays)
 from typing import Any, Optional
 
-from datastax.errors import OverFlowError, UnderFlowError
+from datastax.Utils.Exceptions import OverflowException, UnderflowException
 from datastax.Arrays.AbstractArrays import Queue as AbstractQueue
 
 
 class Queue(AbstractQueue):
     def __init__(self, *, capacity: Optional[int] = None):
         self._array = []
         self.set_capacity(capacity)
@@ -14,27 +14,24 @@
         return len(self.array) == self.capacity
 
     def is_empty(self) -> bool:
         return not self.array
 
     def enqueue(self, item: Any) -> int:
         if self.is_full():
-            raise OverFlowError(self)
+            raise OverflowException(self)
 
         self._array.append(item)
         self._rear += 1
         return 0
 
     def dequeue(self) -> Any:
         if self.is_empty() or self.front >= self.rear:
-            raise UnderFlowError(self)
+            raise UnderflowException(self)
         deleted_item = self._array[self.front]
         self._front += 1
         return deleted_item
 
-    def __len__(self):
-        return len(self.array)
-
     def peek(self) -> Any:
         if self.is_empty() or self._front >= self._rear:
             return "QUEUE EMPTY"
         return self._array[self.front]
```

### Comparing `datastax-0.4.1/datastax/Arrays/Stack.py` & `datastax-0.4.2/datastax/Arrays/Stack.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Stack Implementation using Lists (Pseudo Arrays)
 from typing import Any, Optional
 
-from datastax.errors import UnderFlowError, OverFlowError
+from datastax.Utils.Exceptions import UnderflowException, OverflowException
 from datastax.Arrays.AbstractArrays import Stack as AbstractStack
 
 
 class Stack(AbstractStack):
     def __init__(self, *, capacity: Optional[int] = None):
         self._array = []
         self.set_capacity(capacity)
@@ -14,22 +14,22 @@
         return len(self.array) == self.capacity
 
     def is_empty(self) -> bool:
         return not self.array
 
     def push(self, item: Any) -> int:
         if self.is_full():  # Overflow Condition
-            raise OverFlowError(self)
+            raise OverflowException(self)
 
         self.array.append(item)
         return 0
 
     def pop(self) -> Any:
         if self.is_empty():  # Underflow Condition handled
-            raise UnderFlowError(self)
+            raise UnderflowException(self)
         return self.array.pop()
 
     def __len__(self):
         return len(self.array)
 
     def peek(self) -> Any:
         return 'STACK EMPTY' if self.is_empty() else self.array[-1]
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/CircularLinkedList.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/CircularLinkedList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from abc import ABC
+from abc import ABC as AbstractClass
 from typing import Optional
+from datastax.Nodes.AbstractNodes import Node
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
 from datastax.Utils import Commons
-from datastax.Lists.AbstractLists.Node import Node
 
 
-class CircularLinkedList(LinkedList, ABC):
+class CircularLinkedList(LinkedList, AbstractClass):
     def _max_width(self, node: Optional[Node]):
         max_width = 0
         ref = node
         while ref:
             max_width = max(max_width, len(Commons.repr(ref.data)))
             ref = ref.next
             if ref is node:
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyCircularList.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/DoublyCircularList.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from abc import ABC
-
+from abc import ABC as AbstractClass
 from datastax.Lists.AbstractLists.CircularLinkedList import CircularLinkedList
 from datastax.Lists.AbstractLists.DoublyLinkedList import DoublyLinkedList
 from datastax.Utils import Commons
 
 
-class DoublyCircularList(DoublyLinkedList, CircularLinkedList, ABC):
+class DoublyCircularList(DoublyLinkedList, CircularLinkedList, AbstractClass):
 
     def __str__(self):
         if not self.head:
             return 'NULL'
         start_padding = 6
         top = '    '
         mid = ' ╭─'
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyLinkedList.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/DoublyLinkedList.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from abc import ABC
+from abc import ABC as AbstractClass
 from typing import Optional
+from datastax.Nodes import DoublyNode
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
 from datastax.Utils import Commons
-from datastax.Lists.AbstractLists.DoublyNode import DoublyNode
 
 
-class DoublyLinkedList(LinkedList, ABC):
+class DoublyLinkedList(LinkedList, AbstractClass):
     _head: Optional[DoublyNode] = None
     _tail: Optional[DoublyNode] = None
 
     def __str__(self):
         string = " NULL <"
         start_padding = 8
         bottom = top = " " * start_padding
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/DoublyNode.py` & `datastax-0.4.2/datastax/Nodes/AbstractNodes/DoublyNode.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from abc import ABC
+from abc import ABC as AbstractClass, abstractmethod
 from typing import Optional, Self
 
-from datastax.Lists.AbstractLists.Node import Node
+from datastax.Nodes.AbstractNodes.Node import Node
 from datastax.Utils import Commons
 
 
-class DoublyNode(Node, ABC):
+class DoublyNode(Node, AbstractClass):
     _next: Optional[Self]
     _prev: Optional[Self]
 
     @property
     def next(self):
         return self._next
 
@@ -23,7 +23,11 @@
         mid = (
             f"{' prev' if self.prev else ' NULL'}"
             f" <----  ║{f'{Commons.repr(self.data)}'.center(width)}║  ----> "
             f"{' next' if self.next else ' NULL'}\n"
         )
         dow = f"        └────╨{'─' * width}╨────┘\n"
         return top + mid + dow
+
+    @abstractmethod
+    def set_prev(self, prev: Self):
+        ...
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/LinkedList.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/LinkedList.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from abc import ABC as AbstractClass, abstractmethod
 from typing import Any, Optional, Self, Iterable
-from datastax.Lists.AbstractLists.Node import Node
+from datastax.Nodes import Node
 from datastax.Utils import Commons
-from abc import abstractmethod, ABC as AbstractClass
 
 
 class LinkedList(AbstractClass):
     _head: Optional[Node] = None
     _tail: Optional[Node] = None
 
     def _max_width(self, node: Optional[Node]):
@@ -40,14 +40,20 @@
         heading = self._draw_heading(nodes, length_per_node, start_padding)
         top += "\n"
         mid += f"{' ' if mid[-1] == '>' else ''}NULL\n"
         dow += "\n"
 
         return heading + top + mid + dow
 
+    def __iter__(self):
+        ref = self._head
+        while ref:
+            yield ref.data
+            ref = ref.next
+
     def _draw_heading(self, n: int, lpn: int, start_padding: int) -> str:
         if n == 0:
             return " "
         head, tail = "HEAD".center(lpn), "TAIL".center(lpn)
         spaces = " " * 3
         if self._head is self._tail:
             return f"{' ' * start_padding}{head}\n" \
@@ -65,7 +71,15 @@
     @abstractmethod
     def insert(self, data: Any) -> None:
         ...
 
     @abstractmethod
     def _construct(self, array: Iterable[Any]) -> Self:
         ...
+
+    @abstractmethod
+    def set_head(self, head: Node):
+        ...
+
+    @abstractmethod
+    def set_tail(self, tail: Node):
+        ...
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/Node.py` & `datastax-0.4.2/datastax/Nodes/AbstractNodes/Node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Self, Optional, Any
 from datastax.Utils import Commons
 from abc import ABC as AbstractClass, abstractmethod
 
 
 class Node(AbstractClass):
-    data: Optional[Any]
+    data: Any
     _next: Optional[Self]
 
     @property
     def next(self):
         return self._next
 
     def __str__(self):
@@ -18,9 +18,9 @@
             f" │{f'{Commons.repr(self.data)}'.center(width)}║ ------> "
             f"{'next' if self.next else 'NULL'}\n"
         )
         dow = f" └{'─' * width}╨────┘\n"
         return top + mid + dow
 
     @abstractmethod
-    def set_next(self, _next: Optional[Self]):
+    def set_next(self, _next: Self):
         ...
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/Queue.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/Queue.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-from abc import ABC, abstractmethod
+from abc import ABC as AbstractClass, abstractmethod
 from typing import Optional, Any
+from datastax.Nodes.AbstractNodes import Node
 from datastax.Lists.AbstractLists.LinkedList import LinkedList
-from datastax.Lists.AbstractLists.Node import Node
 from datastax.Utils import Commons
 
 
-class Queue(LinkedList, ABC):
+class Queue(LinkedList, AbstractClass):
     _capacity = 0
     _rear = 0
 
-    def append(self, data: Any) -> None:
-        raise NotImplementedError
-
-    def insert(self, data: Any) -> None:
-        raise NotImplementedError
-
     @property
     def capacity(self):
         return self._capacity
 
     def __str__(self, head: Optional[Node] = None):
         if self.is_empty():
             return '╔═══════════════════╗\n' \
```

### Comparing `datastax-0.4.1/datastax/Lists/AbstractLists/__init__.py` & `datastax-0.4.2/datastax/Lists/AbstractLists/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,20 @@
 - The intention is to enhance usability and readability, making it easier for users to utilize and work with the data structures in a straightforward manner.
 
 Through encapsulating the logic and providing a clear separation between the underlying functionality and the user interface, this subPackage promotes code organization and maintainability, ensuring that users can easily employ the data structures without being burdened by the underlying complexity.
 
 Author: Pritam Kundu
 Date: 2023-07-10
 """
-from .Node import Node
-from .DoublyNode import DoublyNode
 from .LinkedList import LinkedList
 from .DoublyLinkedList import DoublyLinkedList
 from .CircularLinkedList import CircularLinkedList
 from .DoublyCircularList import DoublyCircularList
 from .Queue import Queue
 
 __all__ = [
-    'Node',
-    'DoublyNode',
     'LinkedList',
     'DoublyLinkedList',
     'CircularLinkedList',
     'DoublyCircularList',
     'Queue'
 ]
```

### Comparing `datastax-0.4.1/datastax/Lists/CircularLinkedList.py` & `datastax-0.4.2/datastax/Lists/CircularLinkedList.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Any
-
 from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import CircularLinkedList as AbstractList
 
 
-class CircularLinkedList(AbstractList, LinkedList):
+class CircularLinkedList(LinkedList, AbstractList):
     def append(self, data: Any) -> None:
         super().append(data)
         self.tail.set_next(self.head)
 
     def insert(self, data: Any):
         super().insert(data)
         self.tail.set_next(self.head)
```

### Comparing `datastax-0.4.1/datastax/Lists/DoublyCircularList.py` & `datastax-0.4.2/datastax/Lists/DoublyCircularList.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
-
 from datastax.Lists.DoublyLinkedList import DoublyLinkedList
 from datastax.Lists.CircularLinkedList import CircularLinkedList
 from datastax.Lists.AbstractLists import DoublyCircularList as AbstractList
 
 
-class DoublyCircularList(AbstractList, CircularLinkedList, DoublyLinkedList):
+class DoublyCircularList(CircularLinkedList, DoublyLinkedList, AbstractList):
 
     def append(self, data: Any) -> None:
         super().append(data)
         self.head.set_prev(self.tail)
         self.tail.set_next(self.head)
 
     def insert(self, data: Any) -> None:
```

### Comparing `datastax-0.4.1/datastax/Lists/DoublyLinkedList.py` & `datastax-0.4.2/datastax/Lists/DoublyLinkedList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Any, Optional, Iterable, Self
-
-from datastax.Lists.DoublyNode import DoublyNode
+from datastax.Nodes import DoublyNode
 from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import DoublyLinkedList as AbstractList
 
 
-class DoublyLinkedList(AbstractList, LinkedList):
-    def __init__(self, items: Optional[Iterable[Any]] = None,
+class DoublyLinkedList(LinkedList, AbstractList):
+    def __init__(self, items: Optional[Iterable] = None,
                  head: Optional[DoublyNode] = None,
                  tail: Optional[DoublyNode] = None):
         if head and tail:
             head.set_next(tail)
             tail.set_prev(head)
         super().__init__(items, head, tail)
```

### Comparing `datastax-0.4.1/datastax/Lists/DoublyNode.py` & `datastax-0.4.2/datastax/Nodes/DoublyNode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Self, Optional
+from datastax.Nodes.Node import Node
+from datastax.Nodes.AbstractNodes import DoublyNode as AbstractNode
 
-from datastax.Lists.Node import Node
-from datastax.Lists.AbstractLists import DoublyNode as AbstractNode
 
-
-class DoublyNode(AbstractNode, Node):
+class DoublyNode(Node, AbstractNode):
     def __init__(self, data: Any,
                  _next: Optional[Self] = None,
                  prev: Optional[Self] = None):
         super().__init__(data)
         self.set_next(_next)
         self.set_prev(prev)
 
-    def set_next(self, _next: Optional[Self] = None):
-        if _next is not None and not isinstance(_next, DoublyNode):
-            raise TypeError("The 'next' parameter must be an "
-                            "instance of DoublyNode or its subclass.")
-        super().set_next(_next)
+    def set_next(self, _next: Optional[Self]):
+        if _next is None or isinstance(_next, DoublyNode):
+            super().set_next(_next)
+            return
+        raise TypeError("The 'next' parameter must be an "
+                        "instance of DoublyNode or its subclass.")
 
-    def set_prev(self, prev: Optional[Self] = None):
+    def set_prev(self, prev: Optional[Self]):
         if prev is None or isinstance(prev, DoublyNode):
             self._prev = prev
             return
         raise TypeError("The 'prev' parameter must be an "
                         "instance of DoublyNode or its subclass.")
```

### Comparing `datastax-0.4.1/datastax/Lists/LRUCache.py` & `datastax-0.4.2/datastax/Lists/LRUCache.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 The functions get and put must each run in O(1) average time complexity.
 
 LRU -> Least Recently used
 """
 from typing import Any
 
 from datastax.Lists.DoublyLinkedList import DoublyLinkedList
-from datastax.Lists.DoublyNode import DoublyNode
+from datastax.Nodes import DoublyNode
 
 
 class LRUCache(DoublyLinkedList):
     def __init__(self, capacity: int):
         super().__init__()
         self._capacity = capacity
         self._cache: dict[int, DoublyNode] = {}
```

### Comparing `datastax-0.4.1/datastax/Lists/LinkedList.py` & `datastax-0.4.2/datastax/Lists/LinkedList.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 from typing import Any, Optional, Iterable, Self
+from datastax.Nodes import Node
+from datastax.Lists.AbstractLists import LinkedList as AbstractList
 
-from datastax.Lists.Node import Node
-from datastax.Lists.AbstractLists import LinkedList as AbstractLinkedList
 
-
-class LinkedList(AbstractLinkedList):
-    def __init__(
-            self,
-            items: Optional[Iterable[Any]] = None,
-            head: Optional[Node] = None,
-            tail: Optional[Node] = None
-    ):
+class LinkedList(AbstractList):
+    def __init__(self, items: Optional[Iterable] = None,
+                 head: Optional[Node] = None,
+                 tail: Optional[Node] = None):
         if head and tail:
             head.set_next(tail)
         self.set_head(head)
         self.set_tail(tail)
         if tail and not head:
             self.set_head(tail)
         self._construct(items if items else [])
 
-    def __iter__(self):
-        ref = self._head
-        while ref:
-            yield ref.data
-            ref = ref.next
-
     def set_head(self, head: Node | None):
         if head is None or isinstance(head, Node):
             self._head = head
             return
         raise TypeError("The 'head' parameter must be an "
                         "instance of Node or its subclass.")
 
     def set_tail(self, tail: Node | None):
         if tail is None or isinstance(tail, Node):
             self._tail = tail or self.head
             return
         raise TypeError("The 'tail' parameter must be an "
                         "instance of Node or its subclass.")
 
-    def _construct(self, items: Iterable[Any]) -> Self:
+    def _construct(self, items: Iterable) -> Self:
         for item in items:
             self.append(item)
         return self
 
     def append(self, data: Any) -> None:
         node = Node(data)
         if self.tail and not self.head:
```

### Comparing `datastax-0.4.1/datastax/Lists/Node.py` & `datastax-0.4.2/datastax/Nodes/Node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Any, Self, Optional
-
-from datastax.Lists.AbstractLists import Node as AbstractNode
+from datastax.Nodes.AbstractNodes import Node as AbstractNode
 
 
 class Node(AbstractNode):
     def __init__(self, data: Any,
                  _next: Optional[Self] = None):
         self.data = data
         self.set_next(_next)
 
-    def set_next(self, _next: Optional[Self] = None):
+    def set_next(self, _next: Optional[Self]):
         if _next is None or isinstance(_next, Node):
             self._next = _next
             return
         raise TypeError("The 'next' parameter must be an "
                         "instance of Node or its subclass.")
```

### Comparing `datastax-0.4.1/datastax/Lists/Queue.py` & `datastax-0.4.2/datastax/Lists/Queue.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Queue implementation using LinkedList
-
 from sys import maxsize
 from typing import Any, Optional, Sequence, Self
-from datastax.Lists.Node import Node
-from datastax.errors import OverFlowError, UnderFlowError
+from datastax.Nodes import Node
+from datastax.Utils.Exceptions import OverflowException, UnderflowException
 from datastax.Lists.LinkedList import LinkedList
 from datastax.Lists.AbstractLists import Queue as AbstractQueue
 
 
-class Queue(AbstractQueue, LinkedList):
+class Queue(LinkedList, AbstractQueue):
     def __init__(self, capacity: Optional[int] = None,
                  items: Optional[list] = None):
         super().__init__()
         self._rear = 0
         self.set_capacity(capacity)
         self._build(items if items else [])
 
@@ -36,30 +34,36 @@
                             "instance of int or its subclass.")
         if capacity < 0:
             raise ValueError("Capacity can't be negative")
         self._capacity = capacity
 
     def enqueue(self, data: Any) -> int:
         if self.is_full():
-            raise OverFlowError(self)
+            raise OverflowException(self)
         node = Node(data)
         if not self.head:
             self.set_head(node)
         else:
             self.tail.set_next(node)
         self.set_tail(node)
         self._rear += 1
         return 0
 
     def dequeue(self) -> Any:
         if self.is_empty():
-            raise UnderFlowError(self)
+            raise UnderflowException(self)
         deleted_node = self.head
         deleted_item = deleted_node.data
         self.set_head(self.head.next)
         self._rear -= 1
         return deleted_item
 
     def peek(self) -> str | Optional[Any]:
         if self.is_empty():
             return "QUEUE EMPTY"
         return self._tail.data if self._tail else None
+
+    def append(self, data: Any) -> None:
+        raise NotImplementedError
+
+    def insert(self, data: Any) -> None:
+        raise NotImplementedError
```

### Comparing `datastax-0.4.1/datastax/trees/avl_tree.py` & `datastax-0.4.2/datastax/Trees/AVLTree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,117 +1,107 @@
-# AVL Tree Implementation (Also: Self Balancing Binary Tree)
-from __future__ import annotations
-
 import warnings
 from typing import Any, Optional
-
-from datastax.errors import DuplicateNodeWarning
-from datastax.trees.binary_search_tree import BinarySearchTree, TreeNode
-
-
-class AVLNode(TreeNode):
-    def __init__(self, data: Any,
-                 left: AVLNode = None,
-                 right: AVLNode = None):
-        super().__init__(data, left, right)
-        self.height = 1
+from datastax.Utils.Warnings import DuplicateNodeWarning
+from datastax.Trees.BinarySearchTree import BinarySearchTree
+from datastax.Nodes import AVLNode
 
 
 class AVLTree(BinarySearchTree):
-    def __init__(self, array: list[Any] = None, root=None):
-        self._root: Optional[AVLNode] = root
-        super().__init__(array, root)
+    def __init__(self, items: Optional[list] = None,
+                 root: Optional[AVLNode] = None):
+        self.set_root(root)
+        super().__init__(items, root)
 
     # Private helper method for insert function
-    def _place(self, parent: Optional[AVLNode], data) -> Optional[AVLNode]:
+    def _place(self, parent: AVLNode | None, data) -> AVLNode | None:
         if not parent:
             return AVLNode(data)
         if parent.data < data:
-            parent.right = self._place(parent.right, data)
+            parent.set_right(self._place(parent.right, data))
         elif data < parent.data:
-            parent.left = self._place(parent.left, data)
+            parent.set_left(self._place(parent.left, data))
         else:
             warnings.warn(
                 f"Insertion unsuccessful. Item '{data}' already exists "
                 "in AVLTree", DuplicateNodeWarning
             )
-        parent.height = 1 + max(
+        parent.set_height(1 + max(
             self.height(parent.left),
             self.height(parent.right)
-        )
+        ))
         # Balancing the tree
         return self._balance(parent)
 
     # Function to check balance factor of node
     def balance_factor(self, parent: Optional[AVLNode] = None) -> int:
         parent = parent or self.root
         if parent:
             return self.height(parent.left) - self.height(parent.right)
         return 0
 
     # Function to get height of a tree
     @staticmethod
-    def height(node: Optional[AVLNode]) -> int:
+    def height(node: AVLNode | None) -> int:
         return node.height if node else 0
 
     # Function to balance a node
-    def _balance(self, parent: Optional[AVLNode]) -> Optional[AVLNode]:
+    def _balance(self, parent: AVLNode | None) -> AVLNode | None:
         if not parent:
             return None
         balance_factor = self.balance_factor(parent)
         if balance_factor < -1:
             # Perform LL Rotation
             # if parent.right and parent.right.data < data:
             if parent.right and self.balance_factor(parent.right) <= 0:
                 return self._left_rotate(parent)
             # Perform RL Rotation
             else:
                 if parent.right:
-                    parent.right = self._right_rotate(parent.right)
+                    parent.set_right(self._right_rotate(parent.right))
                 return self._left_rotate(parent)
 
         if balance_factor > 1:
             # Perform RR Rotation
             # if parent.left and data < parent.left.data:
             if parent.left and self.balance_factor(parent.left) >= 0:
                 return self._right_rotate(parent)
             # Perform LR Rotation
             else:
                 if parent.left:
-                    parent.left = self._left_rotate(parent.left)
+                    parent.set_left(self._left_rotate(parent.left))
                 return self._right_rotate(parent)
         return parent
 
     # Private helper method of balance function to perform RR rotation
-    def _right_rotate(self, node: AVLNode) -> Optional[AVLNode]:
+    def _right_rotate(self, node: AVLNode) -> AVLNode | None:
         left = node.left
         if left:
             temp = left.right
-            left.right = node
-            node.left = temp
-            node.height = 1 + max(self.height(node.left),
-                                  self.height(node.right))
-            left.height = 1 + max(self.height(left.left),
-                                  self.height(left.right))
+            left.set_right(node)
+            node.set_left(temp)
+            node.set_height(1 + max(self.height(node.left),
+                                    self.height(node.right)))
+            left.set_height(1 + max(self.height(left.left),
+                                    self.height(left.right)))
         return left
 
     # Private helper method of balance function to perform LL rotation
-    def _left_rotate(self, node: AVLNode) -> Optional[AVLNode]:
+    def _left_rotate(self, node: AVLNode) -> AVLNode | None:
         right = node.right
         if right:
             temp = right.left
-            right.left = node
-            node.right = temp
-            node.height = 1 + max(self.height(node.left),
-                                  self.height(node.right))
-            right.height = 1 + max(self.height(right.left),
-                                   self.height(right.right))
+            right.set_left(node)
+            node.set_right(temp)
+            node.set_height(1 + max(self.height(node.left),
+                                    self.height(node.right)))
+            right.set_height(1 + max(self.height(right.left),
+                                     self.height(right.right)))
         return right
 
-    def _delete(self, root: Optional[AVLNode], item: Any) -> Optional[AVLNode]:
+    def _delete(self, root: AVLNode | None, item: Any) -> AVLNode | None:
         root = super()._delete(root, item)
         if root:
-            root.height = 1 + max(
+            root.set_height(1 + max(
                 self.height(root.left),
                 self.height(root.right)
-            )
+            ))
         return self._balance(root)
```

### Comparing `datastax-0.4.1/datastax/trees/binary_search_tree.py` & `datastax-0.4.2/datastax/Trees/BinarySearchTree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-# Binary Search Tree Implementation
-from __future__ import annotations
-
 import warnings
-from typing import Optional, Any
+from typing import Any, Optional, Self, Sequence
 
-from datastax.errors import (
+from datastax.Utils.Warnings import (
     DuplicateNodeWarning,
     DeletionFromEmptyTreeWarning,
     NodeNotFoundWarning
 )
-from datastax.trees.private_trees.binary_tree import BinaryTree, TreeNode
+from datastax.Nodes import TreeNode
+from datastax.Trees.BinaryTree import BinaryTree
 
 
 class BinarySearchTree(BinaryTree):
-
     def insert(self, data: Any) -> None:
         root = self.root
         if data is None:
             return
         result = self._place(root, data)
         if result:
-            self._root = result
+            self.set_root(result)
+
+    def _construct(self, items: Optional[Sequence] = None) -> Self | None:
+        if not items or items[0] is None:
+            return None
+        for item in items:
+            self.insert(item)
+        return self
 
     def search(self, data: Any):
         """
         Searches a node in log2(n) time complexity BinarySearch Algorithm
         :param data: Any type of content in BST to search
         :return: TreeNode if it is found else None
         """
@@ -53,17 +57,17 @@
         return result
 
     # Private helper function for inserting
     def _place(self, parent, data) -> Optional[TreeNode]:
         if not parent:
             return TreeNode(data)
         elif parent.data < data:
-            parent.right = self._place(parent.right, data)
+            parent.set_right(self._place(parent.right, data))
         elif parent.data > data:
-            parent.left = self._place(parent.left, data)
+            parent.set_left(self._place(parent.left, data))
         else:
             warnings.warn(
                 f"Insertion unsuccessful. Item '{data}' already exists "
                 "in Tree", DuplicateNodeWarning
             )
         return parent
 
@@ -83,19 +87,19 @@
                 return root.right
             # Node with only leftChild, replace with right_child
             if root.right is None:
                 return root.left
             # Node with both children, replace with inorder_predecessor
             predecessor = self.inorder_predecessor(root)
             root.data = predecessor.data
-            root.left = self._delete(root.left, root.data)
+            root.set_left(self._delete(root.left, root.data))
         elif item < root.data:
-            root.left = self._delete(root.left, item)
+            root.set_left(self._delete(root.left, item))
         elif root.data < item:
-            root.right = self._delete(root.right, item)
+            root.set_right(self._delete(root.right, item))
         return root
 
     def delete(self, data: Any = None) -> None:
         """
         Deletes a node which has the data and replaces with inorder predecessor
         :param data: An item corresponding to the node to be deleted
         :return: returns data if node is found else None and raises warning
@@ -108,8 +112,8 @@
             return
         if not self.search(data):
             warnings.warn(
                 "Deletion unsuccessful. Node was not found with current "
                 f"data '{data}'", NodeNotFoundWarning
             )
             return
-        self._root = self._delete(self.root, data)
+        self.set_root(self._delete(self.root, data))
```

### Comparing `datastax-0.4.1/datastax/trees/binary_tree.py` & `datastax-0.4.2/datastax/Trees/BinaryTree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,85 @@
-# Binary Tree Implementation
-from __future__ import annotations
-
 import warnings
-from typing import Any, Optional
-
-from datastax.errors import (
-    PathNotGivenError,
-    PathNotFoundError,
+from typing import Any, Optional, Self, Sequence
+from datastax.Utils.Exceptions import (
+    PathNotGivenException,
+    PathNotFoundException,
+)
+from datastax.Utils.Warnings import (
     PathAlreadyOccupiedWarning,
     NodeNotFoundWarning,
     DeletionFromEmptyTreeWarning,
 )
 from datastax.Lists import Queue
-from datastax.trees.private_trees import binary_tree
-from datastax.trees.private_trees.binary_tree import TreeNode
+from datastax.Nodes import TreeNode
+from datastax.Trees.AbstractTrees import BinaryTree as AbstractTree
 
 
-class BinaryTree(binary_tree.BinaryTree):
-    def insert_path(self, data: Any, path: list[str] = None) -> None:
+class BinaryTree(AbstractTree):
+    def __init__(self, items: Optional[Sequence] = None,
+                 root: Optional[TreeNode] = None):
+        self.set_root(root)
+        self._construct(items)
+        self._string: Optional[str] = None
+
+    def set_root(self, root: TreeNode | None):
+        if root is None or isinstance(root, TreeNode):
+            self._root = root
+            return
+        raise TypeError("The 'root' parameter must be an "
+                        "instance of TreeNode or its subclass.")
+
+    def insert_path(self, data: Any, path: Optional[list[str]] = None) -> None:
         node = TreeNode(data)
         if not self._root:
             self._root = node
             return
         if not path:
-            raise PathNotGivenError(self)
+            raise PathNotGivenException(self)
         parent = self._root
         for direction in path[:-1]:  # Reaching
             if direction == 'left' and parent.left:
                 parent = parent.left
             elif direction == 'right' and parent.right:
                 parent = parent.right
             else:
-                raise PathNotFoundError(self)
+                raise PathNotFoundException(self)
         if path[-1] == 'right' and not parent.right:
-            parent.right = node
+            parent.set_right(node)
         elif path[-1] == 'left' and not parent.left:
-            parent.left = node
+            parent.set_left(node)
         else:
             occupied_node = parent.left if path[-1] == 'left' else parent.right
             warnings.warn("Insertion unsuccessful. Path already occupied by "
                           f"TreeNode [{occupied_node.data}]",
                           PathAlreadyOccupiedWarning)
 
     # Helper function to construct tree by level order -> Array to tree
-    def _construct(self, array: list[Any] = None) -> Optional[BinaryTree]:
-        if not array or array[0] is None:
+    def _construct(self, items: Optional[Sequence] = None) -> Self | None:
+        if not items or items[0] is None:
             return None
 
-        queue = Queue(capacity=len(array))
+        queue = Queue(capacity=len(items))
         current = 0
         root = self.root
         if not root:
-            root = TreeNode(array[0])
+            root = TreeNode(items[0])
             current = 1
         queue.enqueue(root)
-        while not queue.is_empty() and current < len(array):
+        while not queue.is_empty() and current < len(items):
             node = queue.dequeue()
-            node.left = None if array[current] is None else TreeNode(
-                array[current])
+            node.set_left(None if items[current] is None else TreeNode(
+                items[current]))
             if node.left:
                 queue.enqueue(node.left)  # Inserting Left Node
             current += 1
-            if current >= len(array):
+            if current >= len(items):
                 break
-            node.right = None if array[current] is None else TreeNode(
-                array[current])
+            node.set_right(None if items[current] is None else TreeNode(
+                items[current]))
             if node.right:
                 queue.enqueue(node.right)  # Inserting Right Node
             current += 1
         self._root = root
         return self
 
     def delete(self, data: Any = None) -> Optional[Any]:
@@ -125,41 +136,40 @@
                 if not any([node.right.left, node.right.right]):
                     parent = node
 
         data = None
         if parent:
             if parent.right:
                 data = parent.right.data
-                parent.right = None
+                parent.set_right(None)
             else:
                 data = parent.left.data
-                parent.left = None
+                parent.set_left(None)
         elif self._root:
             data = self._root.data
-            self._root = None
+            self.set_root(None)
         else:
             warnings.warn(
                 "Deletion Unsuccessful. Can't delete from empty Tree",
                 DeletionFromEmptyTreeWarning
             )
         return data
 
-    def insert(self, item: Any):
-
+    def insert(self, item: Any) -> None:
         temp = None if item is None else TreeNode(item)
         queue = Queue(capacity=len(self.array_repr))
         if self.root:
             queue.enqueue(self.root)
         while not queue.is_empty():
             node = queue.dequeue()
             if node.left:
                 queue.enqueue(node.left)
             else:
-                node.left = temp
+                node.set_left(temp)
                 return
             if node.right:
                 queue.enqueue(node.right)
             else:
-                node.right = temp
+                node.set_right(temp)
                 return
         else:
             self._root = temp
```

### Comparing `datastax-0.4.1/datastax/trees/fibonacci_tree.py` & `datastax-0.4.2/datastax/Trees/FibonacciTree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-# Fibonacci Tree Implementation
-from __future__ import annotations
-
-from typing import Optional, Any
-
-from datastax.trees.private_trees.binary_tree import BinaryTree, TreeNode
+from typing import Any, Optional, Self, Sequence
+from datastax.Trees.BinaryTree import BinaryTree
+from datastax.Nodes import TreeNode
 
 
 class FibonacciTree(BinaryTree):
-    def __init__(self, nth: int = None):
-        self._n = nth
+    _terms: Optional[int] = None
+    _series: Optional[list] = None
+
+    def __init__(self, terms: int):
+        self._terms = terms
         self._series = None
-        super().__init__(nth)
+        super().__init__([terms])
+
+    @property
+    def terms(self):
+        return self._terms
 
     @property
     def series(self):
         self._series = []
         first, second = 0, 1
-        if self._n == 0:
+        if self._terms == 0:
             self._series.append(first)
-        elif self._n == 1:
+        elif self._terms == 1:
             self._series.append(first)
             self._series.append(second)
         else:
             count = 0
-            while count < self._n + 1:
+            while count < self._terms + 1:
                 self._series.append(first)
                 first, second = second, first + second
                 count += 1
         return self._series
 
-    def _construct(self, n: int = None) -> Optional[FibonacciTree]:
-        if n is None or n < 0:
+    def _construct(self, items: Optional[Sequence] = None) -> Optional[Self]:
+        print(not items, items)
+        if not items or items[0] <= 0:
             return None
-
+        n = items[0]
         self._root = self._fibonacci(n)
         return self
 
     def _fibonacci(self, n: int,
-                   memo: dict[int, TreeNode] = None) -> TreeNode:
+                   memo: Optional[dict[int, TreeNode]] = None) -> TreeNode:
         if memo is None:
             memo = {0: TreeNode(0), 1: TreeNode(1)}
         if n in memo:
             return memo[n]
 
         left, right = self._fibonacci(n - 1), self._fibonacci(n - 2, memo)
         memo[n] = TreeNode(left.data + right.data, left, right)
         return memo[n]
 
     def insert(self, item: Any):
         raise NotImplementedError
+
+    def insert_path(self, data: Any, path: Optional[list[str]] = None) -> None:
+        raise NotImplementedError
```

### Comparing `datastax-0.4.1/datastax/trees/heap_tree.py` & `datastax-0.4.2/datastax/Trees/HeapTree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,113 @@
-# Heap Tree Implementation
-from __future__ import annotations
-
 import warnings
-from typing import Optional, Any
+from typing import Any, Optional, Self, Sequence
 
-from datastax.errors import DeletionFromEmptyTreeWarning
-from datastax.trees.private_trees.binary_tree import BinaryTree, TreeNode
+from datastax.Utils.Warnings import DeletionFromEmptyTreeWarning
+from datastax.Trees.BinaryTree import BinaryTree
+from datastax.Nodes import HeapNode
 
 
-class HeapNode(TreeNode):
-    def __init__(self, data: Any,
-                 left: HeapNode = None,
-                 right: HeapNode = None):
-        super().__init__(data, left, right)
-        self.parent: Optional[HeapNode] = None
-        self.prev_leaf: Optional[HeapNode] = None
+class HeapTree(BinaryTree):
+    _leaf: Optional[HeapNode]
 
+    def __init__(self, items: Optional[list] = None,
+                 root: Optional[HeapNode] = None):
+        self.set_root(root)
+        self.set_leaf(root)
+        super().__init__(items, root)
 
-class HeapTree(BinaryTree):
-    def __init__(self, array: list[Any] = None, root: HeapNode = None):
-        self._root: Optional[HeapNode] = root
-        self._leaf: Optional[HeapNode] = root
-        super().__init__(array, root)
+    @property
+    def leaf(self):
+        return self._leaf
+
+    def set_leaf(self, leaf: HeapNode | None):
+        if leaf is None or isinstance(leaf, HeapNode):
+            self._leaf = leaf
+            return
+        raise TypeError("The 'leaf' parameter must be an "
+                        "instance of HeapNode or its subclass.")
 
-    def _construct(self, array: list[Any] = None) -> Optional[HeapTree]:
-        if not array or array[0] is None:
+    def _construct(self, items: Optional[Sequence] = None) -> Self | None:
+        if not items or items[0] is None:
             return None
-        for item in array:
+
+        for item in items:
             try:
                 self.heappush(item)
             except TypeError as error:
                 raise error
         return self
 
-    @property
-    def leaf(self):
-        return self._leaf
-
     # Function to push an element inside a tree
     def heappush(self, data: Any) -> None:
         root = self.root
         if data is None:
             return
         node = HeapNode(data)
         if root is None:  # Heap Tree is Empty
-            self._root = self._leaf = node
+            self.set_root(node)
+            self.set_leaf(node)
         # Heap tree has nodes. So inserting new node
         # in the left of leftmost leaf node
         elif self.leaf and self.leaf.left is None:
-            self.leaf.left = node
-            node.parent = self.leaf
+            self.leaf.set_left(node)
+            node.set_parent(self.leaf)
         else:
             if not self.leaf:
                 return
-            self.leaf.right = node
+            self.leaf.set_right(node)
             previous_leaf = self.leaf
-            node.parent = self.leaf
+            node.set_parent(previous_leaf)
             self._update_leaf(self.leaf)
-            self.leaf.prev_leaf = previous_leaf
+            self.leaf.set_prev_leaf(previous_leaf)
         self._heapify(node)
 
     # Private function to convert a subtree to heap
     def _heapify(self, node: HeapNode) -> None:
         if node.parent and node.parent.data < node.data:
             node.parent.data, node.data = node.data, node.parent.data
             self._heapify(node.parent)
 
     # Private Helper method of heappush function to
-    # update rightmost node in deepest level
+    # update rightmost node in the deepest level
     def _update_leaf(self, node: HeapNode) -> None:
         # reach extreme left of next level if current level is full
         if node.parent is None:
-            self._leaf = node
+            self.set_leaf(node)
         elif node.parent.left is node:
-            self._leaf = node.parent.right
+            self.set_leaf(node.parent.right)
         elif node.parent.right is node:
             self._update_leaf(node.parent)
         while self.leaf and self.leaf.left:
-            self._leaf = self.leaf.left
+            self.set_leaf(self.leaf.left)
 
     # Function to pop the largest element in the tree
     def heappop(self) -> Optional[Any]:
         if not self.root:
             warnings.warn(
                 "Deletion Unsuccessful. Can't delete when"
                 "tree is Already Empty", DeletionFromEmptyTreeWarning
             )
             return None
         deleted_data = self.root.data
         if self.root is self.leaf and not any(
                 [self.leaf.left, self.leaf.right]):
-            self._root = self._leaf = None
-
+            self.set_root(None)
+            self.set_leaf(None)
         else:
             if self.leaf.right and self.root:
                 self.root.data = self.leaf.right.data
-                self.leaf.right = None
+                self.leaf.set_right(None)
                 self._shift_up(self.root)
             elif self.leaf.left and self.root:
                 self.root.data = self.leaf.left.data
-                self.leaf.left = None
+                self.leaf.set_left(None)
                 self._shift_up(self.root)
             else:  # We have reached the end of a level
-                self._leaf = self.leaf.prev_leaf
+                self.set_leaf(self.leaf.prev_leaf)
                 return self.heappop()
         return deleted_data
 
     # Private helper method of heappop function
     def _shift_up(self, node: HeapNode) -> None:
         root = node
         left_child = root.left
```

### Comparing `datastax-0.4.1/datastax/trees/huffman_tree.py` & `datastax-0.4.2/datastax/Trees/HuffmanTree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-# Implementation of Variable size Huffman Coding Tree
-from __future__ import annotations
-
 from collections import Counter
-from typing import Any, Optional, Union
-
+from typing import Any, Optional, Self, Sequence
 from datastax.Arrays import PriorityQueue
-from datastax.trees.private_trees import huffman_tree
-from datastax.trees.private_trees.huffman_tree import HuffmanNode
+from datastax.Nodes import HuffmanNode
+from datastax.Tables import HuffmanTable
+from datastax.Trees.BinaryTree import BinaryTree
+from datastax.Trees.AbstractTrees import HuffmanTree as AbstractTree
 
 
-class HuffmanTable(huffman_tree.HuffmanTable):
-    def _calculate_size(self):
-        size = 0
-        for char, huff_code in self.data.items():
-            size += ord(char).bit_length() + len(huff_code)
-        self._size = size
-
-
-class HuffmanTree(huffman_tree.HuffmanTree):
-    def _construct(self, data: Union[list[str], str] = None
-                   ) -> Optional[HuffmanTree]:
-        if not data or data[0] is None:
+class HuffmanTree(BinaryTree, AbstractTree):
+    def __init__(self, data: Optional[Sequence] = None):
+        self.data = data
+        super().__init__(data)
+
+    def _construct(self,
+                   items: Optional[Sequence] = None) -> Self | None:
+        if not items or items[0] is None:
             return None
 
         def comparator(n1: HuffmanNode, n2: HuffmanNode) -> HuffmanNode:
             if n1.frequency > n2.frequency:
                 return n2
             return n1
 
         nodes = (
             HuffmanNode(
-                _data, None, None, frequency
-            ) for _data, frequency in Counter(data).items()
+                data, None, None, frequency
+            ) for data, frequency in Counter(items).items()
         )
         p_queue = PriorityQueue(capacity=None, custom_comparator=comparator)
         for node in nodes:
             p_queue.enqueue(node)
 
         while len(p_queue.array) >= 2:
             node1 = p_queue.dequeue()
             node2 = p_queue.dequeue()
             root_freq = sum((node1.frequency, node2.frequency))
             root = HuffmanNode(None, node1, node2, root_freq)
             p_queue.enqueue(root)
-
-        self._root = p_queue.dequeue()
+        self.set_root(p_queue.dequeue())
         self._calculate_huffman_code()
         self._create_huffman_table()
         return self
 
-    def huffman_code_of(self, character: str) -> Optional[str]:
+    def huffman_code_of(self, character: str) -> str | None:
         def find(node: HuffmanNode, path=None):
             if not node:
                 return None
             path = path or []
             if node.data == character:
                 return path
             path.append(0)
@@ -67,57 +60,57 @@
 
         result = find(self.root)
         return ''.join(map(str, result)) if result else None
 
     # Private method to build data dictionary for HuffmanTable
     def _create_huffman_table(self):
         items = {}
-        for item in self._data:
+        for item in self.data:
             items[item] = self.huffman_code_of(item)
-        self._table = HuffmanTable(items, Counter(self._data))
+        self._table = HuffmanTable(items, Counter(self.data))
 
     def _calculate_huffman_code(self):
         self._huffman_code = ''.join(
-            self.huffman_code_of(character) for character in self._data
+            self.huffman_code_of(character) for character in self.data
         )
         pass
 
-    def size_calculator(self) -> Optional[tuple[int, int]]:
+    def size_calculator(self) -> tuple[int, int] | None:
         """
         Calculates the actual encoding size and total
         huffman encoding size with table included
         """
         if not self.root or not self.huffman_table:
             return None
         fixed_encoding = huffman_encoding = 0
-        frequency = self.huffman_table.frequency
+        frequencies = self.huffman_table.frequencies
 
         for char, huff_code in self.huffman_table.data.items():
             # Converting item to ascii finding bit_length and multiplying
             # it with frequency
-            total_bit_length = ord(char).bit_length() * frequency[char]
+            total_bit_length = ord(char).bit_length() * frequencies[char]
             fixed_encoding += total_bit_length  # Adding to fixed_encoding
 
             # Already in Binary so no conversion to ascii
-            total_bit_length = len(huff_code) * frequency[char]
+            total_bit_length = len(huff_code) * frequencies[char]
             huffman_encoding += total_bit_length  # Adding to huffman_encoding
 
         return fixed_encoding, huffman_encoding + self.huffman_table.size
 
-    def compression_ratio(self) -> Optional[str]:
+    def compression_ratio(self) -> str | None:
         if not self.root:
             return None
         result = self.size_calculator()
         if not result:
             return None
         fixed_encoding, huffman_encoding = result
         compression_ratio = huffman_encoding / fixed_encoding
         return f"{compression_ratio :.2%}"
 
-    def space_saved(self) -> Optional[str]:
+    def space_saved(self) -> str | None:
         if not self.root:
             return None
         result = self.size_calculator()
         if not result:
             return None
         fixed_encoding, huffman_encoding = result
         space_saved = (fixed_encoding - huffman_encoding) / fixed_encoding
```

### Comparing `datastax-0.4.1/datastax/trees/min_heap_tree.py` & `datastax-0.4.2/datastax/Trees/MinHeapTree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Min Heap Tree Implementation
-from __future__ import annotations
-
-from datastax.trees.heap_tree import HeapTree, HeapNode
+from datastax.Trees.HeapTree import HeapTree
+from datastax.Nodes import HeapNode
 
 
 class MinHeapTree(HeapTree):
     def _heapify(self, node: HeapNode) -> None:
         if node.parent and node.parent.data > node.data:
             node.parent.data, node.data = node.data, node.parent.data
             self._heapify(node.parent)
```

### Comparing `datastax-0.4.1/datastax/trees/min_segment_tree.py` & `datastax-0.4.2/datastax/Trees/MinSegmentTree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# Min Segment Tree implementation
-from __future__ import annotations
-
 from sys import maxsize
-from typing import Any, Optional
-
-from datastax.trees.private_trees.segment_tree import SegmentTree, SegmentNode
+from typing import Optional, Self, Sequence
+from datastax.Trees.SegmentTree import SegmentTree
+from datastax.Nodes import SegmentNode
 
 
 class MinSegmentTree(SegmentTree):
-    def __init__(self, array=None, root=None):
-        self._lazy_tree = SegmentTree()
-        super().__init__(array, root)
+    _lazy_tree = SegmentTree()
 
-    def insert(self, item: Any):
-        raise NotImplementedError
+    def __init__(self, item: Optional[Sequence] = None,
+                 root: Optional[SegmentNode] = None):
+        super().__init__(item, root)
 
     @property
     def lazy_tree(self):
         return self._lazy_tree
 
-    def _construct(self, array: list[int] = None) -> Optional[MinSegmentTree]:
+    def _construct(self, array: Optional[Sequence] = None) -> Self | None:
         if not array or array[0] is None:
             return None
 
-        def build(left: int, right: int) -> tuple[SegmentNode, ...]:
+        def build(left: int, right: int) -> tuple[SegmentNode, SegmentNode]:
             node, lazy_node = SegmentNode(None), SegmentNode(maxsize)
             # Leaf Node
             if array and left == right:
                 node.left_index, node.right_index = left, right
+                lazy_node.left_index, lazy_node.right_index = left, right
                 node.data = array[left]
                 return node, lazy_node
             # Intermediate Node
             mid = (left + right) // 2
-            node.left, lazy_node.left = build(left, mid)
-            node.right, lazy_node.right = build(mid + 1, right)
+            left_node, lazy_left_node = build(left, mid)
+            right_node, lazy_right_node = build(mid + 1, right)
+            node.set_left(left_node), lazy_node.set_left(lazy_left_node)
+            node.set_right(right_node), lazy_node.set_right(lazy_right_node)
             node.left_index = lazy_node.left_index = node.left.left_index
             node.right_index = lazy_node.right_index = node.right.right_index
             node.data = min(node.left.data, node.right.data)
             return node, lazy_node
 
-        self._root, self._lazy_tree._root = build(0, len(array) - 1)
+        root, lazy_root = build(0, len(array) - 1)
+        self.set_root(root), self.lazy_tree.set_root(lazy_root)
         return self
 
     @staticmethod
     def _perform_lazy_update(root: SegmentNode, lazy_node: SegmentNode,
                              start: int, end: int, nodes: int) -> None:
         # has lazy values, needs to be propagated
         if lazy_node.data != maxsize:
             root.data = lazy_node.data
             if start != end:
                 lazy_node.left.data = lazy_node.right.data = root.data
             # No longer a lazy node
             lazy_node.data = maxsize
 
-    def get_min(self, left: int, right: int,
-                root: SegmentNode = None,
-                lazy_node: SegmentNode = None) -> int:
-        if not root:
-            root = self.root
-            lazy_node = self.lazy_tree.root
+    def get_min(self, left: int, right: int) -> int:
+        return self.get_range(left, right, self.root, self.lazy_tree.root)
+
+    def get_range(self, left: int, right: int,
+                  root: SegmentNode | None,
+                  lazy_node: SegmentNode | None) -> int:
         if not root or not lazy_node:
             return maxsize
 
         start, end = root.left_index, root.right_index
         nodes = end - start + 1
 
         # perform lazy update
@@ -72,33 +72,18 @@
         if end < left or start > right or end < start:
             return maxsize
 
         if root.left_index >= left and root.right_index <= right:
             return root.data
 
         return min(
-            self.get_min(left, right, root.left, lazy_node.left),
-            self.get_min(left, right, root.right, lazy_node.right)
+            self.get_range(left, right, root.left, lazy_node.left),
+            self.get_range(left, right, root.right, lazy_node.right)
         )
 
-    def update_at_index(self, index: int, data: int):
-        if not self.root:
-            return None
-
-        def update(node: SegmentNode, new):
-            if index == node.left_index == node.right_index:
-                node.data = new
-            mid = (node.left_index + node.right_index) // 2
-            update_node = node.left if index <= mid else node.right
-            update(update_node, new)
-            node.data = min(node.left.data if node.left else node.data,
-                            node.right.data if node.right else node.data)
-
-        update(self.root, data)
-
     def update_at_range(self, left: int, right: int, data: int) -> None:
         if not self.root:
             return None
 
         def update(node: SegmentNode, lazy_node: SegmentNode) -> None:
             # How many leaf node values to propagate
             start, end = node.left_index, node.right_index
@@ -122,21 +107,34 @@
             # location is partially in bounds
             update(node.left, lazy_node.left)
             update(node.right, lazy_node.right)
             node.data = min(node.left.data, node.right.data)
 
         update(self.root, self.lazy_tree.root)
 
+    def update_at_index(self, index: int, data: int) -> None:
+        if not self.root:
+            return None
+
+        def update(node: SegmentNode, new: int):
+            if index == node.left_index == node.right_index:
+                node.data = new
+            mid = (node.left_index + node.right_index) // 2
+            update_node = node.left if index <= mid else node.right
+            update(update_node, new)
+            node.data = min(node.left.data if node.left else node.data,
+                            node.right.data if node.right else node.data)
+
+        update(self.root, data)
+
 
 if __name__ == '__main__':
     tree = MinSegmentTree([2, 3, 1, 4, 2, 5, 2, 3, 1, 5])
     # tree = MinSegmentTree()
     print(tree)
     tree.update_at_range(3, 9, -5)
     print(tree)
     tree.update_at_range(5, 8, +3)
     print(tree.get_min(3, 5))
     print(tree)
     print(tree.lazy_tree)
     print(tree.segment_array)
-    print(tree)
-    print(tree.lazy_tree)
```

### Comparing `datastax-0.4.1/datastax/trees/private_trees/binary_tree.py` & `datastax-0.4.2/datastax/Trees/AbstractTrees/HuffmanTree.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,51 @@
-# Private module to separate print logic from main logic of BinaryTree
-from __future__ import annotations
-
 import math
-from typing import Any, Optional
-
-from datastax.Lists import Queue
-
-
-def _node_builder(data: Optional[str], piece_width: int) -> str:
-    value: str = data or ''
-    gap1 = int(math.ceil(piece_width / 2 - len(value) / 2))
-    gap2 = int(math.floor(piece_width / 2 - len(value) / 2))
-    return f"{' ' * gap1}{value}{' ' * gap2}"
-
-
-# private method to mangle string __repr__
-def _mangled(item: Any) -> str:
-    if '\n' in str(item):
-        return f"{str(type(item))[8:-2].split('.')[-1]}@{id(item)}"
-    return str(item)
-
-
-class TreeNode:
-    def __init__(self, data: Any,
-                 left=None,
-                 right=None) -> None:
-        self.left = left
-        self.data = data
-        self.right = right
-
-    def __str__(self):
-        values = [self.data,
-                  self.left.data if self.left else None,
-                  self.right.data if self.right else None]
-        values = list(
-            map(lambda value: "" if value is None else _mangled(value), values)
-        )
-        max_width = max(len(_mangled(data)) for data in values if data)
-        if max_width % 2:
-            max_width += 1  # To make max_width even
-
-        "Building string from calculated values"
-        per_piece = 2 * (max_width + 4)
-        string_builder = f"{_node_builder(values[0], per_piece)}\n"
-        per_piece //= 2
-        hpw = int(per_piece // 2 - 1)
-        if any(values[1:]):
-            if all(values[1:]):
-                string_builder += (
-                    f"{' ' * (hpw + 1)}"
-                    f"┌{'─' * hpw}┴{'─' * hpw}┐\n"
-                )
-                string_builder += _node_builder(
-                    values[1], per_piece
-                ) + _node_builder(values[2], per_piece)
-            elif values[1]:
-                string_builder += f"{' ' * (hpw + 1)}┌{'─' * hpw}┘\n"
-                string_builder += _node_builder(values[1], per_piece)
-            else:
-                string_builder += f"{' ' * (per_piece - 1)} └{'─' * hpw}┐\n"
-                string_builder += (
-                    f"{' ' * (per_piece - 1)} "
-                    f"{_node_builder(values[2], per_piece)}"
-                )
+from typing import Optional
+from abc import ABC as AbstractClass, abstractmethod
+from datastax.Utils import Commons
+from datastax.Nodes import HuffmanNode
+from datastax.Tables import HuffmanTable
+from datastax.Trees.AbstractTrees.BinaryTree import BinaryTree
 
-        return string_builder
-
-    def preorder_print(self) -> str:
-        values = [self.data, self.left.data if self.left else None,
-                  self.right.data if self.right else None]
-        values = list(
-            map(lambda value: "" if value is None else _mangled(value), values)
-        )
 
-        string_builder = f'{values[0]}\n'
-        if any(values[1:]):
-            if all(values[1:]):
-                string_builder += f"├─▶ {values[1]}\n"
-                string_builder += f"└─▶ {values[2]}"
-            else:
-                string_builder += f"└─▶ {values[1] or values[2]}"
-
-        return string_builder
-
-    def __repr__(self):
-        return self.__str__()
-
-
-class BinaryTree:
-    def __init__(self, array=None, root=None):
-        self._root = root
-        self._construct(array)
-        self._string: Optional[str] = None
+class HuffmanTree(BinaryTree, AbstractClass):
+    _data: Optional[list[str] | str]
+    _table: Optional[HuffmanTable] = None
+    _huffman_code = ""
 
     @property
-    def root(self):
-        return self._root
+    def huffman_table(self):
+        return self._table
 
-    def _construct(self, array=None):
-        if not array or array[0] is None:
-            return None
-        for item in array:
-            try:
-                self.insert(item)
-            except TypeError as error:
-                raise error
-        return self
-
-    def insert(self, item: Any):
-        raise NotImplementedError
-
-    @property  # Level Order Traversal -> Tree to array
-    def array_repr(self) -> list[Any]:
-        array = []
-        queue = Queue()
-        if self.root:
-            queue.enqueue(self.root)
-        while not queue.is_empty():
-            node = queue.dequeue()
-            array.append(node.data)
-            if node.left:
-                queue.enqueue(node.left)
-            if node.right:
-                queue.enqueue(node.right)
-
-        return array
+    @property
+    def huffman_code(self):
+        return self._huffman_code
 
     # Level order Traversal of Tree
     def __str__(self):  # noqa: C901
         root = self.root
         if not root:
             return "  NULL"
 
-        lines: list[list[Optional[str]]] = []
-        level: list[Optional[TreeNode]] = [root]
-        nodes: int = 1
-        max_width: int = 0
+        lines = []
+        level = [root]
+        nodes = 1
+        max_width = 0
         while nodes:
-            line: list[Optional[str]] = []
-            next_level: list[Optional[TreeNode]] = []
+            line = []
+            next_level = []
             nodes = 0
             for node in level:
                 if node:
-                    data = _mangled(node.data)
+                    data = Commons.repr(node.data or node.frequency)
+                    frequency = "│"
+                    if not any([node.left, node.right]):
+                        frequency = f"{node.frequency}"
                     max_width = max(len(data), max_width)
-                    line.append(data)
+                    line.append([data, frequency])
                     next_level += [node.left, node.right]
                     if node.left:
                         nodes += 1
                     if node.right:
                         nodes += 1
                     continue
                 line.append(None)
@@ -156,65 +53,123 @@
             if max_width % 2:
                 max_width += 1
             lines.append(line)
             level = next_level
         ##################################################################
         "Building string from calculated values"
         per_piece = len(lines[-1]) * (max_width + 4)
-
-        string_builder = f"{_node_builder(lines[0][0], per_piece)}\n"
+        string_builder = f"{Commons.node_builder(lines[0][0][0], per_piece)}\n"
+        string_builder += Commons.node_builder("   0", per_piece // 2)
+        string_builder = (
+            f"{string_builder[:]}" f"{Commons.node_builder(lines[0][0][1], 1)}"
+        )
+        string_builder += (
+                Commons.node_builder("1   ", per_piece // 2 - 1) + "\n"
+        )
         per_piece //= 2
         for _, line in enumerate(lines[1:], 1):
             hpw = int(math.floor(per_piece / 2) - 1)
             # Printing ┌ ┴ ┐ or ┌ ─ ┘ or └ ─ ┐ components
             for j, value in enumerate(line):
                 string_builder += (
-                    ('┴' if value else '┘') if line[j - 1] else (
-                        '└' if value else ' ')) if j % 2 else ' '
+                    (
+                        ("┴" if value else "┘")
+                        if line[j - 1]
+                        else ("└" if value else " ")
+                    )
+                    if j % 2
+                    else " "
+                )
 
                 if not value:
-                    string_builder += ' ' * (per_piece - 1)
+                    string_builder += " " * (per_piece - 1)
                     continue
                 if j % 2:
                     string_builder += f"{'─' * hpw}┐{' ' * hpw}"
                 else:
                     string_builder += f"{' ' * hpw}┌{'─' * hpw}"
-            string_builder += '\n'
+            string_builder += "\n"
 
             # Printing the value of each Node
             for value in line:
-                string_builder += _node_builder(value, per_piece)
-            string_builder += '\n'
+                value = value[0] if value else value
+                string_builder += Commons.node_builder(value, per_piece)
+            string_builder += "\n"
+            for value in line:
+                internal = value and value[1] == "│"
+                if internal:
+                    string_builder += (
+                        Commons.node_builder("   0", per_piece // 2)
+                    )
+                data = f"{value[1]}" if value else value
+                piece_width = 1 if internal else per_piece
+                string_builder = (
+                    f"{string_builder[:] if internal else string_builder}"
+                    f"{Commons.node_builder(data, piece_width)}"
+                )
+                if value and value[1] == "│":
+                    string_builder += (
+                        Commons.node_builder("1   ", per_piece // 2 - 1)
+                    )
+
+            string_builder += "\n"
             per_piece //= 2
 
         return string_builder
 
     # Pre Order Traversal of Tree
     def preorder_print(self) -> None:
-        def string_builder(parent: Optional[TreeNode], has_right_child: bool,
-                           padding="", component="") -> None:
+        def string_builder(
+                parent: Optional[HuffmanNode],
+                has_right_child: bool,
+                padding="",
+                component="",
+        ) -> None:
             if not parent:
                 return
             if self._string is not None:
-                self._string += (
-                    f"\n{padding}{component}"
-                    f"{_mangled(parent.data)}"
-                )
+                self._string += f"\n{padding}{component}"
+                data = parent.data
+                if not data:
+                    data = parent.frequency
+                    self._string += str(data)
+                else:
+                    data = Commons.repr(data)
+                    self._string += f"{data} [{parent.frequency}]"
             if parent is not root:
                 padding += "│   " if has_right_child else "    "
             left_pointer = "├─▶ " if parent.right else "└─▶ "
             right_pointer = "└─▶ "
-            string_builder(parent.left, bool(parent.right), padding,
-                           left_pointer)
-            string_builder(parent.right, False, padding, right_pointer)
+            string_builder(parent.left, bool(parent.right),
+                           padding, left_pointer)
+            string_builder(parent.right, False,
+                           padding, right_pointer)
 
         root = self.root
         if not root:
             self._string = "NULL"
             print(self._string)
             return
         self._string = ""
         string_builder(root, bool(root.right))
         print(self._string)
 
-    def __repr__(self):
-        return self.__str__()
+    @abstractmethod
+    def huffman_code_of(self, character: str):
+        ...
+
+    @abstractmethod
+    def size_calculator(self):
+        ...
+
+    @abstractmethod
+    def compression_ratio(self):
+        ...
+
+    @abstractmethod
+    def space_saved(self):
+        ...
+
+    @staticmethod
+    @abstractmethod
+    def decode_from_table(huffman_code: str, huffman_table: dict) -> str:
+        ...
```

### Comparing `datastax-0.4.1/datastax/trees/private_trees/segment_tree.py` & `datastax-0.4.2/datastax/Trees/AbstractTrees/SegmentTree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,40 @@
-from __future__ import annotations
-
 import math
-from typing import Any, Optional
-
-from datastax.trees.private_trees.binary_tree import (
-    BinaryTree, TreeNode, _node_builder, _mangled
-)
-
-
-class SegmentNode(TreeNode):
-    def __init__(self, data: Any,
-                 left: SegmentNode = None,
-                 right: SegmentNode = None):
-        self.left_index = 0
-        self.right_index = 0
-        super().__init__(data, left, right)
+from typing import Optional
+from abc import ABC as AbstractClass, abstractmethod
+from datastax.Utils import Commons
+from datastax.Nodes import SegmentNode
+from datastax.Trees.AbstractTrees.BinaryTree import BinaryTree
 
 
-class SegmentTree(BinaryTree):
-    def insert(self, item: Any):
-        raise NotImplementedError
+class SegmentTree(BinaryTree, AbstractClass):
+    _segment_array: Optional[list]
 
     @property
     def segment_array(self):
-        segment_array = []
-        self._traverse_leafs(self.root, segment_array)
-        return segment_array
-
-    def _traverse_leafs(self, node, array):
-        if not node:
-            return
-        if not any((node.left, node.right)):
-            array.append(node.data)
-            return
-        # if left child is found, check for leaf node recursively
-        if node.left:
-            self._traverse_leafs(node.left, array)
-        # if right child is found, check for leaf node recursively
-        if node.right:
-            self._traverse_leafs(node.right, array)
+        self._segment_array = []
+        self._traverse_leafs(self.root)
+        return self._segment_array
 
     def __str__(self):  # noqa: C901
         root = self.root
         if not root:
             return "  NULL"
 
-        lines: list[list] = []
-        level: list[Optional[SegmentNode]] = [root]
-        nodes: int = 1
-        max_width: int = 0
+        lines = []
+        level = [root]
+        nodes = 1
+        max_width = 0
         while nodes:
-            line: list[Optional[list]] = []
-            next_level: list[Optional[SegmentNode]] = []
+            line = []
+            next_level = []
             nodes = 0
             for node in level:
                 if node:
-                    data = _mangled(node.data)
+                    data = Commons.repr(node.data)
                     _range = None
                     if node.left_index != node.right_index:
                         _range = f"[{node.left_index}:{node.right_index}]"
                     max_width = max(len(data), max_width)
                     line.append([data, _range])
                     next_level += [node.left, node.right]
                     if node.left:
@@ -73,16 +48,17 @@
                 max_width += 1
             lines.append(line)
             level = next_level
         ##################################################################
         "Building string from calculated values"
         per_piece = len(lines[-1]) * (max_width + 4)
 
-        string_builder = f"{_node_builder(lines[0][0][0], per_piece)}\n"
-        string_builder += f"{_node_builder(lines[0][0][1], per_piece)}\n"
+        string_builder = f"{Commons.node_builder(lines[0][0][0], per_piece)}\n"
+        string_builder += \
+            f"{Commons.node_builder(lines[0][0][1], per_piece)}\n"
         per_piece //= 2
         for _, line in enumerate(lines[1:], 1):
             hpw = int(math.floor(per_piece / 2) - 1)
             # Printing ┌ ┴ ┐ or ┌ ─ ┘ or └ ─ ┐ components
             for j, value in enumerate(line):
                 string_builder += (
                     ('┴' if value else '┘') if line[j - 1] else (
@@ -96,19 +72,19 @@
                 else:
                     string_builder += f"{' ' * hpw}┌{'─' * hpw}"
             string_builder += '\n'
 
             # Printing the value of each Node
             for value in line:
                 value = value[0] if value else value
-                string_builder += _node_builder(value, per_piece)
+                string_builder += Commons.node_builder(value, per_piece)
             string_builder += '\n'
             for value in line:
                 value = value[1] if value else value
-                string_builder += _node_builder(value, per_piece)
+                string_builder += Commons.node_builder(value, per_piece)
             string_builder += '\n'
 
             per_piece //= 2
 
         return string_builder
 
     def preorder_print(self) -> None:
@@ -116,15 +92,15 @@
                            has_right_child: bool,
                            padding="", component="") -> None:
             if not parent:
                 return
             if self._string is not None:
                 self._string += (
                     f"\n{padding}{component}"
-                    f"{_mangled(parent.data)} "
+                    f"{Commons.repr(parent.data)} "
                 )
                 if parent.left_index != parent.right_index:
                     self._string += (
                         f"[{parent.left_index}:{parent.right_index}]"
                     )
 
             if parent is not root:
@@ -138,7 +114,25 @@
         root = self.root
         if not root:
             print("NULL")
             return
         self._string = ""
         string_builder(root, bool(root.right))
         print(self._string)
+
+    @abstractmethod
+    def update_at_range(self, left: int, right: int, data: int) -> None:
+        ...
+
+    @abstractmethod
+    def update_at_index(self, index: int, data: int) -> None:
+        ...
+
+    @abstractmethod
+    def get_range(self, left: int, right: int,
+                  root: SegmentNode | None,
+                  lazy_node: SegmentNode | None):
+        ...
+
+    @abstractmethod
+    def _traverse_leafs(self, node: SegmentNode | None) -> None:
+        ...
```

### Comparing `datastax-0.4.1/datastax/trees/red_black_tree.py` & `datastax-0.4.2/datastax/Trees/RedBlackTree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# Implementation of Variable size Huffman Coding Tree
-from __future__ import annotations
-
 import warnings
 from typing import Optional, Any
+from datastax.Utils.Warnings import DuplicateNodeWarning
+from datastax.Utils import ColorCodes
+from datastax.Nodes import RedBlackNode
+from datastax.Trees.BinarySearchTree import BinarySearchTree
+from datastax.Trees.AbstractTrees import RedBlackTree as AbstractTree
 
-from datastax.errors import (
-    DuplicateNodeWarning
-)
-from datastax.trees.binary_search_tree import BinarySearchTree
-from datastax.trees.private_trees import red_black_tree
-from datastax.trees.private_trees.red_black_tree import (
-    RedBlackNode,
-    BLACK, RED
-)
+RED, BLACK = ColorCodes.RED, ColorCodes.BLACK
 
 
-class RedBlackTree(BinarySearchTree,
-                   red_black_tree.RedBlackTree):
+class RedBlackTree(BinarySearchTree, AbstractTree):
     # Private helper function for inserting
     def _place(self,
                parent: Optional[RedBlackNode],
                data) -> Optional[RedBlackNode]:
         node = RedBlackNode(data)
         parent = None
         search = self.root
@@ -33,211 +26,213 @@
             else:
                 warnings.warn(
                     f"Insertion unsuccessful. Item '{data}' already exists "
                     "in Tree", DuplicateNodeWarning
                 )
                 return None
 
-        node.parent = parent
+        node.set_parent(parent)
         # Node to be added is root node
         if not parent:
-            node.color = BLACK
+            node.set_color(BLACK)
             return node
         if parent.data > node.data:
-            parent.left = node
+            parent.set_left(node)
         else:
-            parent.right = node
+            parent.set_right(node)
         self._post_place(node)
         return self.root
 
     @staticmethod
     def sibling_of(node: Optional[RedBlackNode]):
         if not node or not node.parent:
             return None
         if node.parent.left is node:
             return node.parent.right
         return node.parent.left
 
     def _post_place(self, node: Optional[RedBlackNode]):
         if not node or node is self.root:
             return
-        # * Resolve Red Red Conflict
+        # * Resolve Red-Red Conflict
         parent = node.parent
         if parent and parent.color is RED:
             sibling = self.sibling_of(parent)
             # CASE 1: Recolor and move up to see if more work required.
             if sibling and sibling.color is RED:
-                parent.color = sibling.color = BLACK
+                parent.set_color(BLACK)
+                sibling.set_color(BLACK)
                 if parent.parent and parent.parent is not self.root:
-                    parent.parent.color = RED
+                    parent.parent.set_color(RED)
                     self._post_place(parent.parent)
             # CASE 2: Color is black so restructuring (rotations) and
             # recoloring both are required.
             else:
                 # CASE A: Parent is left child
                 if parent.parent and parent is parent.parent.left:
                     # CASE i: Perform RR Rotation
                     # Both node and parent are Left Child of G.Parent
                     if node is parent.right:
                         # CASE ii: Perform LR Rotation
                         # node is Right and parent is Left Child of G.Parent
                         parent = self._left_rotate(parent)
                     if parent and parent.parent:
-                        parent.color = BLACK
-                        parent.parent.color = RED
+                        parent.set_color(BLACK)
+                        parent.parent.set_color(RED)
                         self._right_rotate(parent.parent)
                 # CASE B: Parent is right child
                 else:
                     # CASE i: Perform LL Rotation
                     # Both node and parent are Right Child of G.Parent
                     if node is parent.left:
                         # CASE ii: Perform RL Rotation
                         # node is Left and parent is Right Child of G.Parent
                         parent = self._right_rotate(parent)
                     if parent and parent.parent:
-                        parent.color = BLACK
-                        parent.parent.color = RED
+                        parent.set_color(BLACK)
+                        parent.parent.set_color(RED)
                         self._left_rotate(parent.parent)
 
     # Private helper method of balance function to perform RR rotation
-    def _right_rotate(self, node: RedBlackNode) -> Optional[RedBlackNode]:
+    def _right_rotate(self, node: RedBlackNode) -> RedBlackNode:
         left = node.left
         if not left:
             return left
-        left.parent = node.parent
+        left.set_parent(node.parent)
 
-        node.left = left.right
+        node.set_left(left.right)
         if node.left:
-            node.left.parent = node
-        left.right = node
-        node.parent = left
+            node.left.set_parent(node)
+        left.set_right(node)
+        node.set_parent(left)
 
         if left.parent:
             if node is left.parent.left:
-                left.parent.left = left
+                left.parent.set_left(left)
             else:
-                left.parent.right = left
+                left.parent.set_right(left)
         else:
-            self._root = left
+            self.set_root(left)
         return left
 
     # Private helper method of balance function to perform LL rotation
-    def _left_rotate(self, node: RedBlackNode) -> Optional[RedBlackNode]:
+    def _left_rotate(self, node: RedBlackNode) -> RedBlackNode:
         right = node.right
         if not right:
             return right
-        right.parent = node.parent
+        right.set_parent(node.parent)
 
-        node.right = right.left
+        node.set_right(right.left)
         if node.right:
-            node.right.parent = node
+            node.right.set_parent(node)
 
-        right.left = node
-        node.parent = right
+        right.set_left(node)
+        node.set_parent(right)
 
         if right.parent:
             if node is right.parent.left:
-                right.parent.left = right
+                right.parent.set_left(right)
             else:
-                right.parent.right = right
+                right.parent.set_right(right)
         else:
-            self._root = right
+            self.set_root(right)
         return right
 
     # Private helper method for delete to perform exchange of data between node
     def _transplant(self, node: RedBlackNode,
                     new_node: Optional[RedBlackNode]) -> None:
         if not node.parent:
-            self._root = new_node
+            self.set_root(new_node)
         elif node is node.parent.left:
-            node.parent.left = new_node
+            node.parent.set_left(new_node)
         else:
-            node.parent.right = new_node
+            node.parent.set_right(new_node)
         if new_node:
-            new_node.parent = node.parent
+            new_node.set_parent(node.parent)
 
     def _delete(self, root, item: Any):
         node = self.search(item)
         if not node:
             return node
         color = node.color
         if node.left and node.right:
             predecessor = self.inorder_predecessor(node)
             color = predecessor.color
             pull_up = predecessor.left
             if predecessor.parent is node and pull_up:
-                pull_up.parent = predecessor
+                pull_up.set_parent(predecessor)
             else:
                 self._transplant(predecessor, pull_up)
-                predecessor.left = node.left
+                predecessor.set_left(node.left)
                 if node.left:
-                    node.left.parent = predecessor
+                    node.left.set_parent(predecessor)
             self._transplant(node, predecessor)
-            predecessor.right = node.right
+            predecessor.set_right(node.right)
             if node.right:
-                node.right.parent = predecessor
-            predecessor.color = node.color
+                node.right.set_parent(predecessor)
+            predecessor.set_color(node.color)
         else:
             pull_up = node.left if node.left else node.right
             self._transplant(node, pull_up)
 
         if color is BLACK:
             self._post_delete(pull_up)
 
         return self.root
 
-    def _resolve_left_black_conflict(self, node):
+    def _resolve_left_black_conflict(self, node: RedBlackNode) -> RedBlackNode:
         parent = node.parent
         sibling = parent.right
-        if sibling.color == RED:
-            sibling.color = BLACK
-            parent.color = RED
+        if sibling.color is RED:
+            sibling.set_color(BLACK)
+            parent.set_color(RED)
             self._left_rotate(parent)
             sibling = node.parent.right
 
-        if sibling.left.color == BLACK and sibling.right.color == BLACK:
-            sibling.color = RED
+        if sibling.left.color is BLACK and sibling.right.color is BLACK:
+            sibling.set_color(RED)
             node = parent
         else:
-            if sibling.right.color == BLACK:
-                sibling.left.color = BLACK
-                sibling.color = RED
+            if sibling.right.color is BLACK:
+                sibling.left.set_color(BLACK)
+                sibling.set_color(RED)
                 self._right_rotate(sibling)
                 sibling = parent.right
 
-            sibling.color = parent.color
-            parent.color = BLACK
-            sibling.right.color = BLACK
+            sibling.set_color(parent.color)
+            parent.set_color(BLACK)
+            sibling.right.set_color(BLACK)
             self._left_rotate(parent)
             node = self.root
 
         return node
 
-    def _resolve_right_black_conflict(self, node):
+    def _resolve_right_black_conflict(self,
+                                      node: RedBlackNode) -> RedBlackNode:
         parent = node.parent
         sibling = parent.left
         if sibling.color is RED:
-            sibling.color = BLACK
-            parent.color = RED
+            sibling.set_color(BLACK)
+            parent.set_color(RED)
             self._right_rotate(parent)
             sibling = parent.left
 
         if sibling.right.color is sibling.left.color is BLACK:
-            sibling.color = RED
+            sibling.set_color(RED)
             node = parent
         else:
             if sibling.left.color is BLACK:
-                sibling.right.color = BLACK
-                sibling.color = RED
+                sibling.right.set_color(BLACK)
+                sibling.set_color(RED)
                 self._left_rotate(sibling)
                 sibling = parent.left
 
-            sibling.color = parent.color
-            parent.color = BLACK
-            sibling.left.color = BLACK
+            sibling.set_color(parent.color)
+            parent.set_color(BLACK)
+            sibling.left.set_color(BLACK)
             self._right_rotate(parent)
             node = self.root
         return node
 
     def _post_delete(self, node: Optional[RedBlackNode]):
         # ! Resolve Double Black sentinel Conflict
         while node and node is not self.root and node.color is BLACK:
@@ -245,8 +240,8 @@
             if not parent:
                 break
             if node is parent.left:
                 node = self._resolve_left_black_conflict(node)
             else:
                 node = self._resolve_right_black_conflict(node)
         if node:
-            node.color = BLACK
+            node.set_color(BLACK)
```

### Comparing `datastax-0.4.1/datastax/trees/splay_tree.py` & `datastax-0.4.2/datastax/Trees/SplayTree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-# Splay Tree Implementation
-from __future__ import annotations
-
 import warnings
 from typing import Any, Optional
 
-from datastax.errors import (
+from datastax.Utils.Warnings import (
     DuplicateNodeWarning,
     DeletionFromEmptyTreeWarning,
     NodeNotFoundWarning
 )
-from datastax.trees.binary_search_tree import BinarySearchTree, TreeNode
-
 
-class SplayNode(TreeNode):
-    def __init__(self, data: Any,
-                 left: SplayNode = None,
-                 right: SplayNode = None) -> None:
-        super().__init__(data, left, right)
-        self.parent: Optional[SplayNode] = None
+from datastax.Trees.BinarySearchTree import BinarySearchTree
+from datastax.Nodes import SplayNode
 
 
 class SplayTree(BinarySearchTree):
     # Private helper function for inserting
     def _place(self, parent: Optional[SplayNode], data) -> Optional[SplayNode]:
         node = SplayNode(data)
         parent = None
@@ -37,22 +28,22 @@
                     f"Insertion unsuccessful. Item '{data}' already exists "
                     "in Tree. Splaying it",
                     DuplicateNodeWarning
                 )
                 if parent:
                     self._splay(parent)
                 return None
-        node.parent = parent
+        node.set_parent(parent)
         # Node to be added is root node
         if not parent:
             return node
         if parent.data > node.data:
-            parent.left = node
+            parent.set_left(node)
         else:
-            parent.right = node
+            parent.set_right(node)
         self._splay(node)
         return self.root
 
     def search(self, data: Any):
         """
         Searches a node in log2(n) time complexity BinarySearch Algorithm
         :param data: Any type of content in BST to search
@@ -90,86 +81,86 @@
         return self.root
 
     # Private helper method of balance function to perform RR rotation
     def _zig_rotate(self, node: SplayNode) -> Optional[SplayNode]:
         left = node.left
         if not left:
             return left
-        left.parent = node.parent
+        left.set_parent(node.parent)
 
-        node.left = left.right
+        node.set_left(left.right)
         if node.left:
-            node.left.parent = node
-        left.right = node
-        node.parent = left
+            node.left.set_parent(node)
+        left.set_right(node)
+        node.set_parent(left)
 
         if left.parent:
             if node is left.parent.left:
-                left.parent.left = left
+                left.parent.set_left(left)
             else:
-                left.parent.right = left
+                left.parent.set_right(left)
         else:
-            self._root = left
+            self.set_root(left)
         return left
 
     # Private helper method of balance function to perform LL rotation
     def _zag_rotate(self, node: SplayNode) -> Optional[SplayNode]:
         right = node.right
         if not right:
             return right
-        right.parent = node.parent
+        right.set_parent(node.parent)
 
-        node.right = right.left
+        node.set_right(right.left)
         if node.right:
-            node.right.parent = node
+            node.right.set_parent(node)
 
-        right.left = node
-        node.parent = right
+        right.set_left(node)
+        node.set_parent(right)
 
         if right.parent:
             if node is right.parent.left:
-                right.parent.left = right
+                right.parent.set_left(right)
             else:
-                right.parent.right = right
+                right.parent.set_right(right)
         else:
-            self._root = right
+            self.set_root(right)
         return right
 
     def delete(self, data: Any = None) -> None:
         if not self.root:
             warnings.warn(
                 "Deletion Unsuccessful. Can't delete from empty Tree",
                 DeletionFromEmptyTreeWarning
             )
             return
-        self._root = self._delete(self.root, data)
+        self.set_root(self._delete(self.root, data))
 
     def _delete(self, root, item: Any):
         node = self.search(item)
 
         if node.data != item:  # item was not found
             return self.root
         # Splitting the tree
         # First completing leftSubTree
         left_tree = SplayTree(None, self.root.left)
         if left_tree.root:
-            left_tree.root.parent = None
+            left_tree.root.set_parent(None)
 
         right_tree = SplayTree(None, self.root.right)
         if right_tree.root:
-            right_tree.root.parent = None
+            right_tree.root.set_parent(None)
 
         if left_tree.root:
             # Finding the maximum element in left subtree
             predecessor = self.inorder_predecessor(self.root)
             if predecessor:
                 left_tree._splay(predecessor)
-            left_tree.root.right = right_tree.root
+            left_tree.root.set_right(right_tree.root)
             if right_tree.root:
-                right_tree.root.parent = left_tree.root
+                right_tree.root.set_parent(left_tree.root)
             self._root = left_tree.root
         else:
             self._root = right_tree.root
 
         return self.root
 
     def _splay(self, node: SplayNode):
```

### Comparing `datastax-0.4.1/datastax/trees/sum_segment_tree.py` & `datastax-0.4.2/datastax/Trees/SumSegmentTree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-# Sum Segment Tree implementation
-from __future__ import annotations
-
-from typing import Any, Optional
-
-from datastax.trees.private_trees.segment_tree import SegmentTree, SegmentNode
+from typing import Optional, Self, Sequence
+from datastax.Trees.SegmentTree import SegmentTree
+from datastax.Nodes import SegmentNode
 
 
 class SumSegmentTree(SegmentTree):
-    def __init__(self, array=None, root=None):
-        self._lazy_tree = SegmentTree()
-        super().__init__(array, root)
+    _lazy_tree = SegmentTree()
 
-    def insert(self, item: Any):
-        raise NotImplementedError
+    def __init__(self, items: Optional[Sequence] = None,
+                 root: Optional[SegmentNode] = None):
+        super().__init__(items, root)
 
     @property
     def lazy_tree(self):
         return self._lazy_tree
 
-    def _construct(self, array: list[int] = None) -> Optional[SumSegmentTree]:
+    def _construct(self, array: Optional[Sequence] = None) -> Self | None:
         if not array or array[0] is None:
             return None
 
-        def build(left: int, right: int) -> tuple[SegmentNode, ...]:
+        def build(left: int, right: int) -> tuple[SegmentNode, SegmentNode]:
             node, lazy_node = SegmentNode(None), SegmentNode(0)
             # Leaf Node
             if array and left == right:
                 node.left_index, node.right_index = left, right
                 lazy_node.left_index, lazy_node.right_index = left, right
                 node.data = array[left]
                 return node, lazy_node
             # Intermediate Node
             mid = (left + right) // 2
-            node.left, lazy_node.left = build(left, mid)
-            node.right, lazy_node.right = build(mid + 1, right)
+            left_node, lazy_left_node = build(left, mid)
+            right_node, lazy_right_node = build(mid + 1, right)
+            node.set_left(left_node), lazy_node.set_left(lazy_left_node)
+            node.set_right(right_node), lazy_node.set_right(lazy_right_node)
             node.left_index = lazy_node.left_index = node.left.left_index
             node.right_index = lazy_node.right_index = node.right.right_index
             node.data = sum((node.left.data, node.right.data))
             return node, lazy_node
 
-        self._root, self._lazy_tree._root = build(0, len(array) - 1)
+        root, lazy_root = build(0, len(array) - 1)
+        self.set_root(root), self.lazy_tree.set_root(lazy_root)
         return self
 
     @staticmethod
     def _perform_lazy_update(root: SegmentNode, lazy_node: SegmentNode,
                              start: int, end: int, nodes: int) -> None:
         # has lazy values, needs to be propagated
         if lazy_node.data:
             root.data += lazy_node.data * nodes
             if start != end:
                 lazy_node.left.data += lazy_node.data
                 lazy_node.right.data += lazy_node.data
             # No longer a lazy node
             lazy_node.data = 0
 
-    def get_sum(self, left: int, right: int,
-                root: SegmentNode = None,
-                lazy_node: SegmentNode = None) -> int:
-        if not root:
-            root = self.root
-            lazy_node = self.lazy_tree.root
+    def get_sum(self, left: int, right: int) -> int:
+        return self.get_range(left, right, self.root, self.lazy_tree.root)
+
+    def get_range(self, left: int, right: int,
+                  root: SegmentNode | None,
+                  lazy_node: SegmentNode | None) -> int:
         if not root or not lazy_node:
             return 0
 
         start, end = root.left_index, root.right_index
         nodes = end - start + 1
 
         # perform lazy update
@@ -73,16 +72,16 @@
         if end < left or start > right or end < start:
             return 0
 
         if root.left_index >= left and root.right_index <= right:
             return root.data
 
         return sum((
-            self.get_sum(left, right, root.left, lazy_node.left),
-            self.get_sum(left, right, root.right, lazy_node.right)
+            self.get_range(left, right, root.left, lazy_node.left),
+            self.get_range(left, right, root.right, lazy_node.right)
         ))
 
     def update_at_range(self, left: int, right: int, data: int) -> None:
         if not self.root:
             return None
 
         def update(node: SegmentNode, lazy_node: SegmentNode) -> None:
@@ -97,16 +96,16 @@
                 return
 
             # location is perfectly in bounds
             if left <= start <= end <= right:
                 node.data += data * nodes
                 # Mark its children lazy, no need to propagate further
                 if start != end:
-                    lazy_node.left.data += data
-                    lazy_node.right.data += data
+                    lazy_node.left.data += node.data
+                    lazy_node.right.data += node.data
                 return
 
             # location is partially in bounds
             update(node.left, lazy_node.left)
             update(node.right, lazy_node.right)
             node.data = sum((node.left.data, node.right.data))
 
@@ -124,22 +123,7 @@
             mid = (node.left_index + node.right_index) // 2
             update_node = node.left if index <= mid else node.right
             difference = update(update_node, new)
             node.data += difference
             return difference
 
         update(self.root, data)
-
-
-if __name__ == '__main__':
-    tree = SumSegmentTree([2, 3, 1, 4, 2, 5, 2, 3, 1, 5])
-    # tree = SumSegmentTree()
-    print(tree)
-    tree.update_at_range(3, 9, +5)
-    print(tree)
-    tree.update_at_range(5, 8, +3)
-    print(tree.get_sum(3, 5))
-    print(tree)
-    print(tree.lazy_tree)
-    print(tree.segment_array)
-    # print(tree)
-    # print(tree.lazy_tree)
```

### Comparing `datastax-0.4.1/datastax/trees/threaded_binary_tree.py` & `datastax-0.4.2/datastax/Trees/ThreadedBinaryTree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,105 @@
-# Threaded Binary Tree Implementation
-from __future__ import annotations
-
 import warnings
-from typing import Optional, Any, Union
-
-from datastax.errors import DuplicateNodeWarning, ExplicitInsertionWarning
-from datastax.trees import TreeNode, AVLNode, HeapNode
-from datastax.trees.private_trees import threaded_binary_tree
-from datastax.trees.private_trees.threaded_binary_tree import ThreadedNode
+from typing import Any, Optional, Self, Sequence
+from datastax.Utils.Warnings import DuplicateNodeWarning
+from datastax.Lists import Queue
+from datastax.Trees.BinaryTree import BinaryTree
+from datastax.Trees.AbstractTrees import ThreadedBinaryTree as AbstractTree
+from datastax.Nodes import ThreadedNode
+
+
+class ThreadedBinaryTree(BinaryTree, AbstractTree):
+    dummy_node = ThreadedNode(None)
+    tail: Optional[ThreadedNode] = None
+    head: Optional[ThreadedNode] = None
+
+    def set_root(self, root):
+        if root is None or isinstance(root, ThreadedNode):
+            super().set_root(root)
+            self.head = self.tail = self.root
+            self.dummy_node.set_left(self.root)
+            self.dummy_node.set_right(self.dummy_node)
+            return
+        raise TypeError("The 'root' parameter must be an "
+                        "instance of ThreadedNode or its subclass.")
 
-rootNode = Union[TreeNode, AVLNode, HeapNode]
+    def _construct(self, items: Optional[Sequence] = None) -> Self | None:
+        if not items or items[0] is None:
+            return None
+        for item in items:
+            self.insert(item)
+        return self
+
+    @property  # Level Order Traversal -> Tree to array
+    def array_repr(self) -> list[Any]:
+        array = []
+        queue = Queue()
+        if self.root:
+            queue.enqueue(self.root)
+        while not queue.is_empty():
+            node = queue.dequeue()
+            array.append(node.data)
+            if node.left_is_child:
+                queue.enqueue(node.left)
+            if node.right_is_child:
+                queue.enqueue(node.right)
 
+        return array
 
-class ThreadedBinaryTree(threaded_binary_tree.ThreadedBinaryTree):
-    def convert_to_tbt(self, root: rootNode) -> None:
-        def insert_inorder(node: Optional[ThreadedNode]) -> None:
+    def convert_from(self, root: Any) -> None:
+        def insert_inorder(node: ThreadedNode | None) -> None:
             if not node:
                 return
             insert_inorder(node.left)
             array.append(node)
             insert_inorder(node.right)
 
-        def clone_binary_tree(node: rootNode) -> Optional[ThreadedNode]:
+        def clone_binary_tree(node) -> Optional[ThreadedNode]:
             if not node:
                 return None
             return ThreadedNode(node.data,
                                 clone_binary_tree(node.left),
                                 clone_binary_tree(node.right))
 
         array: list[ThreadedNode] = []
-        self._root = clone_binary_tree(root)
+        self.set_root(clone_binary_tree(root))
 
         # Storing inorder traversal in queue
-        insert_inorder(self._root)
+        insert_inorder(self.root)
         for n in range(len(array)):
             if not array[n].left:
-                array[n].left = self.dummy_node if not n else array[n - 1]
+                array[n].set_left(
+                    self.dummy_node if not n else array[n - 1]
+                )
             if not array[n].right:
-                array[n].right = self.dummy_node if n == len(array) - 1 \
-                    else array[n + 1]
+                array[n].set_right(
+                    self.dummy_node if n == len(array) - 1 else array[n + 1]
+                )
 
         self.head, self.tail = array[0], array[-1]
-        self.dummy_node.left = self.root
-        self.dummy_node.left_is_child = True
+        self.dummy_node.set_left(self.root)
+        self.dummy_node.set_left_is_child(True)
 
-    def insert(self, data: Any, root: ThreadedNode = None) -> None:
-        if not isinstance(self.tree, ThreadedBinaryTree):
-            warnings.warn(
-                "Can't insert in Threaded Tree with explicit insertion logic"
-                "of Foreign Tree Logic",
-                ExplicitInsertionWarning
-            )
-            return
+    def insert(self, data: Any, root: Optional[ThreadedNode] = None) -> None:
         root = root or self.root
-        node = ThreadedNode(data)
         if not root:
-            self._root = node
-            node.left = node.right = self.dummy_node
+            node = ThreadedNode(data, self.dummy_node, self.dummy_node)
+            node.set_left_is_child(False)
+            node.set_right_is_child(False)
+            self.set_root(node)
             self.head = self.tail = self.root
-            self.dummy_node.left = self.root
-            self.dummy_node.left_is_child = True
+            self.dummy_node.set_left(self.root)
+            self.dummy_node.set_left_is_child(True)
             return
 
+        node = ThreadedNode(data)
         left = right = False
+
         while root:
+
             if data is None:
                 break
             if root.data > data:
                 if not root.left_is_child:
                     # will insert the child as left child
                     left = True
                     break
@@ -83,39 +115,50 @@
             else:
                 warnings.warn(
                     f"Insertion unsuccessful. Item '{data}' already exists "
                     "in Tree", DuplicateNodeWarning)
                 return
 
         if left and root:
-            node.left = root.left
-            root.left = node
-            node.left_is_child = root.left_is_child
-            root.left_is_child = True
-            node.right = root
+            node.set_left(root.left)
+            root.set_left(node)
+            node.set_left_is_child(root.left_is_child)
+            root.set_left_is_child(True)
+            node.set_right(root)
 
         elif right and root:
-            node.right = root.right
-            root.right = node
-            node.right_is_child = root.right_is_child
-            root.right_is_child = True
-            node.left = root
+            node.set_right(root.right)
+            root.set_right(node)
+            node.set_right_is_child(root.right_is_child)
+            root.set_right_is_child(True)
+            node.set_left(root)
 
         if node.left is self.dummy_node:
             self.head = node
         elif node.right is self.dummy_node:
             self.tail = node
 
     # DFS Traversal without using stack
     def inorder(self) -> list[Any]:
-        ref: ThreadedNode = self.head
-        array: list[Any] = []
-        while ref is not self.dummy_node:
+        ref = self.head
+        array = []
+        while ref and ref is not self.dummy_node:
             array.append(ref.data)
             if not ref.right_is_child:
                 ref = ref.right
             else:
                 node = ref.right
                 while node.left_is_child:
                     node = node.left
                 ref = node
         return array
+
+
+if __name__ == '__main__':
+    T = ThreadedBinaryTree([10, 30], ThreadedNode(20))
+    print(T)
+    # print(T.root)
+    # print(T.root.left)
+    # print(T.root.right is T.dummy_node)
+    T.insert(110)
+    print(T)
+    print(ThreadedBinaryTree([110, 10, 20]))
```

### Comparing `datastax-0.4.1/datastax.egg-info/PKG-INFO` & `datastax-0.4.2/datastax.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datastax
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python library to handle dataStructures
 Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax
 Author: Pritam K
 Author-email: pritamkundu771@gmail.com
 Maintainer: Pritam Kundu
 License: MIT
@@ -19,31 +19,27 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Typing :: Typed
-Requires-Python: >=3.11
+Requires-Python: >3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-    updated: Wednesday, 12th July 2023
+    updated: Thursday, 03rd August 2023
 
 <div align=center>
     <a href="https://github.com/warmachine028/datastax">
         <img width=200 src="https://github.com/warmachine028/datastax/assets/75939390/2c1ad8f7-b1ed-44aa-9923-307af5a52cfc" alt="datastax">
     </a>
     <p style="font-family: roboto, calibri; font-size:12pt; font-style:italic">Simplicity meets intelligence</p>
     <a href="https://pypi.org/project/datastax">
@@ -68,28 +64,37 @@
     <br>
 </div>
 
 # [dataStax](https://github.com/warmachine028/datastax)
 
 ## What's New?
 
-- Refactored Array Contents
-- Added AbstractArray SubModule to abstract print logic
-- Added more test cases for Queues
-- Type Checked Arrays and Lists with mypy
+- Refactored Trees
+- Added Nodes SubPackage
+- Separated TreeNodes into Nodes
+- Added Tables SubPackage
+- Added Colors and ColorCodes in Utils
+- Refactored Lists
+- Removed `__repr__` overrides
+- Added Exceptions in Utils
+- Added Warnings in Utils
+- Added new workflows
+- Added datastax.Wiki
 
 ## Table of Contents
 
+- [What's New](#whats-new)
 - [Introduction](#introduction)
 - [Problem Statement](#problem-statement)
 - [Benefits](#benefits)
 - [Requirements](#requirements)
 - [Installation](#installation)
 - [Usage](#usage)
-- [What's Next](#whats-next)
+- [Documentation](#documentation)
+- [License](#license)
 
 ## Introduction
 
 - This library offers a simple yet powerful solution for implementing common abstract data structures.
 - With a pure Python implementation, it provides representations of tree, linked list, and array-based data structures
   accessible through a basic command prompt interface.
 - The package includes visualization features that enhance the understanding of each data structure.
@@ -149,15 +154,15 @@
   1. LinkedLists
   2. Trees
   3. Arrays
   
   Usage
   > py datastax <data-structure> [data]
   Data Structures:
-  ->  trees          Hierarchical DS
+  ->  Trees          Hierarchical DS
   ->  linkedlists    Linear DS
   ->  arrays         Fixed Size Linear DS
 
   ```
 - Then follow as the instruction guides
 
 ```bash
@@ -179,20 +184,19 @@
   ...
 ```
 
 ### Practical Usage
 
 - **Queue**
 
-![queue](https://github.com/warmachine028/datastax/assets/75939390/0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409)
+![queue](https://github.com/warmachine028/datastax/assets/75939390/e62ba451-f499-45dc-bcb9-9e29ebfe6dbd)
 
 ![queue_output](https://github.com/warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde)
 
-------------------------------------
----------------
+---------------------------------------------------
 
 - **BinaryTree**
 
 ![binaryTree](https://github.com/warmachine028/datastax/assets/75939390/7228c4b4-def7-4c6b-9e29-e6e244c2c4c1)
 
 ![binaryTree_output](https://github.com/warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c)
 
@@ -220,25 +224,33 @@
 
 ![sst_output](https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-88c7-40e4dcc11215)
 
 ---------------------------------------------------
 
 - **HuffmanTree**
 
-![hft](https://github.com/warmachine028/datastax/assets/75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e)
+![hft](https://github.com/warmachine028/datastax/assets/75939390/bab7da94-624f-40ac-b746-463157e84cdf)
 
 ![hft_output](https://github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-8dbf91c008a2)
 
 ---------------------------------------------------
 
 - **RedBlackTree**
 
 ![rbt](https://github.com/warmachine028/datastax/assets/75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba)
 
 ![rbt_output](https://github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-db84dbf274f0)
 
-## What's Next
+## Documentation
+
+- For detailed documentation. See [documentation](https://github.com/warmachine028/datastax/wiki)
+- (Still in progress) 
+
+## License
+
+- see [LICENSE]
+
+**Pritam, 2023**
+
+[license]: https://github.com/warmachine028/datastax/blob/main/LICENSE
 
-- Enhanced Documentation
-- Better TestCases for Huffman Tree
-- Better TestCases for Segment Trees
-- Test Cases for Fibonacci Tree
+<!-- 03/08/23 -->
```

#### html2text {}

```diff
@@ -1,93 +1,94 @@
-Metadata-Version: 2.1 Name: datastax Version: 0.4.1 Summary: A python library
+Metadata-Version: 2.1 Name: datastax Version: 0.4.2 Summary: A python library
 to handle dataStructures Home-page: https://github.com/warmachine028/datastax
 Download-URL: https://pypi.python.org/pypi/datastax Author: Pritam K Author-
 email: pritamkundu771@gmail.com Maintainer: Pritam Kundu License: MIT Project-
 URL: Bug Tracker, https://github.com/warmachine028/datastax/issues Project-URL:
 Documentation, https://github.com/warmachine028/datastax#readme Project-URL:
 Source Code, https://github.com/warmachine028/datastax Platform: Windows
 Platform: Linux Platform: Solaris Platform: Mac OS-X Platform: Unix Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 End Users/Desktop Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Documentation
-Classifier: Topic :: Education :: Testing Classifier: Topic :: Scientific/
-Engineering :: Visualization Classifier: Topic :: Software Development ::
-Documentation Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Testing :: Unit
-Classifier: Typing :: Typed Requires-Python: >=3.11 Description-Content-Type:
-text/markdown License-File: LICENSE updated: Wednesday, 12th July 2023
+Independent Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Documentation Classifier: Topic :: Education :: Testing Classifier:
+Topic :: Scientific/Engineering :: Visualization Classifier: Topic :: Software
+Development :: Documentation Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Topic :: Software Development ::
+Testing :: Unit Classifier: Typing :: Typed Requires-Python: >3.11 Description-
+Content-Type: text/markdown License-File: LICENSE updated: Thursday, 03rd
+August 2023
                                   [datastax]
                          Simplicity meets intelligence
                            [PyPI] [PyPI_Downloads]
             [https://img.shields.io/github/v/release/warmachine028/
      datastax?color=brightgreen] [https://img.shields.io/github/v/release/
                                 warmachine028/
       datastax?color=lightgreen&include_prereleases&label=pre%20release]
     [https://img.shields.io/github/stars/warmachine028/datastax] [https://
  img.shields.io/github/license/warmachine028/datastax?color=orange] [https://
         img.shields.io/github/forks/warmachine028/datastax?color=cyan]
 # [dataStax](https://github.com/warmachine028/datastax) ## What's New? -
-Refactored Array Contents - Added AbstractArray SubModule to abstract print
-logic - Added more test cases for Queues - Type Checked Arrays and Lists with
-mypy ## Table of Contents - [Introduction](#introduction) - [Problem Statement]
-(#problem-statement) - [Benefits](#benefits) - [Requirements](#requirements) -
-[Installation](#installation) - [Usage](#usage) - [What's Next](#whats-next) ##
-Introduction - This library offers a simple yet powerful solution for
-implementing common abstract data structures. - With a pure Python
-implementation, it provides representations of tree, linked list, and array-
-based data structures accessible through a basic command prompt interface. -
-The package includes visualization features that enhance the understanding of
-each data structure. - Students can greatly benefit from utilizing this package
-for their learning and educational purposes. - Please note that this project is
-currently a work in progress and undergoing active development. ## Problem
-Statement - Many CS students encounter difficulties in comprehending the
-intricate internal architecture of complex Abstract Data Types (ADTs) during
-the initial stages of their B.Tech course. - When attempting to solve coding
-challenges that involve writing test cases using these ADTs, it becomes
-excessively burdensome to manually create these data structures from scratch. -
-Furthermore, while developing programs that implement these ADTs, numerous
-errors are encountered due to the inability to visualize and understand the
-underlying processes of these data structures. ## Benefits - Swift installation
-process - Efficient and prompt updates - Minimal disk space usage due to its
-small size - No additional modules or dependencies needed - Developed entirely
-from scratch - Upcoming user-friendly documentation - Command line
-demonstration for easy usage ## Requirements - Runs on latest Python 3.11+ -
-(Suggesting you to always update to the latest python version) ## Installation
-1. Use the python package manager [pip](https://pip.pypa.io/en/stable/) to
-install datastax. ```bash pip install datastax ``` ## Usage ### Demo - To get a
-demo of the library use the following command - **Windows**: ```bash > py -
-m datastax ``` - **Unix based systems**: ```bash $ python3 -m datastax ``` -
-_Result_ ```bash Available modules are: 1. LinkedLists 2. Trees 3. Arrays Usage
-> py datastax  [data] Data Structures: -> trees Hierarchical DS -> linkedlists
-Linear DS -> arrays Fixed Size Linear DS ``` - Then follow as the instruction
-guides ```bash > py -m datastax linkedlist 1 2 3 4 Visuals for LinkedLists: 1.
-Singly Linked List: HEAD TAIL âââââââ¥âââââ
+Refactored Trees - Added Nodes SubPackage - Separated TreeNodes into Nodes -
+Added Tables SubPackage - Added Colors and ColorCodes in Utils - Refactored
+Lists - Removed `__repr__` overrides - Added Exceptions in Utils - Added
+Warnings in Utils - Added new workflows - Added datastax.Wiki ## Table of
+Contents - [What's New](#whats-new) - [Introduction](#introduction) - [Problem
+Statement](#problem-statement) - [Benefits](#benefits) - [Requirements]
+(#requirements) - [Installation](#installation) - [Usage](#usage) -
+[Documentation](#documentation) - [License](#license) ## Introduction - This
+library offers a simple yet powerful solution for implementing common abstract
+data structures. - With a pure Python implementation, it provides
+representations of tree, linked list, and array-based data structures
+accessible through a basic command prompt interface. - The package includes
+visualization features that enhance the understanding of each data structure. -
+Students can greatly benefit from utilizing this package for their learning and
+educational purposes. - Please note that this project is currently a work in
+progress and undergoing active development. ## Problem Statement - Many CS
+students encounter difficulties in comprehending the intricate internal
+architecture of complex Abstract Data Types (ADTs) during the initial stages of
+their B.Tech course. - When attempting to solve coding challenges that involve
+writing test cases using these ADTs, it becomes excessively burdensome to
+manually create these data structures from scratch. - Furthermore, while
+developing programs that implement these ADTs, numerous errors are encountered
+due to the inability to visualize and understand the underlying processes of
+these data structures. ## Benefits - Swift installation process - Efficient and
+prompt updates - Minimal disk space usage due to its small size - No additional
+modules or dependencies needed - Developed entirely from scratch - Upcoming
+user-friendly documentation - Command line demonstration for easy usage ##
+Requirements - Runs on latest Python 3.11+ - (Suggesting you to always update
+to the latest python version) ## Installation 1. Use the python package manager
+[pip](https://pip.pypa.io/en/stable/) to install datastax. ```bash pip install
+datastax ``` ## Usage ### Demo - To get a demo of the library use the following
+command - **Windows**: ```bash > py -m datastax ``` - **Unix based systems**:
+```bash $ python3 -m datastax ``` - _Result_ ```bash Available modules are: 1.
+LinkedLists 2. Trees 3. Arrays Usage > py datastax  [data] Data Structures: -
+> Trees Hierarchical DS -> linkedlists Linear DS -> arrays Fixed Size Linear DS
+``` - Then follow as the instruction guides ```bash > py -m datastax linkedlist
+1 2 3 4 Visuals for LinkedLists: 1. Singly Linked List: HEAD TAIL
 âââââââ¥âââââ âââââââ¥âââââ
-âââââââ¥âââââ â 1 â ----->â 2 â ----->â 3 â
------>â 4 â -----> NULL âââââââ¨âââââ
+âââââââ¥âââââ âââââââ¥âââââ â 1
+â ----->â 2 â ----->â 3 â ----->â 4 â -----> NULL
 âââââââ¨âââââ âââââââ¨âââââ
-âââââââ¨âââââ 2. Doubly Linked List: HEAD TAIL
+âââââââ¨âââââ âââââââ¨âââââ 2.
+Doubly Linked List: HEAD TAIL
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ
 ââââââ¥ââââââ¥âââââ NULL <----- â 1 â <----
 ---> â 2 â <-------> â 3 â <-------> â 4 â -----> NULL
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ
 ââââââ¨ââââââ¨âââââ ... ``` ### Practical Usage
 - **Queue** ![queue](https://github.com/warmachine028/datastax/assets/75939390/
-0fe72e7a-7eb9-4ee9-9b7a-6c0f83d98409) ![queue_output](https://github.com/
+e62ba451-f499-45dc-bcb9-9e29ebfe6dbd) ![queue_output](https://github.com/
 warmachine028/datastax/assets/75939390/daecb209-d459-4374-96e0-816deb08dcde) --
----------------------------------- --------------- - **BinaryTree** !
+------------------------------------------------- - **BinaryTree** !
 [binaryTree](https://github.com/warmachine028/datastax/assets/75939390/
 7228c4b4-def7-4c6b-9e29-e6e244c2c4c1) ![binaryTree_output](https://github.com/
 warmachine028/datastax/assets/75939390/2357fa58-3122-47ad-ac7f-f67d72ef6e8c) --
 ------------------------------------------------- - **MinHeapTree** ![mht]
 (https://github.com/warmachine028/datastax/assets/75939390/1c00a207-9ea0-4965-
 898f-29e37883fac5) ![mht_output](https://github.com/warmachine028/datastax/
 assets/75939390/fcfe24d9-6b80-4b16-873c-3f5c3d808d70) -------------------------
@@ -96,16 +97,17 @@
 [tbt_output](https://github.com/warmachine028/datastax/assets/75939390/
 9e77c5dc-082c-471b-90d5-33792673bdf3) -----------------------------------------
 ---------- - **SumSegmentTree** ![sst](https://github.com/warmachine028/
 datastax/assets/75939390/7bdcfd6e-37ac-4421-b6d2-acd59cf4976c) ![sst_output]
 (https://github.com/warmachine028/datastax/assets/75939390/3a3f1de2-72e8-4b1d-
 88c7-40e4dcc11215) --------------------------------------------------- -
 **HuffmanTree** ![hft](https://github.com/warmachine028/datastax/assets/
-75939390/5dc609a6-51c2-4ec9-88ba-c1ea175ef88e) ![hft_output](https://
+75939390/bab7da94-624f-40ac-b746-463157e84cdf) ![hft_output](https://
 github.com/warmachine028/datastax/assets/75939390/2de13da6-8eaa-4e62-a06a-
 8dbf91c008a2) --------------------------------------------------- -
 **RedBlackTree** ![rbt](https://github.com/warmachine028/datastax/assets/
 75939390/8d924d6e-d63a-4891-bf9e-c7acdb3775ba) ![rbt_output](https://
 github.com/warmachine028/datastax/assets/75939390/3af4ceb6-1e68-4906-ba39-
-db84dbf274f0) ## What's Next - Enhanced Documentation - Better TestCases for
-Huffman Tree - Better TestCases for Segment Trees - Test Cases for Fibonacci
-Tree
+db84dbf274f0) ## Documentation - For detailed documentation. See
+[documentation](https://github.com/warmachine028/datastax/wiki) - (Still in
+progress) ## License - see [LICENSE] **Pritam, 2023** [license]: https://
+github.com/warmachine028/datastax/blob/main/LICENSE
```

### Comparing `datastax-0.4.1/datastax.egg-info/SOURCES.txt` & `datastax-0.4.2/datastax.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.py
 datastax/__init__.py
 datastax/__main__.py
-datastax/errors.py
 datastax.egg-info/PKG-INFO
 datastax.egg-info/SOURCES.txt
 datastax.egg-info/dependency_links.txt
 datastax.egg-info/top_level.txt
 datastax/Arrays/PriorityQueue.py
 datastax/Arrays/Queue.py
 datastax/Arrays/Stack.py
@@ -15,43 +14,75 @@
 datastax/Arrays/AbstractArrays/Array.py
 datastax/Arrays/AbstractArrays/Queue.py
 datastax/Arrays/AbstractArrays/Stack.py
 datastax/Arrays/AbstractArrays/__init__.py
 datastax/Lists/CircularLinkedList.py
 datastax/Lists/DoublyCircularList.py
 datastax/Lists/DoublyLinkedList.py
-datastax/Lists/DoublyNode.py
 datastax/Lists/LRUCache.py
 datastax/Lists/LinkedList.py
-datastax/Lists/Node.py
 datastax/Lists/Queue.py
 datastax/Lists/__init__.py
 datastax/Lists/AbstractLists/CircularLinkedList.py
 datastax/Lists/AbstractLists/DoublyCircularList.py
 datastax/Lists/AbstractLists/DoublyLinkedList.py
-datastax/Lists/AbstractLists/DoublyNode.py
 datastax/Lists/AbstractLists/LinkedList.py
-datastax/Lists/AbstractLists/Node.py
 datastax/Lists/AbstractLists/Queue.py
 datastax/Lists/AbstractLists/__init__.py
+datastax/Nodes/AVLNode.py
+datastax/Nodes/DoublyNode.py
+datastax/Nodes/HeapNode.py
+datastax/Nodes/HuffmanNode.py
+datastax/Nodes/Node.py
+datastax/Nodes/RedBlackNode.py
+datastax/Nodes/SegmentNode.py
+datastax/Nodes/SplayNode.py
+datastax/Nodes/ThreadedNode.py
+datastax/Nodes/TreeNode.py
+datastax/Nodes/__init__.py
+datastax/Nodes/AbstractNodes/DoublyNode.py
+datastax/Nodes/AbstractNodes/HuffmanNode.py
+datastax/Nodes/AbstractNodes/Node.py
+datastax/Nodes/AbstractNodes/RedBlackNode.py
+datastax/Nodes/AbstractNodes/SegmentNode.py
+datastax/Nodes/AbstractNodes/ThreadedNode.py
+datastax/Nodes/AbstractNodes/TreeNode.py
+datastax/Nodes/AbstractNodes/__init__.py
+datastax/Tables/HuffmanTable.py
+datastax/Tables/__init__.py
+datastax/Tables/AbstractTables/HuffmanTable.py
+datastax/Tables/AbstractTables/__init__.py
+datastax/Trees/AVLTree.py
+datastax/Trees/BinarySearchTree.py
+datastax/Trees/BinaryTree.py
+datastax/Trees/ExpressionTree.py
+datastax/Trees/FibonacciTree.py
+datastax/Trees/HeapTree.py
+datastax/Trees/HuffmanTree.py
+datastax/Trees/MinHeapTree.py
+datastax/Trees/MinSegmentTree.py
+datastax/Trees/RedBlackTree.py
+datastax/Trees/SegmentTree.py
+datastax/Trees/SplayTree.py
+datastax/Trees/SumSegmentTree.py
+datastax/Trees/ThreadedBinaryTree.py
+datastax/Trees/__init__.py
+datastax/Trees/AbstractTrees/BinaryTree.py
+datastax/Trees/AbstractTrees/HuffmanTree.py
+datastax/Trees/AbstractTrees/RedBlackTree.py
+datastax/Trees/AbstractTrees/SegmentTree.py
+datastax/Trees/AbstractTrees/ThreadedBinaryTree.py
+datastax/Trees/AbstractTrees/__init__.py
+datastax/Utils/ColorCodes.py
+datastax/Utils/Colors.py
 datastax/Utils/Commons.py
 datastax/Utils/__init__.py
-datastax/trees/__init__.py
-datastax/trees/avl_tree.py
-datastax/trees/binary_search_tree.py
-datastax/trees/binary_tree.py
-datastax/trees/expression_tree.py
-datastax/trees/fibonacci_tree.py
-datastax/trees/heap_tree.py
-datastax/trees/huffman_tree.py
-datastax/trees/min_heap_tree.py
-datastax/trees/min_segment_tree.py
-datastax/trees/red_black_tree.py
-datastax/trees/splay_tree.py
-datastax/trees/sum_segment_tree.py
-datastax/trees/threaded_binary_tree.py
-datastax/trees/private_trees/__init__.py
-datastax/trees/private_trees/binary_tree.py
-datastax/trees/private_trees/huffman_tree.py
-datastax/trees/private_trees/red_black_tree.py
-datastax/trees/private_trees/segment_tree.py
-datastax/trees/private_trees/threaded_binary_tree.py
+datastax/Utils/Exceptions/DatastaxException.py
+datastax/Utils/Exceptions/InvalidExpressionException.py
+datastax/Utils/Exceptions/OverflowException.py
+datastax/Utils/Exceptions/PathNotFoundException.py
+datastax/Utils/Exceptions/PathNotGivenException.py
+datastax/Utils/Exceptions/UnderflowException.py
+datastax/Utils/Exceptions/UnmatchedBracketPairException.py
+datastax/Utils/Exceptions/__init__.py
+datastax/Utils/Warnings/DatastaxWarnings.py
+datastax/Utils/Warnings/__init__.py
```

### Comparing `datastax-0.4.1/setup.py` & `datastax-0.4.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,65 @@
 
 import datastax
 
 try:  # https://stackoverflow.com/questions/30700166/python-open-file-error
     with codecs.open("README.md", 'r', errors='ignore', encoding='utf8') as f:
         readme_contents = f.read()
 
-except Exception as error:
+except FileNotFoundError as e:
     readme_contents = (
-        'This library which supports ADTs like LinkedLists and Trees and its '
-        'types. This instant library is solely written from scratch and '
-        'requires no additional libraries to be installed. It solves the '
+        'This library which supports ADTs like Arrays, LinkedLists and Trees '
+        'and its types. This instant library is solely written from scratch '
+        'and requires no additional libraries to be installed. It solves the '
         'purpose of writing programs for complex data structures from scratch,'
         ' visualizing ADTs and simplify  writing its inner architectures. This'
         ' Module Supports the following dataStructures:\n'
-        '1. Arrays:\n'
+        '1. Nodes\n'
+        '   a. Node\n'
+        '   b. Doubly Node\n'
+        '   c. Tree Node\n'
+        '   d. AVL Node\n'
+        '   e. Red-Black Node\n'
+        '   f. Splay Node\n'
+        '   g. Heap Node\n'
+        '   h. Segment Node\n'
+        '   i. Huffman Node\n'
+        '   j. Threaded Node\n'
+        '2. Arrays:\n'
         '   a. Queue\n'
         '   b. Stack\n\n'
         '   c. Priority Queue\n\n'
-        '2. Lists:\n'
-        '   a. Singly Linked List\n'
-        '   b. Doubly Linked List\n'
-        '   c. Circular Linked List\n'
-        '   d. Doubly Circular List\n'
+        '3. Lists:\n'
+        '   a. Singly-Linked List\n'
+        '   b. Doubly-Linked List\n'
+        '   c. Circular-Linked List\n'
+        '   d. Doubly-Circular List\n'
         '   e. Queue\n\n'
         '   f. LRU Cache\n\n'
-        '3. Trees:\n'
+        '4. Trees:\n'
         '   a. Binary Tree\n'
-        '   b. Binary Search Tree\n'
-        '   c. AVL Tree\n'
-        '   d. Heap Tree\n'
-        '   e. Min Heap Tree\n'
-        '   f. Expression Tree\n'
-        '   e. Threaded Binary Tree\n'
-        '   f. Segment Trees\n'
-        '       i. Sum Segment Tree\n'
-        '      ii. Min Segment Tree\n'
-        '   g. Huffman Tree\n'
-        '   h. Red Black Tree\n'
-        '   i. Fibonacci Tree\n'
-        '   j. Splay Tree\n\n'
+        '   b. Search Trees\n'
+        '        i. Binary-Search Tree\n'
+        '       ii. AVL Tree\n'
+        '      iii. Red-Black Tree\n'
+        '       iv. Splay Tree\n'
+        '   c. Heap Trees\n'
+        '        i. Max-Heap Tree\n'
+        '       ii. Min-Heap Tree\n'
+        '   d. Segment Trees\n'
+        '       i. Sum-Segment Tree\n'
+        '      ii. Min-Segment Tree\n'
+        '   f. Huffman Tree\n'
+        '   g. Fibonacci Tree\n'
+        '   h. Expression Tree\n'
+        '   g. Threaded-Binary Tree\n\n'
+        '5. Tables\n'
+        '   a. HuffmanTable'
     )
-    sys.stderr.write(f"Warning: Could not open README.md due {error}\n")
+    sys.stderr.write(f"Warning: Could not open README.md due {e}\n")
 setup(
     name='datastax',
     maintainer="Pritam Kundu",
     description='A python library to handle dataStructures',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/warmachine028/datastax',
@@ -69,39 +84,41 @@
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Science/Research",
 
         "License :: OSI Approved :: MIT License",
 
         "Operating System :: OS Independent",
 
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
 
         "Topic :: Documentation",
         "Topic :: Education :: Testing",
         "Topic :: Scientific/Engineering :: Visualization",
         "Topic :: Software Development :: Documentation",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing :: Unit",
 
         "Typing :: Typed"
     ],
     platforms=["Windows", "Linux", "Solaris", "Mac OS-X", "Unix"],
     test_suite='pytest',
     version=datastax.__version__,
-    python_requires='>=3.11',
+    python_requires='>3.11',
     packages=[
         'datastax',
         'datastax/Utils',
+        'datastax/Utils/Exceptions',
+        'datastax/Utils/Warnings',
         'datastax/Arrays',
         'datastax/Arrays/AbstractArrays',
+        'datastax/Nodes',
+        'datastax/Nodes/AbstractNodes',
         'datastax/Lists',
         'datastax/Lists/AbstractLists',
-        'datastax/trees',
-        'datastax/trees/private_trees',
+        'datastax/Trees',
+        'datastax/Trees/AbstractTrees',
+        'datastax/Tables',
+        'datastax/Tables/AbstractTables',
     ],
     author_email='pritamkundu771@gmail.com',
 )
 # python setup.py sdist bdist_wheel
```

