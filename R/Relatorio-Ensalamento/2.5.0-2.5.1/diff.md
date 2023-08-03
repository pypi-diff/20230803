# Comparing `tmp/Relatorio_Ensalamento-2.5.0.tar.gz` & `tmp/Relatorio_Ensalamento-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio_Ensalamento-2.5.0.tar", last modified: Mon Jul 31 16:24:22 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.5.1.tar", last modified: Thu Aug  3 17:34:12 2023, max compression
```

## Comparing `Relatorio_Ensalamento-2.5.0.tar` & `Relatorio_Ensalamento-2.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:24:22.979505 Relatorio_Ensalamento-2.5.0/
--rw-rw-rw-   0        0        0      549 2023-07-31 16:24:22.979505 Relatorio_Ensalamento-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:24:22.946196 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    50274 2023-07-31 16:23:28.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:24:22.967588 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      549 2023-07-31 16:24:22.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-31 16:24:22.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:24:22.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-31 16:24:22.000000 Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 16:24:22.972501 Relatorio_Ensalamento-2.5.0/Sugestao/
--rw-rw-rw-   0        0        0    59471 2023-07-14 21:19:02.000000 Relatorio_Ensalamento-2.5.0/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.5.0/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:24:22.977525 Relatorio_Ensalamento-2.5.0/Unificar_XML/
--rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.5.0/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.5.0/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-31 16:24:22.984117 Relatorio_Ensalamento-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-31 16:24:20.000000 Relatorio_Ensalamento-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:34:12.060435 Relatorio_Ensalamento-2.5.1/
+-rw-rw-rw-   0        0        0      506 2023-08-03 17:34:12.061952 Relatorio_Ensalamento-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 17:34:11.979128 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    50274 2023-07-31 16:23:28.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:34:12.012730 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-08-03 17:34:11.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-08-03 17:34:11.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:34:11.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-03 17:34:11.000000 Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 17:34:12.035835 Relatorio_Ensalamento-2.5.1/Sugestao/
+-rw-rw-rw-   0        0        0    59519 2023-08-03 17:33:30.000000 Relatorio_Ensalamento-2.5.1/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.5.1/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:34:12.055118 Relatorio_Ensalamento-2.5.1/Unificar_XML/
+-rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.5.1/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.5.1/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-08-03 17:34:12.068961 Relatorio_Ensalamento-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-08-03 17:33:30.000000 Relatorio_Ensalamento-2.5.1/setup.py
```

### Comparing `Relatorio_Ensalamento-2.5.0/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.5.1/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.5.0/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.5.1/Sugestao/Sugestao.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,27 @@
         self.diferenca_capacidade = diferenca_capacidade
         self.analise_capacidade = analise_capacidade
         self.capacidade_sala = capacidade_sala
 
         if capacidade_sala == 0:
             porcentagem_utilizacao = 0 - alunos_matriculados
         else:
-            porcentagem_utilizacao = (alunos_matriculados / capacidade_sala) * 100
-            porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
+            try:
+                porcentagem_utilizacao = (alunos_matriculados / capacidade_sala) * 100
+            except:
+                print(alunos_matriculados,'|',capacidade_sala)
+
 
         self.porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
 
 class Subutilizada:
     def __init__(self, sala, disciplina):
         self.sala = sala
         self.disciplina = disciplina
+
 class AmbienteDeAprendizagem:
     def __init__(self, nome_sala, nome_sala_abrev, capacidade_sala, status, disciplina, tipo, tipo_detalhado, escola,curso):
         self.nome_sala = nome_sala
         self.nome_sala_abrev = nome_sala_abrev
 
         try:
             self.capacidade_sala = int(capacidade_sala)
@@ -1049,15 +1053,15 @@
         # ordenando em ordem crescente a lista
         list_empty_classroom = sorted(list_empty_classroom, key=lambda x: x.capacidade_sala)
 
         # armazenando lista de prioridades da escola
         try:
             list_blocos = dict_retorna_prioridade_escola[data[1]["Escola"]]
         except:
-            continue
+            list_blocos = []
 
         # lista que vai ser inserida como sugestão
         list_aux = []
 
         # todo 1 verificação
         # verificar o bloco atual e o tipo detalhado
         for classroom in list_empty_classroom:
```

### Comparing `Relatorio_Ensalamento-2.5.0/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.5.1/Unificar_XML/Unificar_XML.py`

 * *Files identical despite different names*

