# Comparing `tmp/ofnodes-1.6.1.tar.gz` & `tmp/ofnodes-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.6.1.tar", max compression
+gzip compressed data, was "ofnodes-1.7.0.tar", max compression
```

## Comparing `ofnodes-1.6.1.tar` & `ofnodes-1.7.0.tar`

### file list

```diff
@@ -1,10 +1,18 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.6.1/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.6.1/README.md
--rw-r--r--   0        0        0      590 2024-04-20 03:24:00.640697 ofnodes-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.6.1/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.1/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     2820 2024-04-20 03:24:00.640697 ofnodes-1.6.1/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.6.1/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.6.1/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    28576 2024-04-20 03:24:00.640697 ofnodes-1.6.1/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.7.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.7.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-23 19:27:37.585725 ofnodes-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-22 18:07:58.574458 ofnodes-1.7.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.7.0/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.7.0/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    20313 2024-04-23 17:49:14.794379 ofnodes-1.7.0/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.7.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.7.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.7.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     2632 2024-04-23 19:26:45.294035 ofnodes-1.7.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.7.0/PKG-INFO
```

### Comparing `ofnodes-1.6.1/LICENSE` & `ofnodes-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.1/README.md` & `ofnodes-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.1/pyproject.toml` & `ofnodes-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.6.1"
+version = "1.7.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.6.1/src/ofnodes/__init__.py` & `ofnodes-1.7.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.6.1/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.7.0/src/ofnodes/components/structures/mixins.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,269 +1,256 @@
-from typing import Optional, Any
-
+from typing import Any
 from ofnodes.nodes.singlynode import SinglyNode
 
+class SearchMixin:
+    """Mixin class providing search functionality for linked lists."""
 
-class SinglyLinkedList:
-    """A class representing a singly linked list.
+    def search(self, target_data):
+        """Searches each node's data in a linked list until the first occurrence of
+        the target is found.
 
-    This class provides functionality to create and manipulate a singly linked list
-    data structure. Each node in the linked list contains a reference to the next
-    node in the sequence.
-
-    Attributes:
-        _head (Optional[SinglyNode]): The head of the linked list.
-        _tail (Optional[SinglyNode]): The tail of the linked list.
-        _target (Optional[Any]): The target data or node instance.
-
-    Examples:
-        >>> linked_list = SinglyLinkedList()
-        >>> linked_list
-        SinglyLinkedList(head=None, tail=None, target=None)
-    """
-
-    __slots__ = ('_head', '_tail', '_target',)
-
-    def __init__(self, values=None) -> None:
-        self._head: Optional[SinglyNode] = None
-        self._tail: Optional[SinglyNode] = None
-        self._target: Optional[Any|SinglyNode] = None
-        if values:
-            for value in values:
-                self.tail = value
-
-
-    @property
-    def head(self) -> SinglyNode | None:
-        """Getter property for the head of the linked list.
+        Args:
+            target_data (Any): The value to search for in the linked list.
 
         Returns:
-            SinglyNode | None: The head of the linked list, or None if the list is empty.
+            bool: True if the target value is found in the linked list, False otherwise.
+
+        Raises:
+            ValueError: If the linked list is empty.
 
         Notes:
-            The `head` property allows access to the first node in the linked list.
+            This method iterates through the linked list starting from the head node
+            and checks each node's data value for equality with the target value.
 
         Examples:
             >>> llist = SinglyLinkedList()
             >>> llist.head = "first node"
-            >>> llist.head = [42.0, True, "LGRW"]
-            >>> llist.tail = "third node added to list"
-            >>> llist
-            SinglyLinkedList(head=This node's data is 3 of type list., tail=This node's data is 24 of type str.)
-            >>> llist.tail = None
-            >>> llist
-            SinglyLinkedList(head=This node's data is 3 of type list., tail=This node's data is of type NoneType.)
-            >>> llist.head.next.data
-            'first node'
-            >>> llist.remove_tail()
-            >>> llist.tail.data
-            'third node added to list'
-        """
-        return self._head
-
-    @head.setter
-    def head(self, value: SinglyNode | Any) -> None:
+            >>> llist.head = "second node"
+            >>> llist.search("first node")
+            True
+            >>> llist.search(SinglyNode("first node"))
+            False
+            >>> llist.search("third node")
+            False
+            >>> llist.tail = "third node"
+            >>> llist.search("third node")
+            True
         """
-        Setter property for the head of the linked list.
+        if self._head is None:
+            raise ValueError("Cannot search an empty linked list.")
 
-        Args:
-            value (SinglyNode | Any): The value to be set as the head. If the value is
-                not already a SinglyNode object, it is wrapped in a SinglyNode.
-        """
-        match value:
-            case SinglyNode():
-                node = value
-            case _:
-                node = SinglyNode(value)
+        current_node = self._head
+        while current_node:
+            if current_node.data == target_data:
+                return True
+            current_node = current_node.next
+        return False
 
-        match self._head:
-            case None:
-                self._head = node
-                self._tail = node
+class RemoveMixin:
+    """Mixin class providing remove functionality for linked structures."""
 
-            case self._head:
-                setattr(node, '_next', self._head)
-                setattr(self, "_head", node)
+    def remove(self, target_data):
+        """Removes the first occurrence of a node with the specified target data from the linked structure.
 
-    @head.deleter
-    def head(self):
-        """Deleter property for the head of the linked list.
+        Args:
+            target_data (Any | Node): The data or node to be removed from the linked structure.
 
         Raises:
-            AttributeError: Deleting the `head` attribute is not allowed.
-        """
-        raise AttributeError(
-            f"{type(self).__name__}'s `head` attribute " "cannot be deleted."
-        )
-
-    @property
-    def target(self) -> SinglyNode|Any:
-        """Getter property for the node data to target in a Linked List.
+            ValueError: If the linked structure is empty.
 
         Returns:
-            target: The first node instance of the linked list containing data\
-            matching the target. If no target match, the data is assigned as passed\
-            to target.
+            None: This method does not return any value.
+
+        Removes the first occurrence of a node with the specified target data from the linked structure.
+        If the linked structure is empty, a ValueError is raised.
+
+        If the target data is found in the linked structure:
+        - If the target node is the head, the head of the linked structure is updated to the next node.
+        - If the target node is the tail, the tail of the linked structure is updated to the previous node.
+        - For any other node, the reference to the next node is adjusted to skip the target node.
 
         Notes:
-            Any data can be assigned as the target data. Each node in the
-            `SinglyLinkedList` has its data compared to the target data. The first
-            node instance data that match the target data is assigned to the `.target`
-            property. If a match is not found, the target data is stored as is in the
-            `.target` attribute.
+            This method removes only the first occurrence of the target data if multiple nodes contain the same data.
 
         Examples:
-            >>> sllist = SinglyLinkedList()
-            >>> sllist.target = '5 node'
-            Empty `SinglyLinkedList()`. Target data is assigned to SinglyLinkedList's target property.
-            >>> type(sllist.target) != SinglyNode
-            True
-            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
+            >>> linked_structure = LinkedStructure()
+            >>> list(linked_structure.insert_tail(f"{i} node") for i in range(1, 5))
             [None, None, None, None]
-            >>> sllist.target = '5 node'
-            No target matches. Target data assigned to SinglyLinkedList's target property.
-            >>> sllist.tail = '5 node'
-            >>> sllist.target = '5 node'
-            At least one target match. First target node instance is assigned to SinglyLinkedList's target property.
-            >>> type(sllist.target) == SinglyNode
-            True
-            >>> sllist.target is sllist.tail
-            True
+            >>> linked_structure.remove('0 node')
+            >>> linked_structure.target
+            '0 node'
+            >>> linked_structure.head, linked_structure.head.next, linked_structure.tail
+            (Node(data='1 node'), Node(data='2 node'), Node(data='4 node'))
+            >>> linked_structure.remove('1 node')
+            >>> linked_structure.target
+            Node(data='1 node')
+            >>> linked_structure.head, linked_structure.head.next, linked_structure.tail
+            (Node(data='2 node'), Node(data='3 node'), Node(data='4 node'))
+            >>> linked_structure.remove(linked_structure.tail)
+            >>> linked_structure.target
+            Node(data='4 node')
+            >>> linked_structure.head, linked_structure.head.next, linked_structure.tail
+            (Node(data='2 node'), Node(data='3 node'), Node(data='3 node'))
+            >>> linked_structure.head.next
+            Node(data='3 node')
+            >>> linked_structure.tail
+            Node(data='3 node')
+            >>> linked_structure.remove(linked_structure.tail)
+            >>> linked_structure.tail
+            Node(data='2 node')
+            >>> linked_structure.head.next
+            >>> linked_structure.head, linked_structure.head.next, linked_structure.tail
+            (Node(data='2 node'), None, Node(data='2 node'))
         """
-        return self._target
+        self.target = target_data  # trigger the setter
 
-    @target.setter
-    def target(self, target_data: Any | SinglyNode):
-        """Setter property for the target node data of the linked list.
+        if getattr(self._head, 'data') == self._target:
+            self.remove_head()
+            return
 
-        Args:
-            target (Any): The data for which to match to node data.
-        """
+        current_node = self._head
+        while current_node.next is not self._tail:
+            if current_node.next.data == self._target:
+                setattr(current_node, '_next', current_node.next.next)
+                return
+            current_node = current_node.next
 
-        match self._head:
-            case None:
-                raise ValueError(f"Cannot assign target data to empty {type(self).__name__}.")
+        if getattr(self._tail, 'data') == self._target:
+            self.remove_tail()
+            return
 
-            case self._head:
-                if target_data:
-                    #  TODO: data validation
-                    validated_data = target_data
-                    self._target = validated_data
-                    return
-                raise ValueError("Target data unacceptable.")
+    def remove_head(self) -> None:
+        """Removes the head node from the linked structure.
 
+            Raises:
+                ValueError: If the linked structure is empty.
 
-    @target.deleter
-    def target(self):
-        """Deleter property for the target of the linked list.
+            Returns:
+                None
 
-        Raises:
-            AttributeError: Deleting the `target` attribute is not allowed.
+            Notes:
+                - If the head node is the only node in the list, both the head and tail references are set to None.
+                - If the head node is not the only node, the head reference is updated to point to the next node.
+                TODO: overload `-` operator to support:
+                        1) `linked_structure - linked_structure.head`
+                        2) `linked_structure - linked_structure.tail`
+                        3) `linked_structure - linked_structure.spot()`
+
+            Examples:
+                >>> linked_structure = LinkedStructure()
+                >>> linked_structure
+                LinkedStructure(head=None, tail=None)
+                >>> linked_structure.head = {42: "a string"}
+                >>> linked_structure
+                LinkedStructure(head=Node(data='1 node'), tail=Node(data='1 node'))
+                >>> linked_structure.head.data[42]
+                'a string'
+                >>> linked_structure.remove_head()
+                >>> linked_structure
+                LinkedStructure(head=None, tail=None)
         """
-        raise AttributeError(
-            f"{type(self).__name__}'s `target` attribute " "cannot be deleted."
-        )
+        if self._head and self._head is self._tail:
+            self._head = None
+            self._tail = None
+            return
+        if self._head and self._head is not self._tail:
+            self._head = self._head.next
+            return
+        raise ValueError("Cannot remove head from empty list")
 
-    @property
-    def tail(self) -> SinglyNode | None:
-        """
-        Getter property for the tail of the linked list.
+    def remove_tail(self) -> None:
+        """Removes the tail node from the linked structure.
+
+        Raises:
+            ValueError: If the linked structure is empty.
 
         Returns:
-            SinglyNode | None: The tail of the linked list, or None if the list is empty.
+            None
 
         Examples:
-            >>> llist = SinglyLinkedList()
-            >>> llist
-            SinglyLinkedList(head=None, tail=None)
-            >>> llist.tail = "first node in the list"
-            >>> assert llist.tail is llist.head
-            >>> assert llist.next is None
-            >>> assert llist.head.next is None
-            >>> llist.tail
-            >>> llist.tail = "new tail"
-            >>> assert llist.head.next is llist.tail
-            >>> llist
-            SinglyLinkedList(head=This node's data is 22 of type str., tail=This node's data is 8 of type str.)
-            >>> llist.head, llist.tail
-            (SinglyNode(data='first node in the list'), SinglyNode(data='new tail'))
-        """
-        return self._tail
-
-    @tail.setter
-    def tail(self, value: SinglyNode | Any) -> None:
-        """Setter property for the tail of the linked list.
-
-        Args:
-            value (SinglyNode | Any): The value to be set as the tail. If the value is
-                not already a SinglyNode object, it is wrapped in a SinglyNode.
-
-        Notes:
-            Setting the `tail` property allows modification of the last node in the linked list.
-        """
-        match value:
-            case SinglyNode():
-                node = value
-            case _:
-                node = SinglyNode(value)
-
+            >>> linked_structure = LinkedStructure()
+            >>> linked_structure
+            LinkedStructure(head=None, tail=None)
+            >>> linked_structure.head = True
+            >>> linked_structure
+            LinkedStructure(head=Node(data=True), tail=Node(data=True))
+            >>> linked_structure.tail = ['strings', Node(lambda x: str(x)*2)]
+            >>> linked_structure
+            LinkedStructure(head=Node(data=True), tail=Node(data=['strings', Node(data=<function <lambda> at 0x74a9932a2fc0>)]))
+            >>> linked_structure.tail
+            Node(data=['strings', Node(data=<function <lambda> at 0x74a9932a2fc0>)])
+            >>> linked_structure.tail.data[1].data
+            <function <lambda> at 0x74a9932a2fc0>
+            >>> x = linked_structure.tail.data[1].data
+            >>> x("skrrt")
+            'skrrtskrrt'
+            >>> linked_structure.remove_tail()
+            >>> x("skrrt")
+            'skrrtskrrt'
+            >>> linked_structure.tail
+            Node(data=True)
+            """
         match self._head:
             case None:
-                setattr(self, "_head", node)
-                setattr(self, "_tail", node)
+                raise ValueError("Cannot remove tail from empty list")
             case self._head:
                 if not getattr(self._head, "_next"):
                     # it's a one node list
-                    setattr(self._head, "_next", node)
-                    setattr(self, "_tail", node)
+                    setattr(self, "_head", None)
+                    setattr(self, "_tail", None)
+                    return
+                if getattr(self._head, "next") is self._tail:
+                    # there are two nodes
+                    setattr(self, "_tail", self._head)
+                    setattr(self._tail, "_next", None)
                     return
-                # there're more than one node
-                setattr(self._tail, "_next", node)
-                setattr(self, "_tail", node)
-
-    @tail.deleter
-    def tail(self):
-        """Deleter property for the tail of the linked list.
+                # there are more than two nodes
+                node = self._head
+                # find second to last node
+                while getattr(node, "_next") and getattr(node._next, "_next"):
+                    if getattr(node._next, "_next") is self._tail:
+                        node = getattr(node, "_next")  # target found
+                        break
+                    node = getattr(node, "_next")  # keep looking
+                setattr(node, "_next", None)  # point the second to last node to None
+                setattr(self, "_tail", node)  # assign tail to the node
 
-        Raises:
-            AttributeError: Deleting the `tail` attribute is not allowed.
+class PrintMixin:
+    """Mixin class providing node data print functionality"""
+    def print_node_data(self) -> None:
+        """Traverse the linked data structure and print the data attribute of each node.
+
+        Returns:
+            None
+
+        Notes:
+            This method iterates through the linked data structure starting from the head node and prints the data attribute of each node
+            until the end of the linked structure is reached.
+
+        Examples:
+            >>> sllist = SinglyLinkedList()
+            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
+            [None, None, None, None]
+            >>> sllist.head
+            SinglyNode(data='1 node')
+            >>> sllist.tail
+            SinglyNode(data='4 node')
+            >>> sllist.print_node_data()
+            1 node
+            2 node
+            3 node
+            4 node
         """
-        raise AttributeError(
-            f"{type(self).__name__}'s `tail` attribute " "cannot be deleted."
-        )
-
-    def __repr__(self) -> str:
-        #return f"{type(self).__name__}(head={type(self.head).__name__}, tail={self.tail})"
-        if not self._head:
-            return "SinglyLinkedList()"
-        node = self._head
-        nodes = []
-        while node:
-            nodes.append(repr(node.data))
-            node = node.next
-        return f"{type(self).__name__}([" + ', '.join(nodes) + "])"
-
-    def __str__(self) -> str:
-        if not self._head:
-            return "Empty Singly Linked List"
-        node = self._head
-        nodes = []
-        while node:
-            nodes.append(str(node.data))
-            node = node.next
-        return ' -> '.join(nodes)
-            
-    def __dir__(self) -> list[str]:
-        # Get the list of attributes and methods from the parent classes
-        parent_dir = set(super().__dir__())
-        # Filter out private attributes and methods
-        parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
-        # Return a sorted list of all attributes and methods
-        return sorted(parent_dir)
+        current_node = self._head
+        while current_node:
+            print(current_node.data)
+            current_node = current_node.next
 
+class InsertHeadMixin:
+    """Mixin providing functionality to insert a node at the beginning of a linked structure."""
     def insert_head(self, data: Any) -> None:
         """ Inserts a new node with the provided data at the head of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
@@ -300,14 +287,16 @@
             [None, None, None, None]
             >>> llist.head = "to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`'), SinglyNode(data='4 node'), SinglyNode(data='1 node'))
         """
         self.head = data  # trigger the head setter
 
+class InsertTailMixin:
+    """Mixin providing functionality to insert a node at the end of a linked structure."""
     def insert_tail(self, data: Any) -> None:
         """Inserts a new node with the provided data at the tail of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
@@ -350,14 +339,16 @@
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
+class InsertAfterTargetMixin:
+    """Mixin providing functionality to insert a node after a target node in a linked structure."""
     def insert_after_target(self, target_data: Any, data_to_insert: Any) -> bool:
         """
         Inserts a new node containing the specified data after the first occurrence
         of the target data in the linked list.
 
         Args:
             target_data (Any): The data value to search for in the linked list.
@@ -399,14 +390,16 @@
         # check tail
         if getattr(self._tail, 'data') == self.target:
             self.tail = data_to_insert  # # trigger the setter, tail property will validate input
             return True
         # no target match
         return False
 
+class InsertBeforeTargetMixin:
+    """Mixin providing functionality to insert a node before a target node in a linked structure."""
     def insert_before_target(self, target_data: Any, data_to_insert: Any) -> bool:
         """
         Inserts a new node containing the specified data before the first occurrence
         of the target data in the linked list.
 
         Args:
             target_data: The data value to search for in the linked list or the reference to the node.
@@ -453,247 +446,8 @@
             # check after head through tail
             if current_node.next.data == self._target:  # peek
                 new_node = SinglyNode(data_to_insert)  # SinglyNode() will validate data_to_insert
                 setattr(new_node, '_next', current_node.next)  # insert_before()
                 setattr(current_node, '_next', new_node)  # insert before()
                 return True
             current_node = getattr(current_node, 'next')  # traversal
-        return False
-
-
-
-    def search(self, target_data):
-        """Searches each node's data in a linked list until the first occurrence of
-        the target is found.
-
-        Args:
-            target_data (Any): The value to search for in the linked list.
-
-        Returns:
-            bool: True if the target value is found in the linked list, False otherwise.
-
-        Raises:
-            ValueError: If the linked list is empty.
-
-        Notes:
-            This method iterates through the linked list starting from the head node
-            and checks each node's data value for equality with the target value.
-
-        Examples:
-            >>> llist = SinglyLinkedList()
-            >>> llist.head = "first node"
-            >>> llist.head = "second node"
-            >>> llist.search("first node")
-            True
-            >>> llist.search(SinglyNode("first node"))
-            False
-            >>> llist.search("third node")
-            False
-            >>> llist.tail = "third node"
-            >>> llist.search("third node")
-            True
-        """
-        self.target = target_data  # trigger the setter
-        current_node = self._head
-        while current_node:
-            if current_node.data == self._target:
-                return True
-            current_node = current_node.next
-        return False
-
-    def remove(self, target_data: Any | SinglyNode) -> None:
-        """Removes the first occurrence of a node with the specified target data from the linked list.
-
-        Args:
-            target_data (Any | SinglyNode): The data or node to be removed from the linked list.
-
-        Raises:
-            ValueError: If the linked list is empty.
-
-        Returns:
-            None: This method does not return any value.
-
-        Removes the first occurrence of a node with the specified target data from the linked list.
-        If the linked list is empty, a ValueError is raised.
-
-        If the target data is found in the linked list:
-        - If the target node is the head, the head of the linked list is updated to the next node.
-        - If the target node is the tail, the tail of the linked list is updated to the previous node.
-        - For any other node, the reference to the next node is adjusted to skip the target node.
-        Notes:
-            This method removes only the first occurrence of the target data if multiple nodes contain the same data.
-
-        Examples:
-            >>> sllist = SinglyLinkedList()
-            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
-            [None, None, None, None]
-            >>> sllist.remove('0 node')
-            >>> sllist.target
-            '0 node'
-            >>> sllist.head, sllist.head.next, sllist.tail
-            (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
-            >>> sllist.remove('1 node')
-            >>> sllist.target
-            SinglyNode(data='1 node')
-            >>> sllist.head, sllist.head.next, sllist.tail
-            (SinglyNode(data='2 node'), SinglyNode(data='3 node'), SinglyNode(data='4 node'))
-            >>> sllist.remove(sllist.tail)
-            >>> sllist.target
-            SinglyNode(data='4 node')
-            >>> sllist.head, sllist.head.next, sllist.tail
-            (SinglyNode(data='2 node'), SinglyNode(data='3 node'), SinglyNode(data='3 node'))
-            >>> sllist.head.next
-            SinglyNode(data='3 node')
-            >>> sllist.tail
-            SinglyNode(data='3 node')
-            >>> sllist.remove(sllist.tail)
-            >>> sllist.tail
-            SinglyNode(data='2 node')
-            >>> sllist.head.next
-            >>> sllist.head, sllist.head.next, sllist.tail
-            (SinglyNode(data='2 node'), None, SinglyNode(data='2 node'))
-        """
-
-        self.target = target_data  # trigger the setter
-
-        if getattr(self._head, 'data') == self._target:
-            # node = self._head  # the node to be removed
-            self.remove_head()
-            return #node
-
-        current_node = getattr(self, '_head')  # traversal
-        while current_node.next is not self._tail:  # traversal (tail already checked)
-            if current_node.next.data == self._target:  # peek
-                #node = current_node.next  # the node to be removed
-                setattr(current_node, '_next', current_node.next.next)  # remove()
-                return #node
-            current_node = current_node.next  # traversal
-
-        if getattr(self._tail, 'data') == self._target:
-            # node = self._tail  # the node to be removed
-            self.remove_tail()
-            return #node
-
-    def remove_head(self) -> None:
-        """Removes the head node from the linked list.
-
-        Raises:
-            ValueError: If the linked list is empty.
-
-        Returns:
-            None
-
-        Notes:
-            - If the head node is the only node in the list, both the head and tail references are set to None.
-            - If the head node is not the only node, the head reference is updated to point to the next node.
-            TODO: overload `-` operator to support:
-                    1) `linked_list - linked_list.head`
-                    2) `linked_list - linked_list.tail`
-                    3) `linked_list - linked_list.spot()`
-
-        Examples:
-            >>> sllist = SinglyLinkedList()
-            >>> sllist
-            SinglyLinkedList(head=None, tail=None)
-            >>> sllist.head = {42: "a string"}
-            >>> sllist
-            SinglyLinkedList(head=This node's data is 1 of type dict., tail=This node's data is 1 of type dict.)
-            >>> sllist.head.data[42]
-            'a string'
-            >>> sllist.remove_head()
-            >>> sllist
-            SinglyLinkedList(head=None, tail=None)
-        """
-        if self._head and self._head is self._tail:
-            self._head = None
-            self._tail = None
-            return
-        if self._head and self._head is not self._tail:
-            self._head = self._head.next
-            return
-        raise ValueError("Cannot remove head from empty list")
-
-    def remove_tail(self) -> None:
-        """Removes the tail node from the linked list.
-
-        Raises:
-            ValueError: If the linked list is empty.
-
-        Returns:
-            None
-
-        Examples:
-            >>> linked_list = SinglyLinkedList()
-            >>> linked_list
-            SinglyLinkedList(head=None, tail=None)
-            >>> linked_list.head = True
-            >>> linked_list
-            SinglyLinkedList(head=This node's data is of type bool., tail=This node's data is of type bool.)
-            >>> linked_list.tail = ['strings', SinglyNode(lambda x: str(x)*2)]
-            >>> linked_list
-            SinglyLinkedList(head=This node's data is of type bool., tail=This node's data is 2 of type list.)
-            >>> linked_list.tail
-            SinglyNode(data=['strings', SinglyNode(data=<function <lambda> at 0x74a9932a2fc0>)])
-            >>> linked_list.tail.data[1].data
-            <function <lambda> at 0x74a9932a2fc0>
-            >>> x = linked_list.tail.data[1].data
-            >>> x("skrrt")
-            'skrrtskrrt'
-            >>> linked_list.remove_tail()
-            >>> x("skrrt")
-            'skrrtskrrt'
-            >>> linked_list.tail
-            SinglyNode(data=True)
-            """
-        match self._head:
-            case None:
-                raise ValueError("Cannot remove tail from empty list")
-            case self._head:
-                if not getattr(self._head, "_next"):
-                    # it's a one node list
-                    setattr(self, "_head", None)
-                    setattr(self, "_tail", None)
-                    return
-                if getattr(self._head, "next") is self._tail:
-                    # there are two nodes
-                    setattr(self, "_tail", self._head)
-                    setattr(self._tail, "_next", None)
-                    return
-                # there are more than two nodes
-                node = self._head
-                # find second to last node
-                while getattr(node, "_next") and getattr(node._next, "_next"):
-                    if getattr(node._next, "_next") is self._tail:
-                        node = getattr(node, "_next")  # target found
-                        break
-                    node = getattr(node, "_next")  # keep looking
-                setattr(node, "_next", None)  # point the second to last node to None
-                setattr(self, "_tail", node)  # assign tail to the node
-
-    def print_node_data(self) -> None:
-        """Traverse the linked list and print the data attribute of each node.
-
-        Returns:
-            None
-
-        Notes:
-            This method iterates through the linked list starting from the head node and prints the data attribute of each node
-            until the end of the list is reached.
-
-        Examples:
-            >>> sllist = SinglyLinkedList()
-            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
-            [None, None, None, None]
-            >>> sllist.head
-            SinglyNode(data='1 node')
-            >>> sllist.tail
-            SinglyNode(data='4 node')
-            >>> sllist.print_node_data()
-            1 node
-            2 node
-            3 node
-            4 node
-        """
-        current_node = self._head
-        while current_node:
-            print(current_node.data)
-            current_node = current_node.next
+        return False
```

### Comparing `ofnodes-1.6.1/PKG-INFO` & `ofnodes-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.6.1
+Version: 1.7.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

