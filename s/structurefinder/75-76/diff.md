# Comparing `tmp/structurefinder-75.tar.gz` & `tmp/structurefinder-76.tar.gz`

## Comparing `structurefinder-75.tar` & `structurefinder-76.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structurefinder-75/.gitattributes
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 structurefinder-75/StructureFinder.spec
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 structurefinder-75/StructureFinder_linux.spec
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 structurefinder-75/StructureFinder_mac.spec
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 structurefinder-75/install_all_requirements
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 structurefinder-75/install_all_requirements.bat
--rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-75/install_min_requirements
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 structurefinder-75/pytest.ini
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 structurefinder-75/requirements.txt
--rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-75/strf
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 structurefinder-75/strf.bat
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 structurefinder-75/strf_cmd
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 structurefinder-75/strf_cmd.bat
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 structurefinder-75/strf_web
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 structurefinder-75/update.exe
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 structurefinder-75/docs/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/docs/__init__.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 structurefinder-75/docs/changes.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 structurefinder-75/docs/commandline.rst
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 structurefinder-75/docs/conf.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 structurefinder-75/docs/example.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 structurefinder-75/docs/index.rst
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 structurefinder-75/docs/indexing.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 structurefinder-75/docs/installation.rst
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 structurefinder-75/docs/main.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 structurefinder-75/docs/make.bat
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 structurefinder-75/docs/misc.rst
--rw-r--r--   0        0        0   112698 2020-02-02 00:00:00.000000 structurefinder-75/docs/pics/strf_1.png
--rw-r--r--   0        0        0    58105 2020-02-02 00:00:00.000000 structurefinder-75/docs/pics/strf_2.png
--rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 structurefinder-75/docs/pics/strf_4.png
--rw-r--r--   0        0        0    32402 2020-02-02 00:00:00.000000 structurefinder-75/docs/pics/strf_adv.png
--rw-r--r--   0        0        0   167550 2020-02-02 00:00:00.000000 structurefinder-75/docs/pics/strf_web.png
--rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-75/icons/strf.ico
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 structurefinder-75/icons/strf.png
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/__init__.py
--rw-r--r--   0        0        0    56962 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/strf.py
--rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/strf_cmd.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/ccdc/__init__.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/ccdc/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/__init__.py
--rw-r--r--   0        0        0   170898 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/bottle.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/strf_web.py
--rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/favicon.ico
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/strf_web.css
--rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/strf_web.js
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/strf_web_csd.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/custom.css
--rw-r--r--   0        0        0    26132 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css
--rw-r--r--   0        0        0    47706 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map
--rw-r--r--   0        0        0    23409 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css
--rw-r--r--   0        0        0    25648 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map
--rw-r--r--   0        0        0   146010 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css
--rw-r--r--   0        0        0   389287 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map
--rw-r--r--   0        0        0   121200 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css
--rw-r--r--   0        0        0   542194 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map
--rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css
--rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf
--rw-r--r--   0        0        0    38239 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   202471 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0    80776 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    44476 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62850 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41236 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0    69707 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js
--rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/npm.js
--rw-r--r--   0        0        0    24977 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/clipboard/clipboard.js
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js
--rw-r--r--   0        0        0   128442 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/bower.json
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/license.txt
--rw-r--r--   0        0        0    88141 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css
--rw-r--r--   0        0        0   678867 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js
--rw-r--r--   0        0        0    75404 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css
--rw-r--r--   0        0        0   299228 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js
--rw-r--r--   0        0        0   107093 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css
--rw-r--r--   0        0        0   943882 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js
--rw-r--r--   0        0        0    92412 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css
--rw-r--r--   0        0        0   405298 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/advanced_search.tpl
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/simpl_search.tpl
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/spgr.tpl
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/strf_base.tpl
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/cgi_ui/views/strf_web.tpl
--rw-r--r--   0        0        0   128445 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/__init__.py
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/jquery.min.js
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/mol_file_writer.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/sdm.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/displaymol/write_html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/__init__.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/strf_dbpasswd.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/strf_dbpasswd.ui
--rw-r--r--   0        0        0   109362 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/strf_main.py
--rw-r--r--   0        0        0   127483 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/strf_main.ui
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/table_model.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/table_view.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/gui/table_view_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/dialogs.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/download.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/exporter.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/settings.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/update_check.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/misc/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/p4pfile/__init__.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/p4pfile/p4p_reader.py
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pg8000/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pg8000/_version.py
--rw-r--r--   0        0        0    89534 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pg8000/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/core/__init__.py
--rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/core/lattice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/util/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/util/num_utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/pymatgen/util/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/cif.textx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/compare.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/constants.py
--rw-r--r--   0        0        0    54881 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/database_handler.py
--rw-r--r--   0        0        0    12330 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/filecrawler.py
--rw-r--r--   0        0        0    20554 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/fileparser.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/misc.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/spinner.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/unitcell.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/searcher/worker.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/__init__.py
--rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/atoms.py
--rw-r--r--   0        0        0    53857 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/cards.py
--rw-r--r--   0        0        0    44739 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/dsrmath.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/elements.py
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/misc.py
--rw-r--r--   0        0        0    45843 2020-02-02 00:00:00.000000 structurefinder-75/src/structurefinder/shelxfile/shelx.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 structurefinder-75/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 structurefinder-75/LICENSE
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 structurefinder-75/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 structurefinder-75/pyproject.toml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 structurefinder-75/PKG-INFO
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structurefinder-76/.gitattributes
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 structurefinder-76/StructureFinder.spec
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 structurefinder-76/StructureFinder_linux.spec
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 structurefinder-76/StructureFinder_mac.spec
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 structurefinder-76/install_all_requirements
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 structurefinder-76/install_all_requirements.bat
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-76/install_min_requirements
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 structurefinder-76/pytest.ini
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 structurefinder-76/requirements.txt
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-76/strf
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 structurefinder-76/strf.bat
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 structurefinder-76/strf_cmd
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 structurefinder-76/strf_cmd.bat
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 structurefinder-76/strf_web
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 structurefinder-76/update.exe
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 structurefinder-76/docs/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/docs/__init__.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 structurefinder-76/docs/changes.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 structurefinder-76/docs/commandline.rst
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 structurefinder-76/docs/conf.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 structurefinder-76/docs/example.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 structurefinder-76/docs/index.rst
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 structurefinder-76/docs/indexing.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 structurefinder-76/docs/installation.rst
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 structurefinder-76/docs/main.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 structurefinder-76/docs/make.bat
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 structurefinder-76/docs/misc.rst
+-rw-r--r--   0        0        0   112698 2020-02-02 00:00:00.000000 structurefinder-76/docs/pics/strf_1.png
+-rw-r--r--   0        0        0    58105 2020-02-02 00:00:00.000000 structurefinder-76/docs/pics/strf_2.png
+-rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 structurefinder-76/docs/pics/strf_4.png
+-rw-r--r--   0        0        0    32402 2020-02-02 00:00:00.000000 structurefinder-76/docs/pics/strf_adv.png
+-rw-r--r--   0        0        0   167550 2020-02-02 00:00:00.000000 structurefinder-76/docs/pics/strf_web.png
+-rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-76/icons/strf.ico
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 structurefinder-76/icons/strf.png
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/__init__.py
+-rw-r--r--   0        0        0    57019 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/strf.py
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/strf_cmd.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/ccdc/__init__.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/ccdc/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/__init__.py
+-rw-r--r--   0        0        0   170898 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/bottle.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/strf_web.py
+-rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/favicon.ico
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/strf_web.css
+-rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/strf_web.js
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/strf_web_csd.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/custom.css
+-rw-r--r--   0        0        0    26132 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css
+-rw-r--r--   0        0        0    47706 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map
+-rw-r--r--   0        0        0    23409 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css
+-rw-r--r--   0        0        0    25648 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map
+-rw-r--r--   0        0        0   146010 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css
+-rw-r--r--   0        0        0   389287 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map
+-rw-r--r--   0        0        0   121200 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css
+-rw-r--r--   0        0        0   542194 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css
+-rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0    38239 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   202471 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0    80776 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    44476 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62850 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41236 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0    69707 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js
+-rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/npm.js
+-rw-r--r--   0        0        0    24977 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/clipboard/clipboard.js
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js
+-rw-r--r--   0        0        0   128442 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/bower.json
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/license.txt
+-rw-r--r--   0        0        0    88141 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css
+-rw-r--r--   0        0        0   678867 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js
+-rw-r--r--   0        0        0    75404 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css
+-rw-r--r--   0        0        0   299228 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js
+-rw-r--r--   0        0        0   107093 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css
+-rw-r--r--   0        0        0   943882 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js
+-rw-r--r--   0        0        0    92412 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css
+-rw-r--r--   0        0        0   405298 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/advanced_search.tpl
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/simpl_search.tpl
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/spgr.tpl
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/strf_base.tpl
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/cgi_ui/views/strf_web.tpl
+-rw-r--r--   0        0        0   128445 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/__init__.py
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/jquery.min.js
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/mol_file_writer.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/sdm.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/displaymol/write_html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/__init__.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/strf_dbpasswd.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/strf_dbpasswd.ui
+-rw-r--r--   0        0        0   109362 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/strf_main.py
+-rw-r--r--   0        0        0   127483 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/strf_main.ui
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/table_model.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/table_view.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/gui/table_view_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/dialogs.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/download.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/exporter.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/settings.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/update_check.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/misc/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/p4pfile/__init__.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/p4pfile/p4p_reader.py
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pg8000/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pg8000/_version.py
+-rw-r--r--   0        0        0    89534 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pg8000/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/core/__init__.py
+-rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/core/lattice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/util/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/util/num_utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/pymatgen/util/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/cif.textx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/compare.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/constants.py
+-rw-r--r--   0        0        0    54881 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/database_handler.py
+-rw-r--r--   0        0        0    12330 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/filecrawler.py
+-rw-r--r--   0        0        0    20554 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/fileparser.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/misc.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/spinner.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/unitcell.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/searcher/worker.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/__init__.py
+-rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/atoms.py
+-rw-r--r--   0        0        0    53857 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/cards.py
+-rw-r--r--   0        0        0    44739 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/dsrmath.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/elements.py
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/misc.py
+-rw-r--r--   0        0        0    45843 2020-02-02 00:00:00.000000 structurefinder-76/src/structurefinder/shelxfile/shelx.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 structurefinder-76/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 structurefinder-76/LICENSE
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 structurefinder-76/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 structurefinder-76/pyproject.toml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 structurefinder-76/PKG-INFO
```

### Comparing `structurefinder-75/StructureFinder.spec` & `structurefinder-76/StructureFinder.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-75/StructureFinder_linux.spec` & `structurefinder-76/StructureFinder_linux.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-75/StructureFinder_mac.spec` & `structurefinder-76/StructureFinder_mac.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/Makefile` & `structurefinder-76/docs/Makefile`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/changes.txt` & `structurefinder-76/docs/changes.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 StructureFinder Changelog
 -------------------------
 
+* v76 Hardened file indexer against damaged zip files.
+* v75 Fixed merging of databases where a table, e.g. the authors table, is empty.
+* v74 Several small improvements.
 * v73 Minor bugs fixed. New pypi package added: [https://pypi.org/project/structurefinder](https://pypi.org/project/structurefinder)
 * v72 Use _iucr_refine_instructions_details if _shelx_res_file is not found in CIF.
 * v71 Fixed crash when appending a database while no database is opened. Show labels in structure view.
 * v70 Small improvements.
 * v69 Add merging of two databases.
 * v68 New icons and small bugfix.
 * v67 Gives the user the possibility to set the path of the CellCheckCSD executable itself.
```

### Comparing `structurefinder-75/docs/commandline.rst` & `structurefinder-76/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/conf.py` & `structurefinder-76/docs/conf.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/example.rst` & `structurefinder-76/docs/example.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/indexing.rst` & `structurefinder-76/docs/indexing.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/installation.rst` & `structurefinder-76/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/main.rst` & `structurefinder-76/docs/main.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/make.bat` & `structurefinder-76/docs/make.bat`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/misc.rst` & `structurefinder-76/docs/misc.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/pics/strf_1.png` & `structurefinder-76/docs/pics/strf_1.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/pics/strf_2.png` & `structurefinder-76/docs/pics/strf_2.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/pics/strf_4.png` & `structurefinder-76/docs/pics/strf_4.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/pics/strf_adv.png` & `structurefinder-76/docs/pics/strf_adv.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/docs/pics/strf_web.png` & `structurefinder-76/docs/pics/strf_web.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/icons/strf.ico` & `structurefinder-76/icons/strf.ico`

 * *Files identical despite different names*

### Comparing `structurefinder-75/icons/strf.png` & `structurefinder-76/icons/strf.png`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/strf.py` & `structurefinder-76/src/structurefinder/strf.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         self.ui.setupUi(self)
         self.set_window_size_and_position()
         font = QtGui.QFont()
         font.setFamily("Courier")
         font.setStyleHint(QtGui.QFont.Monospace)
         self.ui.SHELXplainTextEdit.setFont(font)
         self.statusBar().showMessage(f'StructureFinder version {VERSION}')
+        self.upd = None
         self.maxfiles = 0
         self.dbfdesc = None
         self.dbfilename = db_file_name
         self.tmpfile = False  # indicates wether a tmpfile or any other db file is used
         self.abort_import_button = QPushButton('Abort Indexing')
         self.progress = QProgressBar(self)
         self.progress.setFormat('')
@@ -228,19 +229,19 @@
         self.resize(wsettings.size)
         self.move(wsettings.position)
         if wsettings.maximized:
             self.showMaximized()
 
     def checkfor_version(self):
         url = 'https://dkratzert.de/files/structurefinder/version.txt'
-        upd = MyDownloader(self, url)
-        upd.finished.connect(self.show_update_warning)
-        upd.failed.connect(upd.failed_to_download)
-        upd.progress.connect(upd.print_status)
-        upd.start()
+        self.upd = MyDownloader(url=url)
+        self.upd.finished.connect(self.show_update_warning)
+        self.upd.failed.connect(self.upd.failed_to_download)
+        self.upd.progress.connect(self.upd.print_status)
+        self.upd.start()
 
     def show_update_warning(self, reply: bytes):
         """
         Reads the reply from the server and displays a warning in case of an old version.
         """
         remote_version = 0
         try:
```

### Comparing `structurefinder-75/src/structurefinder/strf_cmd.py` & `structurefinder-76/src/structurefinder/strf_cmd.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/ccdc/query.py` & `structurefinder-76/src/structurefinder/ccdc/query.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/bottle.py` & `structurefinder-76/src/structurefinder/cgi_ui/bottle.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/strf_web.py` & `structurefinder-76/src/structurefinder/cgi_ui/strf_web.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/favicon.ico` & `structurefinder-76/src/structurefinder/cgi_ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/strf_web.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/strf_web.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/strf_web.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/strf_web.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/strf_web_csd.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/strf_web_csd.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/clipboard/clipboard.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/clipboard/clipboard.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/bower.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/bower.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/license.txt` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/license.txt`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json` & `structurefinder-76/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/advanced_search.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/advanced_search.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/simpl_search.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/simpl_search.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/spgr.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/spgr.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/strf_base.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/strf_base.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/cgi_ui/views/strf_web.tpl` & `structurefinder-76/src/structurefinder/cgi_ui/views/strf_web.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js` & `structurefinder-76/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/jquery.min.js` & `structurefinder-76/src/structurefinder/displaymol/jquery.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/mol_file_writer.py` & `structurefinder-76/src/structurefinder/displaymol/mol_file_writer.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/molecule2D.py` & `structurefinder-76/src/structurefinder/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/sdm.py` & `structurefinder-76/src/structurefinder/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/displaymol/write_html.py` & `structurefinder-76/src/structurefinder/displaymol/write_html.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/strf_dbpasswd.py` & `structurefinder-76/src/structurefinder/gui/strf_dbpasswd.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/strf_dbpasswd.ui` & `structurefinder-76/src/structurefinder/gui/strf_dbpasswd.ui`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/strf_main.py` & `structurefinder-76/src/structurefinder/gui/strf_main.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/strf_main.ui` & `structurefinder-76/src/structurefinder/gui/strf_main.ui`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/table_model.py` & `structurefinder-76/src/structurefinder/gui/table_model.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/table_view.py` & `structurefinder-76/src/structurefinder/gui/table_view.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/gui/table_view_example.py` & `structurefinder-76/src/structurefinder/gui/table_view_example.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/misc/dialogs.py` & `structurefinder-76/src/structurefinder/misc/dialogs.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/misc/download.py` & `structurefinder-76/src/structurefinder/misc/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 
 class MyDownloader(QThread):
     progress = pyqtSignal(str)
     failed = pyqtSignal(int)
     finished = pyqtSignal(bytes)
 
-    def __init__(self, parent, url: str):
-        super().__init__(parent)
+    def __init__(self, url: str):
+        super().__init__()
         self.url = url
 
     def run(self):
         try:
             self.download(self.url)
         except requests.RequestException as e:
             print('Could not connect to download server')
@@ -55,13 +55,13 @@
     w.show()
 
 
     def foo(bar: bytes):
         print(bar.decode('ascii'))
 
 
-    upd = MyDownloader(None, "https://dkratzert.de/files/structurefinder/version.txt")
+    upd = MyDownloader(url="https://dkratzert.de/files/structurefinder/version.txt")
     upd.finished.connect(foo)
     upd.failed.connect(upd.failed_to_download)
     upd.progress.connect(upd.print_status)
     upd.start()
     sys.exit(app.exec_())
```

### Comparing `structurefinder-75/src/structurefinder/misc/exporter.py` & `structurefinder-76/src/structurefinder/misc/exporter.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/misc/settings.py` & `structurefinder-76/src/structurefinder/misc/settings.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/misc/update_check.py` & `structurefinder-76/src/structurefinder/misc/update_check.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/p4pfile/p4p_reader.py` & `structurefinder-76/src/structurefinder/p4pfile/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/pg8000/__init__.py` & `structurefinder-76/src/structurefinder/pg8000/__init__.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/pg8000/core.py` & `structurefinder-76/src/structurefinder/pg8000/core.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/pymatgen/core/lattice.py` & `structurefinder-76/src/structurefinder/pymatgen/core/lattice.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/pymatgen/util/num_utils.py` & `structurefinder-76/src/structurefinder/pymatgen/util/num_utils.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/compare.py` & `structurefinder-76/src/structurefinder/searcher/compare.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/constants.py` & `structurefinder-76/src/structurefinder/searcher/constants.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/database_handler.py` & `structurefinder-76/src/structurefinder/searcher/database_handler.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/filecrawler.py` & `structurefinder-76/src/structurefinder/searcher/filecrawler.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/fileparser.py` & `structurefinder-76/src/structurefinder/searcher/fileparser.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/misc.py` & `structurefinder-76/src/structurefinder/searcher/misc.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/spinner.py` & `structurefinder-76/src/structurefinder/searcher/spinner.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/unitcell.py` & `structurefinder-76/src/structurefinder/searcher/unitcell.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/searcher/worker.py` & `structurefinder-76/src/structurefinder/searcher/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import os
 import re
 import time
+from contextlib import suppress
+from pathlib import Path
 from typing import Optional, Union
+from zipfile import BadZipFile
 
 import gemmi
 from PyQt5 import QtCore
 
+from structurefinder.misc.dialogs import bug_found_warning
 from structurefinder.searcher.database_handler import StructureTable
 from structurefinder.searcher.filecrawler import filewalker_walk, fill_db_with_cif_data, MyZipReader, \
     MyTarReader, fill_db_with_res_data
 from structurefinder.searcher.fileparser import CifFile
 from structurefinder.shelxfile.shelx import ShelXFile
 
 DEBUG = False
@@ -31,17 +35,20 @@
         self.lastid = lastid
         self.excludes = [] if not excludes else excludes
         self.files_indexed = 0
         if standalone:
             self.files_indexed = self.index_files()
 
     def index_files(self):
-        return self.put_files_in_db(searchpath=self.searchpath, structures=self.structures,
+        try:
+            return self.put_files_in_db(searchpath=self.searchpath, structures=self.structures,
                                     fillres=self.add_res_files, excludes=self.excludes,
                                     fillcif=self.add_cif_files, lastid=self.lastid)
+        except Exception:
+            self.finished.emit('The indexer has crashed. Please report this problem.')
 
     def put_files_in_db(self, searchpath: str = '', excludes: Union[list, None] = None, lastid: int = 1,
                         structures=None, fillcif=True, fillres=True) -> int:
         """
         Imports files from a certain directory
         """
         excludes = [] if not excludes else excludes
@@ -53,15 +60,15 @@
         zipcifs = 0
         rescount = 0
         cifcount = 0
         time1 = time.perf_counter()
         patterns = ['*.cif', '*.zip', '*.tar.gz', '*.tar.bz2', '*.tgz', '*.res']
         filelist = filewalker_walk(str(searchpath), patterns, excludes=excludes)
         if DEBUG:
-            print(f'Time for file list: {time.perf_counter()-time1:1} s.')
+            print(f'Time for file list: {time.perf_counter() - time1:1} s.')
         filecount = len(filelist)
         self.number_of_files.emit(filecount)
         options = {}
         for filenum, (filepth, name) in enumerate(filelist, start=1):
             if filenum % 1000 == 0:
                 print(f'{filenum} files...')
                 self.structures.database.commit_db()
@@ -71,21 +78,23 @@
                 return 0
             fullpath = os.path.join(filepth, name)
             options['modification_time'] = time.strftime('%Y-%m-%d', time.gmtime(os.path.getmtime(fullpath)))
             options['file_size'] = int(os.stat(str(fullpath)).st_size)
             cif = CifFile(options=options)
             self.progress.emit(filenum)
             if name.endswith('.cif') and fillcif:
+                cifok = False
                 doc = gemmi.cif.Document()
                 doc.source = fullpath
                 try:
                     doc.parse_file(fullpath)
                 except ValueError:
                     continue
-                cifok = cif.parsefile(doc)
+                with suppress(Exception):
+                    cifok = cif.parsefile(doc)
                 if not cifok:
                     if DEBUG:
                         print(f"Could not parse (.cif): {fullpath}")
                     continue
                 try:
                     tst = fill_db_with_cif_data(cif, filename=name, path=filepth, structure_id=lastid,
                                                 structures=self.structures)
@@ -100,33 +109,43 @@
                 num += 1
                 lastid += 1
                 self.progress.emit(filenum)
                 continue
             if (name.endswith('.zip') or name.endswith('.tar.gz') or name.endswith('.tar.bz2')
                 or name.endswith('.tgz')) and fillcif:
                 if fullpath.endswith('.zip'):
-                    z = MyZipReader(fullpath)
+                    try:
+                        z = MyZipReader(fullpath)
+                    except BadZipFile:
+                        print(f'Bad zip file skipped: {fullpath}')
+                        continue
                     filecount = filecount + len(z)
                     self.number_of_files.emit(filecount)
                 else:
-                    z = MyTarReader(fullpath)
+                    try:
+                        z = MyTarReader(fullpath)
+                    except Exception:
+                        print(f'Bad tar file skipped: {fullpath}')
+                        continue
                     filecount = filecount + len(z)
                     self.number_of_files.emit(filecount)
                 for zippedfile in z:  # the list of cif files in the zip file
+                    cifok = False
                     if not zippedfile:
                         continue
                     # Important here to re-initialize empty cif dictionary:
                     cif = CifFile(options=options)
                     omit = False
                     for ex in excludes:  # remove excludes
                         if re.search(ex, z.cifpath, re.I):
                             omit = True
                     if omit:
                         continue
-                    cifok = cif.parsefile(zippedfile)
+                    with suppress(Exception):
+                        cifok = cif.parsefile(zippedfile)
                     if not cifok:
                         if DEBUG:
                             print(f"Could not parse (zipped): {fullpath}")
                         continue
                     try:
                         tst = fill_db_with_cif_data(cif, filename=z.cifname, path=fullpath, structure_id=lastid,
                                                     structures=self.structures)
@@ -152,16 +171,17 @@
                     res = ShelXFile(fullpath)
                 except Exception as e:
                     if DEBUG:
                         print(e)
                         print(f"Could not parse (.res): {fullpath}")
                     continue
                 if res:
-                    tst = fill_db_with_res_data(res, filename=name, path=filepth, structure_id=lastid,
-                                                structures=self.structures, options=options)
+                    with suppress(Exception):
+                        tst = fill_db_with_res_data(res, filename=name, path=filepth, structure_id=lastid,
+                                                    structures=self.structures, options=options)
                 if not tst:
                     if DEBUG:
                         print('res file not added:', fullpath)
                     continue
                 num += 1
                 rescount += 1
                 lastid += 1
```

### Comparing `structurefinder-75/src/structurefinder/shelxfile/atoms.py` & `structurefinder-76/src/structurefinder/shelxfile/atoms.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/shelxfile/cards.py` & `structurefinder-76/src/structurefinder/shelxfile/cards.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/shelxfile/dsrmath.py` & `structurefinder-76/src/structurefinder/shelxfile/dsrmath.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/shelxfile/elements.py` & `structurefinder-76/src/structurefinder/shelxfile/elements.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/shelxfile/misc.py` & `structurefinder-76/src/structurefinder/shelxfile/misc.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/src/structurefinder/shelxfile/shelx.py` & `structurefinder-76/src/structurefinder/shelxfile/shelx.py`

 * *Files identical despite different names*

### Comparing `structurefinder-75/.gitignore` & `structurefinder-76/.gitignore`

 * *Files identical despite different names*

### Comparing `structurefinder-75/LICENSE` & `structurefinder-76/LICENSE`

 * *Files identical despite different names*

### Comparing `structurefinder-75/README.md` & `structurefinder-76/README.md`

 * *Files identical despite different names*

### Comparing `structurefinder-75/pyproject.toml` & `structurefinder-76/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structurefinder-75/PKG-INFO` & `structurefinder-76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structurefinder
-Version: 75
+Version: 76
 Summary: Search X-ray structures on your hard drive
 Project-URL: Homepage, https://dkratzert.de/structurefinder.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/StructureFinder/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

