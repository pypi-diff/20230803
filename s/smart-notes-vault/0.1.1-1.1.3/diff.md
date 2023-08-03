# Comparing `tmp/smart_notes_vault-0.1.1.tar.gz` & `tmp/smart_notes_vault-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_notes_vault-0.1.1.tar", last modified: Wed Aug  2 12:33:46 2023, max compression
+gzip compressed data, was "smart_notes_vault-1.1.3.tar", last modified: Thu Aug  3 12:29:15 2023, max compression
```

## Comparing `smart_notes_vault-0.1.1.tar` & `smart_notes_vault-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      473 2023-08-02 12:33:46.270642 smart_notes_vault-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-08-02 12:01:22.950382 smart_notes_vault-0.1.1/readme.md
--rw-r--r--   0        0        0      116 2023-08-02 12:23:58.809226 smart_notes_vault-0.1.1/snv/__init__.py
--rw-r--r--   0        0        0    12545 2023-08-02 12:23:58.812753 smart_notes_vault-0.1.1/snv/classes.py
--rw-r--r--   0        0        0      829 2023-08-02 12:23:58.814755 smart_notes_vault-0.1.1/snv/io.py
--rw-r--r--   0        0        0     2142 2023-08-02 12:23:58.810227 smart_notes_vault-0.1.1/snv/md.py
--rw-r--r--   0        0        0        0 2023-08-02 12:01:22.950382 smart_notes_vault-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2092 2023-08-02 12:23:58.811739 smart_notes_vault-0.1.1/tests/conf_vault.py
--rw-r--r--   0        0        0       27 2023-08-02 12:01:22.956078 smart_notes_vault-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2681 2023-08-02 12:23:58.813754 smart_notes_vault-0.1.1/tests/test_class_note.py
--rw-r--r--   0        0        0     2851 2023-08-02 12:23:58.811739 smart_notes_vault-0.1.1/tests/test_class_vault.py
--rw-r--r--   0        0        0      775 2023-08-02 12:23:58.815768 smart_notes_vault-0.1.1/tests/test_io.py
--rw-r--r--   0        0        0     1898 2023-08-02 12:23:58.815768 smart_notes_vault-0.1.1/tests/test_md.py
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 smart_notes_vault-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      474 2023-08-03 12:29:15.414281 smart_notes_vault-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2521 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/readme.md
+-rw-r--r--   0        0        0      111 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/snv/__init__.py
+-rw-r--r--   0        0        0    12215 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/snv/classes.py
+-rw-r--r--   0        0        0      799 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/snv/io.py
+-rw-r--r--   0        0        0     2086 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/snv/md.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:29:10.882347 smart_notes_vault-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2008 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/tests/conf_vault.py
+-rw-r--r--   0        0        0       26 2023-08-03 12:29:10.859347 smart_notes_vault-1.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     2591 2023-08-03 12:29:10.860348 smart_notes_vault-1.1.3/tests/test_class_note.py
+-rw-r--r--   0        0        0     2746 2023-08-03 12:29:10.860348 smart_notes_vault-1.1.3/tests/test_class_vault.py
+-rw-r--r--   0        0        0      745 2023-08-03 12:29:10.860348 smart_notes_vault-1.1.3/tests/test_io.py
+-rw-r--r--   0        0        0     1817 2023-08-03 12:29:10.860348 smart_notes_vault-1.1.3/tests/test_md.py
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 smart_notes_vault-1.1.3/PKG-INFO
```

### Comparing `smart_notes_vault-0.1.1/snv/classes.py` & `smart_notes_vault-1.1.3/snv/classes.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-from snv.md import extract_header, extract_markdown
-
-from pathlib import Path
-from yaml import unsafe_load, dump
-from glob import glob
-
-
-
-class Note:
-
-    def __init__(self, filename: str, content: str = None):
-        """Initializes a new Note object.
-
-        Args:
-            filename (str): The name of the note, including the .md extension.
-            content (str, optional): The content of the note. Defaults to None.
-
-        Raises:
-            ValueError: If the name does not end in .md.
-            TypeError: If name is not a string.
-        """
-        try:
-            if not filename.endswith(".md"):
-                if __debug__:
-                    print(f"Add suffix '.md' to name {filename}")
-                filename += '.md'
-            if not isinstance(filename, str):
-                raise TypeError("Note filename must be a string")
-            path = Path(filename)
-            if not path.is_file:
-                raise ValueError(f"filename {filename!r} is not valid file path")
-            if path.is_absolute():
-                raise ValueError(
-                    f"filename {filename!r} is not relative to vault folder")
-            self.__path = path
-
-            if content:
-                if not isinstance(content, str):
-                    raise TypeError(f"content is not str but {type(content)}")
-            self.__content = content
-        except OSError as exc:
-            raise ValueError(f"filename {filename!r} is not valid path") from exc
-
-    @property
-    def filename(self) -> str:
-        """Returns the name of the note with the .md extension.
-
-        Returns:
-            str: The name of the note.
-        """
-        return str(self.__path)
-
-    @property
-    def content(self) -> str:
-        """Returns the content of the note as a string.
-
-        Returns:
-            str: The content of the note.
-        """
-        return self.__content
-
-    def __str__(self) -> str:
-        return self.__content
-
-    def __repr__(self) -> str:
-        if not self.content:
-            content = type(self.content)
-        else:
-            content = self.content if len(
-                self.content) < 32 else f"{self.content[:32]} ... {len(self.content)} total size"
-        return f"Note(filename={self.filename!r}, content='{content!r}')"
-
-    @property
-    def header(self):
-        if not hasattr(self, "_Note__header"):
-            extract = extract_header(self.content)
-            self.__header = Note.Header(self, extract)
-        return self.__header
-
-    @property
-    def markdown(self):
-        if not hasattr(self, "_Note__markdown"):
-            c = self.content
-            extract = extract_markdown(c)
-            self.__markdown = extract
-        return self.__markdown
-
-    class Header:
-
-        COMMENT_LABEL = "#"
-        KEY_TAGS = "tags"
-
-        def __init__(self, note: "Note", header: str):
-            if not note:
-                raise ValueError("Parameter note is None.")
-            if not isinstance(note, Note):
-                raise TypeError(
-                    f"Parameter note is not type 'Note' but {type(note)}.")
-            self.__note = note
-
-            if header:
-                if not isinstance(header, str):
-                    raise TypeError(
-                        f"Parameter note is not type 'str' but {type(header)}.")
-            self.__header = header
-
-        def __str__(self) -> str:
-            return self.__header or ""
-
-        def __repr__(self) -> str:
-            return f"Note.Header(note={self.__note!r}, len={len(self.__header or '')})"
-
-        def __as_dict(self) -> dict:
-            try:
-                if not self.__header:
-                    return dict()
-                # Remove comment lines, the yaml library can't work with it
-                data = '\n'.join(filter(
-                    lambda line: not line.strip().startswith(self.COMMENT_LABEL),
-                    self.__header.splitlines()
-                ))
-                return unsafe_load(data[4:-4])
-            except Exception as exc:
-                raise ValueError(
-                    f"Can not parse header {self.__header!r}") from exc
-
-        def tags(self) -> list[str]:
-            """Return the list of tags for this note header."""
-            try:
-                data = self.__as_dict()
-                return tuple(data.get(self.KEY_TAGS, tuple()))
-            except Exception as exc:
-                raise ValueError(
-                    f"Can not parse header {self.__header!r}") from exc
-
-        def remove_tag(self, tag: str) -> 'Note':
-            """Remove a tag from the note metadata.  
-
-            Removes the given ptag from the list of tags in the note metadata.
-            If the tag does not exist, no changes are made.
-
-            Args:
-                tag (str): The tag to remove.
-
-            Returns:
-                Note: The Note object.
-
-            Raises:
-                ValueError: If the note metadata cannot be parsed.
-            """
-            try:
-                data = self.__as_dict()
-                if self.KEY_TAGS not in data:
-                    return self.__note
-                tags = list(data[self.KEY_TAGS])
-                if tag not in tags:
-                    return self.__note
-                
-                tags.remove(tag)
-                data[self.KEY_TAGS] = tags
-                comments = '\n'.join(
-                    map(str.strip,
-                        filter(lambda line: line.strip().startswith(self.COMMENT_LABEL),
-                               self.__header.splitlines()
-                               )
-                        )
-                )
-                if comments:
-                    comments += '\n'
-                new_header = f"---\n{comments}{dump(data)}---\n"
-                old_markdown = extract_markdown(str(self.__note))
-                filename = self.__note.filename
-                return Note(
-                    filename,
-                    content=new_header+old_markdown
-                )
-            except Exception as exc:
-                raise ValueError(
-                    f"Can remove tag {tag} from header {self.__header!r}") from exc
-
-class Vault:
-    """Represents a collection of smart notes stored in a folder.
-
-    A Vault is responsible for opening notes, storing new notes, and searching existing notes.
-
-    ## Example of usage
-    - Creating a Vault from a './vault_dir' path.
-    - Checking the length of the Vault is 3 notes.
-    - Accessing the first note.
-    - Checking the name of the first note is 'note1'.
-
-    >>> vault = Vault(Path('./vault_dir'))
-    >>> len(vault)
-    3
-    >>> note = vault[0]
-    >>> note.name
-    'note1'
-
-    Attributes:
-        root_dir (Path): The path to the folder containing the Vault.
-    """
-
-    def __init__(self, root_dir: Path, *, create_root_dir: bool = False) -> None:
-        """Initialize a new Vault.
-
-        Args:
-            root_dir (Path): The path to the directory containing the Vault.
-            create_not_exists_dir (bool, optional): Whether to create the directory if it does not exist, but not parents!!!. Defaults to False.
-
-        Raises:
-            ValueError: If root_dir is None.
-            TypeError: If root_dir is not a Path.
-            FileNotFoundError: If root_dir does not exist and create_root_dir is False.
-            NotADirectoryError: If root_dir is not a directory.
-        """
-
-        if not root_dir:
-            raise ValueError("root_dir cannot be None")
-        if not isinstance(root_dir, Path):
-            raise TypeError(f"root_dir must be a Path, got {type(root_dir)}")
-        if not root_dir.exists():
-            if create_root_dir:
-                if __debug__:
-                    print(f"root_dir {root_dir} is created.")
-                root_dir.mkdir()
-            else:
-                raise FileNotFoundError(f"root_dir {root_dir} does not exist")
-        if not root_dir.is_dir():
-            raise NotADirectoryError(f"root_dir {root_dir} is not a directory")
-        self.__root_dir = root_dir
-
-    def __repr__(self):
-        return f"Vault(root_dir={self.__root_dir!r})"
-
-    def __str__(self):
-        return f"Vault at {self.__root_dir}"
-
-    @property
-    def root_dir(self) -> Path:
-        return self.__root_dir
-
-    def open_note(self, filename: str, *, deep_search=True) -> Note | list[Note]:
-        """Create instance of a note or notes from the vault.  
-
-        Searches for notes matching the given filename. By default, performs a deep, recursive search 
-        through subdirectories. If multiple notes share the same name, returns a list of notes. 
-        Otherwise, returns a single Note object.
-
-        Args: 
-            filename (str): The name of the note(s) to open.
-            deep_search (bool, optional): Whether to search recursively through subdirectories. Defaults to True.
-        Returns: 
-            Note or list[Note]: Either a single Note object or a list of Note objects.
-        Raises:
-            ValueError: If the note could not be opened.
-        """
-        try:
-            if not filename.endswith(".md"):
-                filename += '.md'
-            search = f"**/{filename}" if deep_search else filename
-            if found := glob(search, root_dir=self.root_dir, recursive=deep_search):
-                if __debug__:
-                    print(f"For name {filename} found: {found} files.")
-                notes = []
-                for file in found:
-                    full_path = self.root_dir / file
-                    assert full_path.is_relative_to(
-                        self.root_dir), f"File {full_path} is outside vault root directory."
-
-                    with open(full_path, mode="r", encoding="utf-8") as f:
-                        note = Note(file, f.read())
-                        notes.append(note)
-                return notes[0] if len(notes) == 1 else notes
-            else:
-                return Note(filename, None)
-        except Exception as exc:
-            raise ValueError(f"Open note {filename} failed.") from exc
-
-    def find_note_by_path(self, path_expression: str, recursive=True) -> list[Note]:
-        """
-        Retrieve a list of 'Note' objects based on a given 'path_expression' that can be a pattern
-        representing the location of the desired notes. By default, the search is performed recursively
-        through subdirectories unless 'recursive' is set to False.
-
-        Args: 
-            path_expression: A string representing the pattern used to locate the desired notes.
-            recursive: A boolean indicating whether the search should be performed recursively through
-                        subdirectories. Defaults to True.
-        Returns: 
-            A list of 'Note' objects matching the given 'filename'.
-
-        Raises: 
-            ValueError: If the provided 'path_expression' is not valid.
-        """
-        try:
-            if not path_expression.endswith(".md"):
-                path_expression += '.md'
-            if recursive and not path_expression.startswith("**/"):
-                path_expression = "**/" + path_expression
-
-            files = glob(path_expression, root_dir=self.root_dir,
-                         recursive=recursive)
-            return [self.open_note(file, deep_search=False) for file in files]
-
-        except Exception as exc:
-            raise ValueError(
-                f"Paremeter {path_expression} is nor valid.") from exc
-
-    def save_note(self, note: "Note"):
-        """Persist a note to the vault.  
-
-        Stores the note content to a file named after the note's filename attribute.
-        If the filename does not end in .md, .md is appended. 
-
-        Args:
-            note (Note): The note to be stored.
-
-        Raises:
-            ValueError: If the note could not be saved.
-        """
-        try:
-            filename = note.filename
-            if not filename.endswith(".md"):
-                filename += '.md'
-            filename = self.root_dir / filename
-
-            with open(filename, mode="w", encoding="utf-8") as f:
-                f.write(str(note))
-        except Exception as exc:
-            raise ValueError(
+from snv.md import extract_header, extract_markdown
+
+from pathlib import Path
+from yaml import unsafe_load, dump
+from glob import glob
+
+
+
+class Note:
+
+    def __init__(self, filename: str, content: str = None):
+        """Initializes a new Note object.
+
+        Args:
+            filename (str): The name of the note, including the .md extension.
+            content (str, optional): The content of the note. Defaults to None.
+
+        Raises:
+            ValueError: If the name does not end in .md.
+            TypeError: If name is not a string.
+        """
+        try:
+            if not filename.endswith(".md"):
+                if __debug__:
+                    print(f"Add suffix '.md' to name {filename}")
+                filename += '.md'
+            if not isinstance(filename, str):
+                raise TypeError("Note filename must be a string")
+            path = Path(filename)
+            if not path.is_file:
+                raise ValueError(f"filename {filename!r} is not valid file path")
+            if path.is_absolute():
+                raise ValueError(
+                    f"filename {filename!r} is not relative to vault folder")
+            self.__path = path
+
+            if content:
+                if not isinstance(content, str):
+                    raise TypeError(f"content is not str but {type(content)}")
+            self.__content = content
+        except OSError as exc:
+            raise ValueError(f"filename {filename!r} is not valid path") from exc
+
+    @property
+    def filename(self) -> str:
+        """Returns the name of the note with the .md extension.
+
+        Returns:
+            str: The name of the note.
+        """
+        return str(self.__path)
+
+    @property
+    def content(self) -> str:
+        """Returns the content of the note as a string.
+
+        Returns:
+            str: The content of the note.
+        """
+        return self.__content
+
+    def __str__(self) -> str:
+        return self.__content
+
+    def __repr__(self) -> str:
+        if not self.content:
+            content = type(self.content)
+        else:
+            content = self.content if len(
+                self.content) < 32 else f"{self.content[:32]} ... {len(self.content)} total size"
+        return f"Note(filename={self.filename!r}, content='{content!r}')"
+
+    @property
+    def header(self):
+        if not hasattr(self, "_Note__header"):
+            extract = extract_header(self.content)
+            self.__header = Note.Header(self, extract)
+        return self.__header
+
+    @property
+    def markdown(self):
+        if not hasattr(self, "_Note__markdown"):
+            c = self.content
+            extract = extract_markdown(c)
+            self.__markdown = extract
+        return self.__markdown
+
+    class Header:
+
+        COMMENT_LABEL = "#"
+        KEY_TAGS = "tags"
+
+        def __init__(self, note: "Note", header: str):
+            if not note:
+                raise ValueError("Parameter note is None.")
+            if not isinstance(note, Note):
+                raise TypeError(
+                    f"Parameter note is not type 'Note' but {type(note)}.")
+            self.__note = note
+
+            if header:
+                if not isinstance(header, str):
+                    raise TypeError(
+                        f"Parameter note is not type 'str' but {type(header)}.")
+            self.__header = header
+
+        def __str__(self) -> str:
+            return self.__header or ""
+
+        def __repr__(self) -> str:
+            return f"Note.Header(note={self.__note!r}, len={len(self.__header or '')})"
+
+        def __as_dict(self) -> dict:
+            try:
+                if not self.__header:
+                    return dict()
+                # Remove comment lines, the yaml library can't work with it
+                data = '\n'.join(filter(
+                    lambda line: not line.strip().startswith(self.COMMENT_LABEL),
+                    self.__header.splitlines()
+                ))
+                return unsafe_load(data[4:-4])
+            except Exception as exc:
+                raise ValueError(
+                    f"Can not parse header {self.__header!r}") from exc
+
+        def tags(self) -> list[str]:
+            """Return the list of tags for this note header."""
+            try:
+                data = self.__as_dict()
+                return tuple(data.get(self.KEY_TAGS, tuple()))
+            except Exception as exc:
+                raise ValueError(
+                    f"Can not parse header {self.__header!r}") from exc
+
+        def remove_tag(self, tag: str) -> 'Note':
+            """Remove a tag from the note metadata.  
+
+            Removes the given ptag from the list of tags in the note metadata.
+            If the tag does not exist, no changes are made.
+
+            Args:
+                tag (str): The tag to remove.
+
+            Returns:
+                Note: The Note object.
+
+            Raises:
+                ValueError: If the note metadata cannot be parsed.
+            """
+            try:
+                data = self.__as_dict()
+                if self.KEY_TAGS not in data:
+                    return self.__note
+                tags = list(data[self.KEY_TAGS])
+                if tag not in tags:
+                    return self.__note
+                
+                tags.remove(tag)
+                data[self.KEY_TAGS] = tags
+                comments = '\n'.join(
+                    map(str.strip,
+                        filter(lambda line: line.strip().startswith(self.COMMENT_LABEL),
+                               self.__header.splitlines()
+                               )
+                        )
+                )
+                if comments:
+                    comments += '\n'
+                new_header = f"---\n{comments}{dump(data)}---\n"
+                old_markdown = extract_markdown(str(self.__note))
+                filename = self.__note.filename
+                return Note(
+                    filename,
+                    content=new_header+old_markdown
+                )
+            except Exception as exc:
+                raise ValueError(
+                    f"Can remove tag {tag} from header {self.__header!r}") from exc
+
+class Vault:
+    """Represents a collection of smart notes stored in a folder.
+
+    A Vault is responsible for opening notes, storing new notes, and searching existing notes.
+
+    ## Example of usage
+    - Creating a Vault from a './vault_dir' path.
+    - Checking the length of the Vault is 3 notes.
+    - Accessing the first note.
+    - Checking the name of the first note is 'note1'.
+
+    >>> vault = Vault(Path('./vault_dir'))
+    >>> len(vault)
+    3
+    >>> note = vault[0]
+    >>> note.name
+    'note1'
+
+    Attributes:
+        root_dir (Path): The path to the folder containing the Vault.
+    """
+
+    def __init__(self, root_dir: Path, *, create_root_dir: bool = False) -> None:
+        """Initialize a new Vault.
+
+        Args:
+            root_dir (Path): The path to the directory containing the Vault.
+            create_not_exists_dir (bool, optional): Whether to create the directory if it does not exist, but not parents!!!. Defaults to False.
+
+        Raises:
+            ValueError: If root_dir is None.
+            TypeError: If root_dir is not a Path.
+            FileNotFoundError: If root_dir does not exist and create_root_dir is False.
+            NotADirectoryError: If root_dir is not a directory.
+        """
+
+        if not root_dir:
+            raise ValueError("root_dir cannot be None")
+        if not isinstance(root_dir, Path):
+            raise TypeError(f"root_dir must be a Path, got {type(root_dir)}")
+        if not root_dir.exists():
+            if create_root_dir:
+                if __debug__:
+                    print(f"root_dir {root_dir} is created.")
+                root_dir.mkdir()
+            else:
+                raise FileNotFoundError(f"root_dir {root_dir} does not exist")
+        if not root_dir.is_dir():
+            raise NotADirectoryError(f"root_dir {root_dir} is not a directory")
+        self.__root_dir = root_dir
+
+    def __repr__(self):
+        return f"Vault(root_dir={self.__root_dir!r})"
+
+    def __str__(self):
+        return f"Vault at {self.__root_dir}"
+
+    @property
+    def root_dir(self) -> Path:
+        return self.__root_dir
+
+    def open_note(self, filename: str, *, deep_search=True) -> Note | list[Note]:
+        """Create instance of a note or notes from the vault.  
+
+        Searches for notes matching the given filename. By default, performs a deep, recursive search 
+        through subdirectories. If multiple notes share the same name, returns a list of notes. 
+        Otherwise, returns a single Note object.
+
+        Args: 
+            filename (str): The name of the note(s) to open.
+            deep_search (bool, optional): Whether to search recursively through subdirectories. Defaults to True.
+        Returns: 
+            Note or list[Note]: Either a single Note object or a list of Note objects.
+        Raises:
+            ValueError: If the note could not be opened.
+        """
+        try:
+            if not filename.endswith(".md"):
+                filename += '.md'
+            search = f"**/{filename}" if deep_search else filename
+            if found := glob(search, root_dir=self.root_dir, recursive=deep_search):
+                if __debug__:
+                    print(f"For name {filename} found: {found} files.")
+                notes = []
+                for file in found:
+                    full_path = self.root_dir / file
+                    assert full_path.is_relative_to(
+                        self.root_dir), f"File {full_path} is outside vault root directory."
+
+                    with open(full_path, mode="r", encoding="utf-8") as f:
+                        note = Note(file, f.read())
+                        notes.append(note)
+                return notes[0] if len(notes) == 1 else notes
+            else:
+                return Note(filename, None)
+        except Exception as exc:
+            raise ValueError(f"Open note {filename} failed.") from exc
+
+    def find_note_by_path(self, path_expression: str, recursive=True) -> list[Note]:
+        """
+        Retrieve a list of 'Note' objects based on a given 'path_expression' that can be a pattern
+        representing the location of the desired notes. By default, the search is performed recursively
+        through subdirectories unless 'recursive' is set to False.
+
+        Args: 
+            path_expression: A string representing the pattern used to locate the desired notes.
+            recursive: A boolean indicating whether the search should be performed recursively through
+                        subdirectories. Defaults to True.
+        Returns: 
+            A list of 'Note' objects matching the given 'filename'.
+
+        Raises: 
+            ValueError: If the provided 'path_expression' is not valid.
+        """
+        try:
+            if not path_expression.endswith(".md"):
+                path_expression += '.md'
+            if recursive and not path_expression.startswith("**/"):
+                path_expression = "**/" + path_expression
+
+            files = glob(path_expression, root_dir=self.root_dir,
+                         recursive=recursive)
+            return [self.open_note(file, deep_search=False) for file in files]
+
+        except Exception as exc:
+            raise ValueError(
+                f"Paremeter {path_expression} is nor valid.") from exc
+
+    def save_note(self, note: "Note"):
+        """Persist a note to the vault.  
+
+        Stores the note content to a file named after the note's filename attribute.
+        If the filename does not end in .md, .md is appended. 
+
+        Args:
+            note (Note): The note to be stored.
+
+        Raises:
+            ValueError: If the note could not be saved.
+        """
+        try:
+            filename = note.filename
+            if not filename.endswith(".md"):
+                filename += '.md'
+            filename = self.root_dir / filename
+
+            with open(filename, mode="w", encoding="utf-8") as f:
+                f.write(str(note))
+        except Exception as exc:
+            raise ValueError(
                 f"Note save failed.") from exc
```

### Comparing `smart_notes_vault-0.1.1/snv/io.py` & `smart_notes_vault-1.1.3/snv/io.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from os import getcwd
-from pathlib import Path
-
-from snv.classes import Vault
-
-
-def open_vault(dir: str = getcwd()) -> Vault:
-    """Opens a Vault (collection of notes) from the given directory.
-
-    >>> open_vault('./vault_dir')
-    <Vault: './vault_dir'>
-
-    Args:
-        dir (str, optional): The path to the directory containing the Vault. 
-            Defaults to the current working directory.
-
-    Returns:
-        Vault: An object representing the opened Vault.
-
-    Raises:
-        ValueError: If the Vault could not be opened from the given path.
-    """
-    try:
-        path = Path(dir)
-        return Vault(path)
-    except Exception as exc:
-        raise ValueError(f"Can not open vault from path: {path}") from exc
-
-if __name__ == '__main__':
-    import doctest
+from os import getcwd
+from pathlib import Path
+
+from snv.classes import Vault
+
+
+def open_vault(dir: str = getcwd()) -> Vault:
+    """Opens a Vault (collection of notes) from the given directory.
+
+    >>> open_vault('./vault_dir')
+    <Vault: './vault_dir'>
+
+    Args:
+        dir (str, optional): The path to the directory containing the Vault. 
+            Defaults to the current working directory.
+
+    Returns:
+        Vault: An object representing the opened Vault.
+
+    Raises:
+        ValueError: If the Vault could not be opened from the given path.
+    """
+    try:
+        path = Path(dir)
+        return Vault(path)
+    except Exception as exc:
+        raise ValueError(f"Can not open vault from path: {path}") from exc
+
+if __name__ == '__main__':
+    import doctest
     doctest.testmod()
```

### Comparing `smart_notes_vault-0.1.1/snv/md.py` & `smart_notes_vault-1.1.3/snv/md.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-def extract_header(note: str, *, header_separator='---\n') -> None | str :
-    """Retrieve metadata from a note string.
-
-    The metadata, containing specific information about the note, is enclosed by a designated string,
-    which is set as '---\n' by default. If the metadata is not found, the function returns None.
-
-    Args:
-        note (str): The string content of the note.
-        header_separator (str, optional): The string used to mark the metadata section.
-            Defaults to '---\n'.
-
-    Returns:
-        str or None: The extracted metadata string or None if metadata is not found.
-
-    Raises:
-        ValueError: If the note string cannot be processed.
-    """
-    try:
-        if not note.startswith(header_separator):
-            return None
-        lhs = len(header_separator)
-        header_end = note.index(header_separator, lhs)
-        if not header_end:
-            return  None
-        header = note[:header_end + lhs]
-        return header
-    except ValueError:
-        if __debug__: print(f"Note start with header symbol, but do not finish it, {note}.")
-        return None
-    except Exception as exc:
-        raise ValueError(f"Note is not procesible.") from exc
-    
-def extract_markdown(note: str, *, header_separator='---\n') -> str:
-    """Get the markdown part of note as a string.
-
-    Removes the metadata header and header separator from the note string and returns the remaining 
-    Markdown content.
-
-    Args:
-        note (str): The string content of the note.
-        header_separator (str, optional): The string used to mark the metadata section. 
-            Defaults to '---\n'.
-
-    Returns:
-        str: The Markdown content of the note.
-
-    Raises:
-        ValueError: If the note string cannot be processed.
-    """
-    try:
-        if note.count(header_separator) >= 2:
-            lhs = len(header_separator)
-            content_start = note.index(header_separator, lhs)
-            return note[content_start+lhs:]
-        return note
-    except Exception as exc:
+def extract_header(note: str, *, header_separator='---\n') -> None | str :
+    """Retrieve metadata from a note string.
+
+    The metadata, containing specific information about the note, is enclosed by a designated string,
+    which is set as '---\n' by default. If the metadata is not found, the function returns None.
+
+    Args:
+        note (str): The string content of the note.
+        header_separator (str, optional): The string used to mark the metadata section.
+            Defaults to '---\n'.
+
+    Returns:
+        str or None: The extracted metadata string or None if metadata is not found.
+
+    Raises:
+        ValueError: If the note string cannot be processed.
+    """
+    try:
+        if not note.startswith(header_separator):
+            return None
+        lhs = len(header_separator)
+        header_end = note.index(header_separator, lhs)
+        if not header_end:
+            return  None
+        header = note[:header_end + lhs]
+        return header
+    except ValueError:
+        if __debug__: print(f"Note start with header symbol, but do not finish it, {note}.")
+        return None
+    except Exception as exc:
+        raise ValueError(f"Note is not procesible.") from exc
+    
+def extract_markdown(note: str, *, header_separator='---\n') -> str:
+    """Get the markdown part of note as a string.
+
+    Removes the metadata header and header separator from the note string and returns the remaining 
+    Markdown content.
+
+    Args:
+        note (str): The string content of the note.
+        header_separator (str, optional): The string used to mark the metadata section. 
+            Defaults to '---\n'.
+
+    Returns:
+        str: The Markdown content of the note.
+
+    Raises:
+        ValueError: If the note string cannot be processed.
+    """
+    try:
+        if note.count(header_separator) >= 2:
+            lhs = len(header_separator)
+            content_start = note.index(header_separator, lhs)
+            return note[content_start+lhs:]
+        return note
+    except Exception as exc:
         raise ValueError(f"Note is not procesible.") from exc
```

### Comparing `smart_notes_vault-0.1.1/tests/conf_vault.py` & `smart_notes_vault-1.1.3/tests/conf_vault.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import pytest
-import textwrap
-import snv
-
-from pathlib import Path
-
-
-@pytest.fixture(scope="session")
-def simple_note():
-    return {
-        "filename": "simple.md",
-        "content": textwrap.dedent("""
-            # Simple note
-
-            Contains only text, not other features like:
-                - links
-                - tags
-                - footers
-            """).strip()
-    }
-
-
-@pytest.fixture(scope="session")
-def simple_note_with_header(simple_note):
-    return {
-        "filename": "simple_with_header.md",
-        "content": textwrap.dedent("""
-            ---
-            #aliases: [3D tisk insert]
-            tags: [Honza]
-            created: 2022-07-12
-            ---
-            # simple_with_header
-
-            """).strip() + simple_note["content"]
-    }
-
-@pytest.fixture(scope="session")
-def simple_note_in_folder(simple_note):
-    return {
-        "filename": "topic/simple_with_header.md",
-        "content": textwrap.dedent("""
-            ---
-            #aliases: [3D tisk insert]
-            tags: [Honza]
-            created: 2022-07-12
-            ---
-            # topic/simple_with_header
-           
-            """).strip() + simple_note["content"]
-    }
-
-@pytest.fixture(scope="session")
-def all_notes(
-    simple_note,
-    simple_note_with_header,
-    simple_note_in_folder,
-):
-    return [
-        simple_note,
-        simple_note_with_header,
-        simple_note_in_folder,
-    ]
-
-
-@pytest.fixture(scope="session")
-def vault_dir(tmp_path_factory: pytest.TempPathFactory,
-              all_notes):
-    root_dir = tmp_path_factory.mktemp("vault")
-
-    for note_fixture in all_notes:
-        path = Path(root_dir / note_fixture["filename"])
-        if not path.parent.exists():
-            path.parent.mkdir(parents=True, exist_ok=True)
-
-        with open(path, mode="w", encoding="utf-8") as file:
-            file.write(note_fixture["content"])
-
-    return root_dir
-
-
-@pytest.fixture(scope="session")
-def vault(vault_dir):
-    return snv.open_vault(vault_dir)
+import pytest
+import textwrap
+import snv
+
+from pathlib import Path
+
+
+@pytest.fixture(scope="session")
+def simple_note():
+    return {
+        "filename": "simple.md",
+        "content": textwrap.dedent("""
+            # Simple note
+
+            Contains only text, not other features like:
+                - links
+                - tags
+                - footers
+            """).strip()
+    }
+
+
+@pytest.fixture(scope="session")
+def simple_note_with_header(simple_note):
+    return {
+        "filename": "simple_with_header.md",
+        "content": textwrap.dedent("""
+            ---
+            #aliases: [3D tisk insert]
+            tags: [Honza]
+            created: 2022-07-12
+            ---
+            # simple_with_header
+
+            """).strip() + simple_note["content"]
+    }
+
+@pytest.fixture(scope="session")
+def simple_note_in_folder(simple_note):
+    return {
+        "filename": "topic/simple_with_header.md",
+        "content": textwrap.dedent("""
+            ---
+            #aliases: [3D tisk insert]
+            tags: [Honza]
+            created: 2022-07-12
+            ---
+            # topic/simple_with_header
+           
+            """).strip() + simple_note["content"]
+    }
+
+@pytest.fixture(scope="session")
+def all_notes(
+    simple_note,
+    simple_note_with_header,
+    simple_note_in_folder,
+):
+    return [
+        simple_note,
+        simple_note_with_header,
+        simple_note_in_folder,
+    ]
+
+
+@pytest.fixture(scope="session")
+def vault_dir(tmp_path_factory: pytest.TempPathFactory,
+              all_notes):
+    root_dir = tmp_path_factory.mktemp("vault")
+
+    for note_fixture in all_notes:
+        path = Path(root_dir / note_fixture["filename"])
+        if not path.parent.exists():
+            path.parent.mkdir(parents=True, exist_ok=True)
+
+        with open(path, mode="w", encoding="utf-8") as file:
+            file.write(note_fixture["content"])
+
+    return root_dir
+
+
+@pytest.fixture(scope="session")
+def vault(vault_dir):
+    return snv.open_vault(vault_dir)
```

### Comparing `smart_notes_vault-0.1.1/tests/test_class_note.py` & `smart_notes_vault-1.1.3/tests/test_class_note.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import pytest
-import snv
-
-
-def test__init__(simple_note_with_header):
-    # Act
-    note = snv.Note(**simple_note_with_header)
-    # Assert
-    assert type(note) is snv.Note
-    assert note.filename == simple_note_with_header["filename"]
-    assert note.content == simple_note_with_header["content"]
-
-def test__init__file_not_exists():
-    # Arrange
-    filename = 'file_not_exists.md'
-    # Act
-    note = snv.Note(filename)
-    # Assert
-    assert type(note) is snv.Note
-    assert note.filename == filename
-    assert note.content is None
-
-def test__repr__(simple_note_with_header):
-    # Arrange
-    note = snv.Note(**simple_note_with_header)
-    # Act
-    result = repr(note)
-    # Assert
-    assert "Note" in result
-    assert f"filename='{note.filename}'" in result
-    assert f"content=" in result
-
-def test__str__(simple_note_with_header):
-    # Arrange
-    note = snv.Note(**simple_note_with_header)
-    # Act
-    content = str(note)
-    # Assert
-    assert content == simple_note_with_header["content"]
-
-def test_property_header_None(simple_note):
-    # Arrange
-    note = snv.Note(**simple_note)
-    # Act
-    header = note.header
-    # Assert
-    assert header is not None
-    assert isinstance(header, snv.Note.Header)
-    assert str(header) == ""
-
-def test_property_header_exists(simple_note_with_header):
-    # Arrange
-    note = snv.Note(**simple_note_with_header)
-    # Act
-    header = note.header
-    # Assert
-    assert header is not None
-    assert isinstance(header,snv.Note.Header)
-    assert str(header) == simple_note_with_header['content'][:69]
-
-class TestHeader:
-
-    def test_getting_tags_from_header(self, simple_note_with_header):
-        # Arrange
-        note = snv.Note(**simple_note_with_header)
-        header = note.header
-        # Act
-        tags = header.tags()
-        # Assert
-        assert tags == ("Honza",)
-
-    def test_removing_tag_from_header(self, simple_note_with_header):
-            # Arrange
-            note = snv.Note(**simple_note_with_header)
-            header = note.header
-            # Act
-            result = header.remove_tag("Honza")
-            # Assert
-            assert isinstance(result, snv.Note)
-            assert "Honza" not in result.header.tags()
-
-    def test_removing_not_contains_tag_from_header(self, simple_note_with_header):
-        # Arrange
-        note = snv.Note(**simple_note_with_header)
-        header = note.header
-        # Act
-        result = header.remove_tag("Not_contains")
-        # Assert
-        assert isinstance(result, snv.Note)
-        assert "Not_contains" not in result.header.tags()
+import pytest
+import snv
+
+
+def test__init__(simple_note_with_header):
+    # Act
+    note = snv.Note(**simple_note_with_header)
+    # Assert
+    assert type(note) is snv.Note
+    assert note.filename == simple_note_with_header["filename"]
+    assert note.content == simple_note_with_header["content"]
+
+def test__init__file_not_exists():
+    # Arrange
+    filename = 'file_not_exists.md'
+    # Act
+    note = snv.Note(filename)
+    # Assert
+    assert type(note) is snv.Note
+    assert note.filename == filename
+    assert note.content is None
+
+def test__repr__(simple_note_with_header):
+    # Arrange
+    note = snv.Note(**simple_note_with_header)
+    # Act
+    result = repr(note)
+    # Assert
+    assert "Note" in result
+    assert f"filename='{note.filename}'" in result
+    assert f"content=" in result
+
+def test__str__(simple_note_with_header):
+    # Arrange
+    note = snv.Note(**simple_note_with_header)
+    # Act
+    content = str(note)
+    # Assert
+    assert content == simple_note_with_header["content"]
+
+def test_property_header_None(simple_note):
+    # Arrange
+    note = snv.Note(**simple_note)
+    # Act
+    header = note.header
+    # Assert
+    assert header is not None
+    assert isinstance(header, snv.Note.Header)
+    assert str(header) == ""
+
+def test_property_header_exists(simple_note_with_header):
+    # Arrange
+    note = snv.Note(**simple_note_with_header)
+    # Act
+    header = note.header
+    # Assert
+    assert header is not None
+    assert isinstance(header,snv.Note.Header)
+    assert str(header) == simple_note_with_header['content'][:69]
+
+class TestHeader:
+
+    def test_getting_tags_from_header(self, simple_note_with_header):
+        # Arrange
+        note = snv.Note(**simple_note_with_header)
+        header = note.header
+        # Act
+        tags = header.tags()
+        # Assert
+        assert tags == ("Honza",)
+
+    def test_removing_tag_from_header(self, simple_note_with_header):
+            # Arrange
+            note = snv.Note(**simple_note_with_header)
+            header = note.header
+            # Act
+            result = header.remove_tag("Honza")
+            # Assert
+            assert isinstance(result, snv.Note)
+            assert "Honza" not in result.header.tags()
+
+    def test_removing_not_contains_tag_from_header(self, simple_note_with_header):
+        # Arrange
+        note = snv.Note(**simple_note_with_header)
+        header = note.header
+        # Act
+        result = header.remove_tag("Not_contains")
+        # Assert
+        assert isinstance(result, snv.Note)
+        assert "Not_contains" not in result.header.tags()
```

### Comparing `smart_notes_vault-0.1.1/tests/test_class_vault.py` & `smart_notes_vault-1.1.3/tests/test_class_vault.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import pytest
-import snv
-import textwrap
-
-from pathlib import Path
-from os import getcwd
-
-
-
-def test__init__(vault_dir):
-    # Act
-    vault = snv.Vault(root_dir=vault_dir)
-    # Assert
-    assert vault.root_dir == vault_dir
-
-def test__init__create_not_exists_dir(tmp_path):
-    # Arrange
-    root_dir = tmp_path / "vault"
-    # Act
-    vault = snv.Vault(root_dir, create_root_dir=True)
-    # Assert
-    assert vault.root_dir == root_dir
-    assert root_dir.exists()
-
-@pytest.mark.parametrize("root_dir, error", [
-    (None, ValueError),
-    ("dir_is_not_path", TypeError),
-    (Path("dir_does_not_exist"), FileNotFoundError),
-    (Path("./readme.md"), NotADirectoryError),
-])
-def test__init__raise_error(root_dir, error):
-    # Act & Assert
-    with pytest.raises(error):
-        snv.Vault(root_dir)
-
-def test_open_note(vault, simple_note):
-    # Arrange
-    filename = simple_note["filename"]
-    # Act
-    result = vault.open_note(filename)
-    # Assert
-    assert result is not None
-    assert type(result) == snv.Note
-    assert result.filename == filename
-    assert result.content == simple_note['content']
-
-def test_open_note_not_existing(vault):
-    # Arrange
-    filename = "not_exists.md"
-    # Act
-    result = vault.open_note(filename)
-    # Assert
-    assert result is not None
-    assert type(result) == snv.Note
-    assert result.filename == filename
-    assert result.content is None
-
-def test_open_note_with_duplicite_name(vault):
-    # Arrange
-    filename = "simple_with_header"
-    # Act
-    result = vault.open_note(filename)
-    # Assert
-    assert result is not None
-    assert type(result) == list
-    assert len(result) == 2
-    assert type(result[0]) == snv.Note 
-    assert type(result[1]) == snv.Note 
-
-def test_find_by_path(vault_dir, all_notes):
-    # Arrange
-    vault = snv.Vault(vault_dir)
-    # Act
-    notes = vault.find_note_by_path("*")
-    # Assert
-    assert len(notes) == len(all_notes)
-    assert all(map(lambda n: isinstance(n, snv.Note), notes))
-    assert notes[0].content is not None
-
-def test_find_by_path_not_recursive(vault_dir, all_notes):
-    # Arrange
-    vault = snv.Vault(vault_dir)
-    # Act
-    notes = vault.find_note_by_path("*", recursive=False)
-    # Assert
-    assert len(notes) == len([n for n in all_notes if "/" not in n['filename']]) 
-
-def test_save_note(vault: snv.Vault):
-    # Arrange
-    note = snv.Note("test", textwrap.dedent("""
-            ---
-            title: Note title 
-            tags: [tag1, tag2]
-            ---
-            # Title 
-
-            Some content
-            ---
-            """).strip())
-    # Act
-    vault.save_note(note)
-    # Assert
-    stored_note = vault.open_note("test", deep_search=False)
-    
-    assert stored_note.content == note.content
+import pytest
+import snv
+import textwrap
+
+from pathlib import Path
+from os import getcwd
+
+
+
+def test__init__(vault_dir):
+    # Act
+    vault = snv.Vault(root_dir=vault_dir)
+    # Assert
+    assert vault.root_dir == vault_dir
+
+def test__init__create_not_exists_dir(tmp_path):
+    # Arrange
+    root_dir = tmp_path / "vault"
+    # Act
+    vault = snv.Vault(root_dir, create_root_dir=True)
+    # Assert
+    assert vault.root_dir == root_dir
+    assert root_dir.exists()
+
+@pytest.mark.parametrize("root_dir, error", [
+    (None, ValueError),
+    ("dir_is_not_path", TypeError),
+    (Path("dir_does_not_exist"), FileNotFoundError),
+    (Path("./readme.md"), NotADirectoryError),
+])
+def test__init__raise_error(root_dir, error):
+    # Act & Assert
+    with pytest.raises(error):
+        snv.Vault(root_dir)
+
+def test_open_note(vault, simple_note):
+    # Arrange
+    filename = simple_note["filename"]
+    # Act
+    result = vault.open_note(filename)
+    # Assert
+    assert result is not None
+    assert type(result) == snv.Note
+    assert result.filename == filename
+    assert result.content == simple_note['content']
+
+def test_open_note_not_existing(vault):
+    # Arrange
+    filename = "not_exists.md"
+    # Act
+    result = vault.open_note(filename)
+    # Assert
+    assert result is not None
+    assert type(result) == snv.Note
+    assert result.filename == filename
+    assert result.content is None
+
+def test_open_note_with_duplicite_name(vault):
+    # Arrange
+    filename = "simple_with_header"
+    # Act
+    result = vault.open_note(filename)
+    # Assert
+    assert result is not None
+    assert type(result) == list
+    assert len(result) == 2
+    assert type(result[0]) == snv.Note 
+    assert type(result[1]) == snv.Note 
+
+def test_find_by_path(vault_dir, all_notes):
+    # Arrange
+    vault = snv.Vault(vault_dir)
+    # Act
+    notes = vault.find_note_by_path("*")
+    # Assert
+    assert len(notes) == len(all_notes)
+    assert all(map(lambda n: isinstance(n, snv.Note), notes))
+    assert notes[0].content is not None
+
+def test_find_by_path_not_recursive(vault_dir, all_notes):
+    # Arrange
+    vault = snv.Vault(vault_dir)
+    # Act
+    notes = vault.find_note_by_path("*", recursive=False)
+    # Assert
+    assert len(notes) == len([n for n in all_notes if "/" not in n['filename']]) 
+
+def test_save_note(vault: snv.Vault):
+    # Arrange
+    note = snv.Note("test", textwrap.dedent("""
+            ---
+            title: Note title 
+            tags: [tag1, tag2]
+            ---
+            # Title 
+
+            Some content
+            ---
+            """).strip())
+    # Act
+    vault.save_note(note)
+    # Assert
+    stored_note = vault.open_note("test", deep_search=False)
+    
+    assert stored_note.content == note.content
```

