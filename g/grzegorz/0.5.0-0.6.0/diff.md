# Comparing `tmp/grzegorz-0.5.0.tar.gz` & `tmp/grzegorz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grzegorz-0.5.0.tar", last modified: Thu Jun 29 21:04:54 2023, max compression
+gzip compressed data, was "grzegorz-0.6.0.tar", last modified: Thu Aug  3 21:30:25 2023, max compression
```

## Comparing `grzegorz-0.5.0.tar` & `grzegorz-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/
--rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.5.0/LICENSE
--rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-06-29 21:04:54.954460 grzegorz-0.5.0/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)     3177 2023-06-29 21:00:50.000000 grzegorz-0.5.0/README.md
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/grzegorz/
--rw-------   0 xylous    (1000) xylous    (1001)        0 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/__init__.py
--rw-------   0 xylous    (1000) xylous    (1001)     8531 2023-06-29 18:45:47.000000 grzegorz-0.5.0/grzegorz/__main__.py
--rw-------   0 xylous    (1000) xylous    (1001)     4156 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/anki_integration.py
--rw-------   0 xylous    (1000) xylous    (1001)     2823 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/fetcher.py
--rw-------   0 xylous    (1000) xylous    (1001)     9808 2023-06-29 18:44:05.000000 grzegorz-0.5.0/grzegorz/generator.py
--rw-------   0 xylous    (1000) xylous    (1001)     3950 2023-06-26 10:32:45.000000 grzegorz-0.5.0/grzegorz/test.py
--rw-------   0 xylous    (1000) xylous    (1001)     9448 2023-06-26 10:06:56.000000 grzegorz-0.5.0/grzegorz/word.py
--rw-------   0 xylous    (1000) xylous    (1001)     4024 2023-06-26 09:43:37.000000 grzegorz-0.5.0/grzegorz/wordlist.py
-drwx------   0 xylous    (1000) xylous    (1001)        0 2023-06-29 21:04:54.954460 grzegorz-0.5.0/grzegorz.egg-info/
--rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/PKG-INFO
--rw-------   0 xylous    (1000) xylous    (1001)      404 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/SOURCES.txt
--rw-------   0 xylous    (1000) xylous    (1001)        1 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/dependency_links.txt
--rw-------   0 xylous    (1000) xylous    (1001)       52 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/entry_points.txt
--rw-------   0 xylous    (1000) xylous    (1001)       39 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/requires.txt
--rw-------   0 xylous    (1000) xylous    (1001)        9 2023-06-29 21:04:54.000000 grzegorz-0.5.0/grzegorz.egg-info/top_level.txt
--rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.5.0/pyproject.toml
--rw-------   0 xylous    (1000) xylous    (1001)      852 2023-06-29 21:04:54.954460 grzegorz-0.5.0/setup.cfg
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-08-03 21:30:25.192701 grzegorz-0.6.0/
+-rw-------   0 xylous    (1000) xylous    (1001)    35148 2022-06-15 13:54:28.000000 grzegorz-0.6.0/LICENSE
+-rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-08-03 21:30:25.192701 grzegorz-0.6.0/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)     3177 2023-06-29 21:00:50.000000 grzegorz-0.6.0/README.md
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-08-03 21:30:25.189368 grzegorz-0.6.0/grzegorz/
+-rw-------   0 xylous    (1000) xylous    (1001)        0 2023-08-01 16:19:05.000000 grzegorz-0.6.0/grzegorz/__init__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     7133 2023-08-02 19:06:43.000000 grzegorz-0.6.0/grzegorz/__main__.py
+-rw-------   0 xylous    (1000) xylous    (1001)     3933 2023-08-03 21:13:49.000000 grzegorz-0.6.0/grzegorz/anki_integration.py
+-rw-------   0 xylous    (1000) xylous    (1001)     1929 2023-08-03 20:52:53.000000 grzegorz-0.6.0/grzegorz/fetcher.py
+-rw-------   0 xylous    (1000) xylous    (1001)     9096 2023-08-03 21:13:35.000000 grzegorz-0.6.0/grzegorz/generator.py
+-rw-------   0 xylous    (1000) xylous    (1001)     2221 2023-08-03 21:14:30.000000 grzegorz-0.6.0/grzegorz/io.py
+-rw-------   0 xylous    (1000) xylous    (1001)     6029 2023-08-03 21:08:45.000000 grzegorz-0.6.0/grzegorz/subcommands.py
+-rw-------   0 xylous    (1000) xylous    (1001)     3866 2023-08-03 20:30:38.000000 grzegorz-0.6.0/grzegorz/test.py
+-rw-------   0 xylous    (1000) xylous    (1001)     7899 2023-08-03 21:13:05.000000 grzegorz-0.6.0/grzegorz/word.py
+-rw-------   0 xylous    (1000) xylous    (1001)     4058 2023-08-03 21:01:40.000000 grzegorz-0.6.0/grzegorz/wordlist.py
+drwx------   0 xylous    (1000) xylous    (1001)        0 2023-08-03 21:30:25.192701 grzegorz-0.6.0/grzegorz.egg-info/
+-rw-------   0 xylous    (1000) xylous    (1001)     3861 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/PKG-INFO
+-rw-------   0 xylous    (1000) xylous    (1001)      443 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/SOURCES.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        1 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/dependency_links.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       52 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/entry_points.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       39 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/requires.txt
+-rw-------   0 xylous    (1000) xylous    (1001)        9 2023-08-03 21:30:25.000000 grzegorz-0.6.0/grzegorz.egg-info/top_level.txt
+-rw-------   0 xylous    (1000) xylous    (1001)       85 2022-06-18 14:25:50.000000 grzegorz-0.6.0/pyproject.toml
+-rw-------   0 xylous    (1000) xylous    (1001)      852 2023-08-03 21:30:25.192701 grzegorz-0.6.0/setup.cfg
```

### Comparing `grzegorz-0.5.0/LICENSE` & `grzegorz-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grzegorz-0.5.0/PKG-INFO` & `grzegorz-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grzegorz
-Version: 0.5.0
+Version: 0.6.0
 Summary: Minimal pair generator and phonetics tool
 Home-page: https://github.com/xylous/grzegorz
 Author: xylous
 Author-email: xylous.e@gmail.com
 Project-URL: Bug Tracker, https://github.com/xylous/grzegorz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grzegorz-0.5.0/README.md` & `grzegorz-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `grzegorz-0.5.0/grzegorz/__main__.py` & `grzegorz-0.6.0/grzegorz/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,16 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from grzegorz.fetcher import fetchipa
-from grzegorz.generator import (MinPairGenerator)
-from grzegorz.word import (Word)
-from grzegorz.anki_integration import makedeck
-from grzegorz.wordlist import (wordlist, print_languages_list)
+from grzegorz.subcommands import *
 
-from os import remove
 import argparse
 
 # Why does it have to be this complicated?
 def create_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
             prog='grzegorz',
             description='Generate minimal pairs from a list of words')
@@ -51,32 +46,32 @@
             help='List all languages for which you can fetch a wordlist')
 
     # 'fullmake' command
     parser_fullmake = subparsers.add_parser('fullmake',
             help='Build an Anki deck for a language automatically')
     parser_fullmake.add_argument('language',
             type=str)
-    parser_fullmake.add_argument('numwords',
-            type=int,
-            help='number of words to sample')
+    parser_fullmake.add_argument('bounds',
+            type=str,
+            help='number of words to keep; alternatively, the range of words to keep, e.g. "1500:3000"')
     parser_fullmake.add_argument('--clean',
             dest='clean',
             action='store_true',
             default=False,
             help='remove temporary files after building the deck')
 
     # 'wordlist' command
     parser_wordlist = subparsers.add_parser('wordlist',
             help='Fetch the word list for a given language, containing a certain number of words')
     parser_wordlist.add_argument('language',
             type=str,
             help='language of the wordlist')
-    parser_wordlist.add_argument('numwords',
-            type=int,
-            help='number of words to keep')
+    parser_wordlist.add_argument('bounds',
+            type=str,
+            help='number of words to keep; alternatively, the range of words to keep, e.g. "1500:3000"')
     parser_wordlist.add_argument('outfile',
             type=str,
             help='path where the wordlist should be stored')
 
     # 'fetchipa' subcommand
     parser_fetchipa = subparsers.add_parser('fetchipa',
             help='Fetch all IPA pronunciations for the words into a JSON file')
@@ -87,14 +82,19 @@
             type=str,
             help='output file (JSON)')
     parser_fetchipa.add_argument('--keep-failed',
             dest='keep_failed',
             action='store_true',
             default=False,
             help='Save the words for which no IPA was found in the output file (default: don\'t)')
+    parser_fetchipa.add_argument('--numproc',
+            type=int,
+            dest='numproc',
+            default=20,
+            help='Number of concurrent processes to handle the wordlist; default: 20')
 
     # 'generate' subcommand
     parser_generate = subparsers.add_parser('generate',
             help='Create minimal pairs, given a JSON input file')
     parser_generate.add_argument('infile',
             type=str,
             help='JSON file created by fetchipa')
@@ -134,96 +134,47 @@
             help="Output file of 'generate'")
     parser_makedeck.add_argument('outfile',
             type=str,
             help="Output file; note that it should ideally have the .apkg extension")
 
     return parser
 
-def fullmake(language: str, numwords: int, clean: bool) -> None:
-    """
-    Practically: wrap all commands into one. If `clean` is True, then
-    temporary files created by this function are removed.
-    """
-    optimise = True
-    keep_phonemes = True
-    keep_chronemes = True
-    keep_stress = True
-
-    wordlist_file = language + "-wordlist.txt"
-    ipa_json = language + "-ipa.json"
-    minpairs_file = language + "-minpairs.json"
-    makedeck_file = "grzegorz-" + language + "-minpairs.apkg"
-
-    if wordlist(language, numwords, wordlist_file) == 1:
-        exit(1)
-    fetchipa(wordlist_file, ipa_json, False)
-    g = MinPairGenerator(
-        optimise,
-        keep_phonemes,
-        keep_chronemes,
-        keep_stress,
-    )
-    g.generate(ipa_json, minpairs_file)
-    makedeck(minpairs_file, makedeck_file)
-
-    if clean:
-        print("Removing temporary files...")
-        remove(wordlist_file)
-        remove(ipa_json)
-        remove(minpairs_file)
-
 def main() -> None:
     parser = create_argparser()
     args = parser.parse_args()
 
     cmd = args.subparser_name
 
     match cmd:
         case 'fullmake':
             clean = args.clean
-            numwords = args.numwords
+            bounds = args.bounds
             language = args.language.lower()
-            fullmake(language, numwords, clean)
+            fullmake(language, bounds, clean)
         case 'wordlist':
-            outfile = args.outfile
-            numwords = args.numwords
-            language = args.language.lower()
-            status = wordlist(language, numwords, outfile)
+            status = wordlist_command(args.language.lower(), args.bounds, args.outfile)
             exit(status)
         case 'fetchipa':
-            fetchipa(args.infile, args.outfile, args.keep_failed)
+            fetchipa(args.infile, args.outfile, args.keep_failed, args.numproc)
         case 'generate':
             infile = args.infile
             outfile = args.outfile
             nooptimise = args.nooptimise;
             no_phonemes = args.no_phonemes;
             no_chronemes = args.no_chronemes;
             no_stress = args.no_stress;
             filter_file_path = args.path
-            g = MinPairGenerator(
-                not nooptimise,
-                not no_phonemes,
-                not no_chronemes,
-                not no_stress
-            )
-            if filter_file_path is not None:
-                g.set_filter_pairs_from_file(filter_file_path)
-            g.generate(infile, outfile)
+            generate_command(infile, outfile, nooptimise, no_phonemes, no_chronemes,
+                     no_stress, filter_file_path)
         case 'makedeck':
-            infile = args.infile
-            outfile = args.outfile
-            makedeck(infile, outfile)
+            makedeck(args.infile, args.outfile)
         case 'analyse':
-            Word("", args.ipa).print_human_readable()
+            print_analysis(args.ipa)
         case 'check':
-            word1 = Word("", args.ipa_first)
-            word2 = Word("", args.ipa_second)
-            generator = MinPairGenerator(False, True, True, True)
-            if not generator.print_human_readable_check(word1, word2):
-                exit(1)
+            print_minpair_check(args.ipa_first, args.ipa_second)
         case 'list-languages':
-            print_languages_list()
+            list_languages()
         case _:
             parser.print_help()
 
 if __name__ == "__main__":
     main()
```

### Comparing `grzegorz-0.5.0/grzegorz/anki_integration.py` & `grzegorz-0.6.0/grzegorz/anki_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from grzegorz.word import MinPair, readfile
+from grzegorz.word import WordPair
 
 import genanki
 from genanki import Note, Deck
-import json
 
 """The model used for the flashcards is rather simple"""
 grzegorz_minpair_model = genanki.Model(
     1958583115, # Randomly generated Model ID. Needs to be hardcoded!
     'Grzegorz Minimal Pairs',
     fields=[
         {'name': 'Word 1 text'},
@@ -40,15 +39,15 @@
 <br>
 
 {{Word 1 audio}}
 
 <br>
 
 <div class="minpair">
-<div id="corret-word" class="word">{{Word 1 text}}<br>{{Word 1 IPA}}</div>
+<div id="correct-word" class="word">{{Word 1 text}}<br>{{Word 1 IPA}}</div>
 <div class="center"><i>or</i></div>
 <div class="word">{{Word 2 text}}<br>{{Word 2 IPA}}</div>
 </div>""",
             'afmt':
 """{{FrontSide}}
 
 <hr id=answer>
@@ -117,54 +116,45 @@
 
 .center {
     display: inline;
     padding: 10px;
 }""",
 )
 
-def makedeck(infile: str, outfile: str) -> None:
-    """Create an Anki deck given a file full of minimal pairs"""
-    json_str = readfile(infile)
-    dict = json.loads(json_str)
-    minpairs = list(map(MinPair.from_dict, dict))
-    notes = list(map(minpair_to_anki_note, minpairs))
-    deck = notes_to_deck(notes)
-    export_deck(deck, outfile)
+def minpairs_to_deck(minpairs: list[WordPair]) -> Deck:
+    """Turn a list of minimal pairs into an Anki deck"""
+    notes = [minpair_to_anki_note(mp) for mp in minpairs]
+    return notes_to_deck(notes)
 
-### HELPER FUNCTIONS ###
+def export_deck(deck: Deck, outfile: str) -> None:
+    """Package the given deck and write it to a file"""
+    genanki.Package(deck).write_to_file(outfile)
 
-def minpair_to_anki_note(minpair: MinPair) -> Note:
+def minpair_to_anki_note(minpair: WordPair) -> Note:
     """
-    Given a minimal pair, create an Anki note from it, with grzegorz_minpair_model
-    as its model.
+    Given a minimal pair, create an Anki note from it, with `grzegorz_minpair_model`
+    as its template.
     """
-    first = minpair.first
-    last = minpair.last
     note = genanki.Note(
         model=grzegorz_minpair_model,
         fields=[
-            first.text,
+            minpair[0].text,
             '',
-            first.ipa,
-            last.text,
+            minpair[0].ipa,
+            minpair[1].text,
             '',
-            last.ipa,
+            minpair[1].ipa,
         ]
     )
     return note
 
 def notes_to_deck(notes: list[Note]) -> Deck:
     """
-    Add a list of notes into a deck called "grzegorz's minimal pairs"
+    Put the `Note`s into a `Deck` called "grzegorz's minimal pairs"
     """
     deck = genanki.Deck(
-        1597757363,
+        1597757363, # deck ID, randomly generated but hardcoded
         "grzegorz's minimal pairs",
     )
     for note in notes:
         deck.add_note(note)
     return deck
-
-def export_deck(deck: Deck, outfile: str) -> None:
-    """Package the given deck and write it to a file"""
-    genanki.Package(deck).write_to_file(outfile)
-    print('Done! Now import', outfile, 'in your Anki')
```

#### html2text {}

```diff
@@ -4,22 +4,21 @@
 Public License as published by the Free Software # Foundation, either version 3
 of the License, or (at your option) any later # version. # # grzegorz is
 distributed in the hope that it will be useful, but WITHOUT ANY # WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR # A
 PARTICULAR PURPOSE. See the GNU General Public License for more details. # #
 You should have received a copy of the GNU General Public License along with #
 grzegorz. If not, see
-www.gnu.org/licenses/>. from grzegorz.word import MinPair, readfile import
-genanki from genanki import Note, Deck import json """The model used for the
-flashcards is rather simple""" grzegorz_minpair_model = genanki.Model
-( 1958583115, # Randomly generated Model ID. Needs to be hardcoded! 'Grzegorz
-Minimal Pairs', fields=[ {'name': 'Word 1 text'}, {'name': 'Word 1 audio'},
-{'name': 'Word 1 IPA'}, {'name': 'Word 2 text'}, {'name': 'Word 2 audio'},
-{'name': 'Word 2 IPA'}, ], templates=[ { 'name': 'Card 1', 'qfmt': """What did
-you hear?
+www.gnu.org/licenses/>. from grzegorz.word import WordPair import genanki from
+genanki import Note, Deck """The model used for the flashcards is rather
+simple""" grzegorz_minpair_model = genanki.Model( 1958583115, # Randomly
+generated Model ID. Needs to be hardcoded! 'Grzegorz Minimal Pairs', fields=[
+{'name': 'Word 1 text'}, {'name': 'Word 1 audio'}, {'name': 'Word 1 IPA'},
+{'name': 'Word 2 text'}, {'name': 'Word 2 audio'}, {'name': 'Word 2 IPA'}, ],
+templates=[ { 'name': 'Card 1', 'qfmt': """What did you hear?
 {{Word 1 audio}}
 {{Word 1 text}}
 {{Word 1 IPA}}
 or
 {{Word 2 text}}
 {{Word 2 IPA}}
 """, 'afmt': """{{FrontSide}}
@@ -38,23 +37,20 @@
 You heard:
 {{Word 2 text}}
 """, }, ], css= """.card { font-family: arial; font-size: 20px; text-align:
 center; color: black; background-color: white; } .word { text-align: center;
 border: 3px outset black; display: inline-block; box-sizing: border-box; }
 .nightMode .word { border: 3px outset white; } .minpair { display: flex;
 justify-content: center; align-items: center; } .center { display: inline;
-padding: 10px; }""", ) def makedeck(infile: str, outfile: str) -> None:
-"""Create an Anki deck given a file full of minimal pairs""" json_str =
-readfile(infile) dict = json.loads(json_str) minpairs = list(map
-(MinPair.from_dict, dict)) notes = list(map(minpair_to_anki_note, minpairs))
-deck = notes_to_deck(notes) export_deck(deck, outfile) ### HELPER FUNCTIONS ###
-def minpair_to_anki_note(minpair: MinPair) -> Note: """ Given a minimal pair,
-create an Anki note from it, with grzegorz_minpair_model as its model. """
-first = minpair.first last = minpair.last note = genanki.Note
-( model=grzegorz_minpair_model, fields=[ first.text, '', first.ipa, last.text,
-'', last.ipa, ] ) return note def notes_to_deck(notes: list[Note]) -> Deck: """
-Add a list of notes into a deck called "grzegorz's minimal pairs" """ deck =
-genanki.Deck( 1597757363, "grzegorz's minimal pairs", ) for note in notes:
-deck.add_note(note) return deck def export_deck(deck: Deck, outfile: str) -
-> None: """Package the given deck and write it to a file""" genanki.Package
-(deck).write_to_file(outfile) print('Done! Now import', outfile, 'in your
-Anki')
+padding: 10px; }""", ) def minpairs_to_deck(minpairs: list[WordPair]) -> Deck:
+"""Turn a list of minimal pairs into an Anki deck""" notes =
+[minpair_to_anki_note(mp) for mp in minpairs] return notes_to_deck(notes) def
+export_deck(deck: Deck, outfile: str) -> None: """Package the given deck and
+write it to a file""" genanki.Package(deck).write_to_file(outfile) def
+minpair_to_anki_note(minpair: WordPair) -> Note: """ Given a minimal pair,
+create an Anki note from it, with `grzegorz_minpair_model` as its template. """
+note = genanki.Note( model=grzegorz_minpair_model, fields=[ minpair[0].text,
+'', minpair[0].ipa, minpair[1].text, '', minpair[1].ipa, ] ) return note def
+notes_to_deck(notes: list[Note]) -> Deck: """ Put the `Note`s into a `Deck`
+called "grzegorz's minimal pairs" """ deck = genanki.Deck( 1597757363, # deck
+ID, randomly generated but hardcoded "grzegorz's minimal pairs", ) for note in
+notes: deck.add_note(note) return deck
```

### Comparing `grzegorz-0.5.0/grzegorz/generator.py` & `grzegorz-0.6.0/grzegorz/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from grzegorz.word import (Word, MinPair, readfile, writefile,
+from grzegorz.word import (Word, WordPair,
                            PHONEME_MINPAIR, CHRONEME_MINPAIR, STRESS_MINPAIR,
                            NOT_MINPAIR)
+from grzegorz.io import readfile
 
-import json
 from tqdm import tqdm
 from itertools import chain, combinations
 
 class MinPairGenerator:
     def __init__(
         self,
         optimise: bool,
@@ -42,50 +42,35 @@
         contents = readfile(path).split("\n")
         lists_of_phonemes = []
         for line in contents:
             if line != "":
                 lists_of_phonemes.append(line.replace(" ", "").split(","))
         self.filter_pairs = phoneme_lists_to_phoneme_pairs(lists_of_phonemes)
 
-    def generate(self, infile: str, outfile: str) -> None:
+    def generate(self, words: list[Word]) -> list[WordPair]:
         """
-        Given the path to a file containing JSON data about serialised `Word`s, create
-        a file `outfile` with all the minimal pairs found, in JSON format
+        Generate minimal pairs from the given parameters
         """
-        jsonstr = readfile(infile)
-        words = json.loads(jsonstr, object_hook=Word.from_dict)
         minpairs = []
 
-        if not self.keep_phonemes and not self.keep_chronemes and not self.keep_stress:
-            print("Generator: skipping all contrasts means no minimal pairs will be generated; abort")
-            return
-        if not self.keep_phonemes:
-            print("Generator: phoneme contrasts will be ignored")
-        if not self.keep_chronemes:
-            print("Generator: chroneme contrasts will be ignored")
-        if not self.keep_stress:
-            print("Generator: syllable stress contrasts will be ignored")
-
         for i in tqdm(range(0,len(words))):
             for j in range(i+1,len(words)):
-                pair = MinPair(words[i], words[j])
+                pair = (words[i], words[j])
                 if self.check_minpair(pair):
                     minpairs.append(pair)
 
-        json_out = json.dumps([MinPair.obj_dict(pair) for pair in minpairs])
-        writefile(outfile, json_out)
-        print('Done! Generated', len(minpairs), 'minimal pairs')
+        return minpairs
 
-    def check_minpair(self, pair: MinPair) -> int:
+    def check_minpair(self, pair: WordPair) -> int:
         """
-        If the given pair si not a minpair, return NOT_MINPAIR; otherwise,
-        return, per case, PHONEME_MINPAIR, CHRONEME_MINPAIR and STRESS_MINPAIR
+        If the given pair is not a minpair, return NOT_MINPAIR; otherwise,
+        return, per case, PHONEME_MINPAIR, CHRONEME_MINPAIR or STRESS_MINPAIR
         """
         # Skip empty entries
-        if not pair.first.phonology or not pair.last.phonology:
+        if not pair[0].phonology or not pair[1].phonology:
             return False
         # A minimal pair is kept if it has an interesting difference.
         if self.keep_phonemes and self.check_phoneme_contrast(pair):
             return PHONEME_MINPAIR
         elif self.keep_chronemes and self.check_chroneme_contrast(pair):
             return CHRONEME_MINPAIR
         elif self.keep_stress and self.check_stress_contrast(pair):
@@ -103,28 +88,30 @@
         return False
 
     def print_human_readable_check(self, word1: Word, word2: Word) -> int:
         word1.print_human_readable()
         print("")
         word2.print_human_readable()
         print("")
-        verdict = self.check_minpair(MinPair(word1, word2))
+        verdict = self.check_minpair((word1, word2))
         if verdict == PHONEME_MINPAIR:
             print("minimal pair based on phoneme difference")
         elif verdict == CHRONEME_MINPAIR:
             print("minimal pair based on chroneme difference")
         elif verdict == STRESS_MINPAIR:
             print("minimal pair based on syllable stress difference")
         else:
             print("not minimal pair")
         return verdict
 
-    def check_phoneme_contrast(self, pair: MinPair) -> bool:
-        first = pair.first.phonology
-        last = pair.last.phonology
+    def check_phoneme_contrast(self, pair: WordPair) -> bool:
+        """Check if the two Words form a minimal pair based on a phoneme
+        difference"""
+        first = pair[0].phonology
+        last = pair[1].phonology
 
         # we have to work with same number of syllables
         if len(first) != len(last):
             return False
 
         diffs = []
         for i in range(0, len(first)):
@@ -137,17 +124,19 @@
                     diffs.append((syl1[j].sound, syl2[j].sound))
 
         if len(diffs) != 1:
             return False
 
         return (not self.optimise or self.check_optimised_phone_pair(diffs[0][0], diffs[0][1]))
 
-    def check_chroneme_contrast(self, pair: MinPair) -> bool:
-        first = pair.first.phonology
-        last = pair.last.phonology
+    def check_chroneme_contrast(self, pair: WordPair) -> bool:
+        """Check if the two `Word`s form a minimal pair based on a sound length
+        difference (i.e. a different chroneme)"""
+        first = pair[0].phonology
+        last = pair[1].phonology
 
         # we have to work with same number of syllables
         if len(first) != len(last):
             return False
 
         # find the number of chroneme differences; if, at any point, we
         # encounter a differnt sound, then we know the words are too different
@@ -162,17 +151,19 @@
                 if syl1[j].sound != syl2[j].sound:
                     return False
                 elif syl1[j].long != syl2[j].long:
                     chroneme_diffs += 1
 
         return chroneme_diffs >= 1
 
-    def check_stress_contrast(self, pair: MinPair) -> bool:
-        first = pair.first.phonology
-        last = pair.last.phonology
+    def check_stress_contrast(self, pair: WordPair) -> bool:
+        """Check if the two `Word`s form a minimal pair based on different
+        placcing of syllable stress, all sounds being the same"""
+        first = pair[0].phonology
+        last = pair[1].phonology
 
         # we have to work with same number of syllables
         if len(first) != len(last):
             return False
 
         fst_stress = []
         snd_stress = []
@@ -182,17 +173,17 @@
             fst_stress += first[i].stress
             snd_stress += last[i].stress
 
         return fst_stress != snd_stress
 
 ### Helper functions ###
 
-def differences(A: list, B: list) -> list:
-    """Given two lists, return pairs of elements that differ at the same index"""
-    return [(a, b) for a, b in zip(A, B) if a != b]
+def flatten(lst: list[list]) -> set[list]:
+    """Return the set of all elements belonging to the sublists of the list"""
+    return set(chain(*lst))
 
 def phoneme_list_to_pairs(phoneme_list: list[str]) -> list[tuple[str]]:
     """
     Hardcoding is a bad practice. And tiresome as well. Especially when you add a
     new sound: you have to manually add so many pairs!
 
     Thus, we use lists of phonemes to group similar sounds together. For
@@ -202,24 +193,20 @@
     """
     s = list(phoneme_list)
     # range(2, 2+1) returns all tuples that are exactly 2 in length - exactly
     # what we need
     pairs = chain.from_iterable(combinations(s, r) for r in range(2, 2+1))
     return list(pairs)
 
-def flatten(lst: list[list]) -> set[list]:
-    """Return the set of all elements belonging to the sublists of the list"""
-    return set(chain(*lst))
-
 def phoneme_lists_to_phoneme_pairs(phoneme_lists: list[list[str]]) -> set[list]:
     """
     Given a list of lists of phonemes, return the combined set of all phoneme
     pairs made from every individual list.
     """
-    return flatten(list(map(phoneme_list_to_pairs, phoneme_lists)))
+    return flatten([phoneme_list_to_pairs(list) for list in phoneme_lists])
 
 ### CONSTANTS ###
 
 """
 All sounds in a particular chain are hard to be distinguished from each other.
 
 Therefore, they form pairs of "interesting differences", which are used to
```

### Comparing `grzegorz-0.5.0/grzegorz/test.py` & `grzegorz-0.6.0/grzegorz/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,56 +45,56 @@
         expected = Syllable(".",[Phone("f", False), Phone("y", True), Phone("ɐ", False)])
         actual = Word("", "/fyːɐ/")
         self.assertListEqual(actual.phonology, [expected])
 
     def test_phoneme_contrast_r_and_m_not_optimised(self):
         w1 = Word("", "/barˈbaz/")
         w2 = Word("", "/bamˈbaz/")
-        self.assertTrue(g.check_phoneme_contrast(MinPair(w1, w2), False))
+        self.assertTrue(g.check_phoneme_contrast((w1, w2)))
 
     def test_phoneme_contrast_with_chroneme_difference(self):
         w1 = Word("", "/barˈbaz/")
         w2 = Word("", "/bar:ˈbaz/")
-        self.assertFalse(g.check_phoneme_contrast(MinPair(w1, w2), False))
+        self.assertFalse(g.check_phoneme_contrast((w1, w2)))
 
     def test_chroneme_contrast(self):
         w1 = Word("", "/barˈbaz/")
         w2 = Word("", "/bar:ˈbaz/")
-        self.assertTrue(g.check_chroneme_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_chroneme_contrast((w1, w2)))
 
     def test_chroneme_contrast_two_diffs(self):
         w1 = Word("", "/barˈbaz/")
         w2 = Word("", "/bar:ˈba:z/")
-        self.assertTrue(g.check_chroneme_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_chroneme_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_two_syllable(self):
         w1 = Word("", "/barˈbaz/")
         w2 = Word("", "/bar.baz/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_three_syllables_1(self):
         w1 = Word("", "/barˈbaz.do/")
         w2 = Word("", "/bar.baz.do/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_three_syllables_2(self):
         w1 = Word("", "/barˈbaz.do/")
         w2 = Word("", "/bar.bazˈdo/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_three_syllables_3(self):
         w1 = Word("", "/barˈbaz.do/")
         w2 = Word("", "/barˌbazˈdo/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_three_syllables_4(self):
         w1 = Word("", "/bar.baz.do/")
         w2 = Word("", "/barˌbazˈdo/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
     def test_syllable_stress_contrast_four_syllables_1(self):
         w1 = Word("", "/bar.baz.do.man/")
         w2 = Word("", "/barˌbazˈdo.man/")
-        self.assertTrue(g.check_stress_contrast(MinPair(w1, w2)))
+        self.assertTrue(g.check_stress_contrast((w1, w2)))
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `grzegorz-0.5.0/grzegorz/word.py` & `grzegorz-0.6.0/grzegorz/word.py`

 * *Files 16% similar despite different names*

```diff
@@ -122,66 +122,18 @@
                     syllable = Syllable(stress, sounds)
                     syllables.append(syllable)
                 stress = crnt
                 sounds = []
 
         return syllables
 
-    @staticmethod
-    def obj_dict(word):
-        """Return this class as a dictionary"""
-        dict = word.__dict__
-        # this might fail since the dictionary is mutated, and the same Word
-        # might be converted more than one time
-        try:
-            # We don't need to know about the sounds of the word; those can be
-            # computed
-            dict.pop('phonology')
-        except KeyError:
-            pass
-        return dict
-
-    @staticmethod
-    def from_dict(dict) -> 'Word':
-        """Deserialise this class from JSON"""
-        return Word(dict['text'], dict['ipa'])
-
-class MinPair:
-    """Two words in a pair. Voilà c'est tout."""
-    def __init__(self, first: Word, last: Word) -> None:
-        self.first = first;
-        self.last = last;
-
-    @staticmethod
-    def obj_dict(obj: 'MinPair'):
-        """Return this class as a dictionary"""
-        dict = obj.__dict__;
-        dict['first'] = Word.obj_dict(dict['first']);
-        dict['last'] = Word.obj_dict(dict['last']);
-        return dict
-
-    @staticmethod
-    def from_dict(dict) -> 'MinPair':
-        """Construct this class from a dictionary"""
-        word1 = Word.from_dict(dict['first'])
-        word2 = Word.from_dict(dict['last'])
-        return MinPair(word1, word2)
+WordPair = tuple[Word, Word]
 
 ### Helper functions ###
 
-def readfile(path: str) -> str:
-    """Return the contents of a file"""
-    with open(path, 'r', encoding='utf-8') as f:
-        return f.read()
-
-def writefile(path: str, text: str) -> None:
-    """Write `text` to the given path"""
-    with open(path, 'w', encoding='utf-8') as f:
-        f.write(text)
-
 def parse_ipa_characters(ipa: str) -> list[str]:
     """ Given an IPA transliteration, return all the IPA characters in it """
     # Remove any any forward slashes, square brackets or round parentheses that
     # may be used to indicate the type of pronunciation (rough, precise or
     # imprecise respectively)
     chars = re.sub(r"[\\/\[\]\(\)]", "", ipa)
     # Some scripts use `ː` to denote vowel length, some use `:`. Don't be
```

### Comparing `grzegorz-0.5.0/grzegorz/wordlist.py` & `grzegorz-0.6.0/grzegorz/wordlist.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 # grzegorz is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # grzegorz.  If not, see <https://www.gnu.org/licenses/>.
 
-from grzegorz.word import writefile
-
 import requests
 
-"""List of languages for which word lists can be fetched"""
 VALID_LANGUAGES = [
     # Germanic languages
     ('english', 'en'),
     ('german', 'de'),
     ('norwegian', 'no'),
     ('swedish', 'sv'),
     ('danish', 'da'),
@@ -58,77 +55,77 @@
     ('armenian', 'hy'),
     ('persian', 'fa'),
     ('hindi', 'hi'),
     ('tamil', 'ta'),
     ('chinese', 'zh'),
     ('japanese', 'ja'),
 ]
+"""
+List of languages for which word lists can be fetched, in tuple format, with the
+first element being the language full name and the second element being the
+language code
+"""
 
-"""This is where all the lists are fetched from"""
 RESOURCES_REPO_LINK = 'https://raw.githubusercontent.com/hermitdave/FrequencyWords/master/content/2016'
+"""All the wordlists are fetched from here"""
+
 
-def wordlist(lang, numwords, outfile) -> int:
+def wordlist(lang: str, upperbound: int, lowerbound: int = 0) -> list[str]:
     """
-    Fetch a word list of `numwords` and put it into `outfile` for the given
-    language, if it's valid
-    If the operation failed, then return 1, otherwise return 0
+    Return the most common words that are between index `lowerbound` and
+    `upperbound` in the given language. Note that the first element is always
+    the language name. If it isn't present, then the language is invalid.
     """
-    language = lang_name(lang)
     if not valid_lang(lang):
-        print(lang, "? I can't fetch a wordlist for that", sep='')
-        return 1
+        return []
+
+    language = lang_name(lang)
     link = wordlist_link_for_lang(lang)
-    words_kept_slice = slice(0, numwords)
+    words_kept_slice = slice(lowerbound, upperbound)
     raw_words = fetch_contents(link).splitlines()[words_kept_slice]
-    raw_words = list(map(format_line, raw_words))
+    raw_words = [line.split()[0] for line in raw_words]
     raw_words.insert(0, language)
-    writefile(outfile, '\n'.join(raw_words))
-    print("Fetched", numwords, language, "words into", outfile)
-    return 0
+    return raw_words
 
 def print_languages_list() -> None:
     for (lang, code) in sorted(VALID_LANGUAGES, key=lambda pair: pair[1]):
         print(code, ", ", lang, sep="")
 
 ### HELPER FUNCTIONS ###
 
-def valid_lang(lang):
-    """We only accept languages that are on the list"""
+def valid_lang(lang: str) -> bool:
+    """Check if `wordlist()` can fetch a wordlist for the given language or
+    language code"""
     for pair in VALID_LANGUAGES:
         if lang in pair:
             return True
     return False
 
-def lang_code(lang):
-    """Given a language, return its language code"""
+def lang_code(lang: str) -> str:
+    """Given a language, return its language code, provided it's in the
+    `VALID_LANGUAGES` property"""
     for pair in VALID_LANGUAGES:
         if lang in pair:
             _, code = pair
             return code
     return ''
 
-def lang_name(lang):
-    """Given a language, return its language fullname"""
+def lang_name(lang: str) -> str:
+    """Given a language, return its language fullname, provided it's in the
+    `VALID_LANGUAGES` property"""
     for pair in VALID_LANGUAGES:
         if lang in pair:
             name, _ = pair
             return name
     return ''
 
-def wordlist_link_for_lang(lang):
-    """Return the link to the wordlist for the given language"""
+def wordlist_link_for_lang(lang: str):
+    """Return the link to the wordlist for the given language, provided it is
+    valid"""
     code = lang_code(lang)
     link = RESOURCES_REPO_LINK + "/" + code + "/" + code + "_50k.txt"
     return link
 
-def fetch_contents(link):
+def fetch_contents(link: str):
     """Return the string containing the webpage at `link`"""
     res = requests.get(link)
     return res.text
-
-def format_line(line):
-    """
-    The format of the list we fetched is not perfect: we need to keep only the
-    first word on every line
-    """
-    first_word = line.split()[0]
-    return first_word
```

### Comparing `grzegorz-0.5.0/grzegorz.egg-info/PKG-INFO` & `grzegorz-0.6.0/grzegorz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grzegorz
-Version: 0.5.0
+Version: 0.6.0
 Summary: Minimal pair generator and phonetics tool
 Home-page: https://github.com/xylous/grzegorz
 Author: xylous
 Author-email: xylous.e@gmail.com
 Project-URL: Bug Tracker, https://github.com/xylous/grzegorz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `grzegorz-0.5.0/setup.cfg` & `grzegorz-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = grzegorz
-version = 0.5.0
+version = 0.6.0
 author = xylous
 author_email = xylous.e@gmail.com
 description = Minimal pair generator and phonetics tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/xylous/grzegorz
 project_urls =
```

