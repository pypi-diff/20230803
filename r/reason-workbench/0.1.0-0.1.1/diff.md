# Comparing `tmp/reason_workbench-0.1.0.tar.gz` & `tmp/reason_workbench-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reason_workbench-0.1.0.tar", last modified: Tue Aug  1 19:21:06 2023, max compression
+gzip compressed data, was "reason_workbench-0.1.1.tar", last modified: Thu Aug  3 21:36:04 2023, max compression
```

## Comparing `reason_workbench-0.1.0.tar` & `reason_workbench-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-01 19:21:06.017240 reason_workbench-0.1.0/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-01 19:21:06.016715 reason_workbench-0.1.0/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      189 2023-07-29 15:22:53.000000 reason_workbench-0.1.0/README.md
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-01 19:21:06.011314 reason_workbench-0.1.0/reason_workbench/
--rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.0/reason_workbench/__init__.py
--rw-r--r--   0 joshbottum   (501) staff       (20)    14350 2023-08-01 19:16:57.000000 reason_workbench-0.1.0/reason_workbench/main.py
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-01 19:21:06.015866 reason_workbench-0.1.0/reason_workbench.egg-info/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/SOURCES.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/dependency_links.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/entry_points.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/requires.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-01 19:21:05.000000 reason_workbench-0.1.0/reason_workbench.egg-info/top_level.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-01 19:21:06.017499 reason_workbench-0.1.0/setup.cfg
--rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-07-29 15:22:08.000000 reason_workbench-0.1.0/setup.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.941100 reason_workbench-0.1.1/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-03 21:36:04.940668 reason_workbench-0.1.1/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)      189 2023-07-29 15:22:53.000000 reason_workbench-0.1.1/README.md
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.936049 reason_workbench-0.1.1/reason_workbench/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.1/reason_workbench/__init__.py
+-rw-r--r--   0 joshbottum   (501) staff       (20)    17468 2023-08-03 21:31:08.000000 reason_workbench-0.1.1/reason_workbench/main.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.940068 reason_workbench-0.1.1/reason_workbench.egg-info/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/SOURCES.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/dependency_links.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/entry_points.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/requires.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/top_level.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-03 21:36:04.941263 reason_workbench-0.1.1/setup.cfg
+-rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-08-03 19:58:23.000000 reason_workbench-0.1.1/setup.py
```

### Comparing `reason_workbench-0.1.0/reason_workbench/main.py` & `reason_workbench-0.1.1/reason_workbench/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import csv
 import pandas as pd
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, pipeline
 import bert_score
 import logging
 import matplotlib.pyplot as plt
+from tqdm import tqdm
 
 # Disable warning messages from transformers
 logging.getLogger("transformers.modeling_utils").setLevel(logging.ERROR)
 
 
 def load_data_from_file(file_path):
     if file_path.endswith('.json'):
@@ -124,16 +125,14 @@
                 output_file.write("Type: " + record.get('type', 'N/A') + "\n")
                 output_file.write("Precision: " + str(round(record['precision'], 5)) + "\n")
                 output_file.write("Recall: " + str(round(record['recall'], 5)) + "\n")
                 output_file.write("F1 Score: " + str(round(record['f1'], 5)) + "\n")
                 output_file.write("=" * 10 + "\n")
 
 
-
-
 def plot_data(epoch_record):
     # Lists to store data for the plots
     prompt_types = []
     generation_times = []
     precisions = []
     recalls = []
     f1_scores = []
@@ -168,23 +167,58 @@
     plt.ylabel('Scores')
     plt.title('Prompt Types vs. BERTScores (Precision, Recall, F1)')
     plt.xticks([i + width for i in x], prompt_types, rotation=45, ha='right')
     plt.legend()
     plt.tight_layout()
     plt.show()
 
+def save_output_to_markdown(epoch_record):
+    with open("output.md", "w") as md_file:
+        # Write the common fields only once
+        md_file.write(f"# Model: {epoch_record['Example 1']['model_id']}\n")
+        md_file.write(f"Project: {epoch_record['Example 1'].get('project_id', 'N/A')}\n")
+        md_file.write(f"User: {epoch_record['Example 1']['user_id']}\n")
+        md_file.write("Run Date: " + datetime.datetime.fromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S') + "\n")
+        md_file.write("Model load time: " + str(round(epoch_record["Example 1"]["model_load_time"], 5)) + "\n")
+        md_file.write("Tokenizer load time: " + str(round(epoch_record["Example 1"]["tokenizer_load_time"], 5)) + "\n")
+        md_file.write("Pipeline load time: " + str(round(epoch_record["Example 1"]["pipeline_load_time"], 5)) + "\n")
+        md_file.write("=" * 30 + "\n\n")
+
+        # Loop through the examples and write the rest of the fields
+        for example_number, record in epoch_record.items():
+            if example_number != "Example 1":
+                md_file.write(f"## {example_number}\n")
+                md_file.write("Prompt: " + record.get('prompt', 'N/A') + "\n")
+                md_file.write("Generated Text: " + record.get('generated_answer', 'N/A') + "\n")
+                md_file.write("Reference Answer: " + record.get('reference_answer', 'N/A') + "\n")
+                md_file.write("Generation Time: " + str(round(record['generation_time'], 5)) + "\n")
+                md_file.write("Type: " + record.get('type', 'N/A') + "\n")
+                md_file.write("Precision: " + str(round(record['precision'], 5)) + "\n")
+                md_file.write("Recall: " + str(round(record['recall'], 5)) + "\n")
+                md_file.write("F1 Score: " + str(round(record['f1'], 5)) + "\n")
+                md_file.write("=" * 10 + "\n\n")
+
+
 
 def main():
     # Initialize input_data dictionary
     input_data = {}
+    valid_choices = ['1', '2', '3']
 
-    # Ask the user to choose the input data source
-    print("Would you like to run the Reasoning Workbench with the sample data or your own provided JSON or CSV file?")
-    print("Enter '1' for sample data, '2' for JSON, or '3' for CSV:")
-    user_choice = input()
+    while True:
+        # Ask the user to choose the input data source
+        print("Would you like to run the Reasoning Workbench with the sample data or your own provided JSON or CSV file?")
+        print("Enter '1' for sample data, '2' for JSON, or '3' for CSV:")
+        user_choice = input()
+        print()
+
+        if user_choice in valid_choices:
+            break
+        else:
+            print("Invalid choice. Please try again.")
     
     # Load data based on user choice
     if user_choice == '1':
         # Use the sample data dictionary
         input_data = {
             "user_id": "jbottum",
             "project_id": "project1",
@@ -231,43 +265,66 @@
         input_data = load_data_from_file(json_file_path)
     elif user_choice == '3':
         csv_file_path = input("Enter the path to your CSV file: ")
         input_data = load_data_from_file(csv_file_path)
     else:
         print("Invalid choice. Please try again.")
 
-    # Load tokenizer, model, and pipeline, and store those loading times
-    tokenizer_start_time = time.time()
-    tokenizer = AutoTokenizer.from_pretrained(input_data['model_id'])
-    tokenizer_end_time = time.time()
-
-    model_start_time = time.time()
-    model = AutoModelForSeq2SeqLM.from_pretrained(input_data['model_id'])
-    model_end_time = time.time()
-
-    pipe_start_time = time.time()
-    pipe = pipeline(task='text2text-generation', model=model, tokenizer=tokenizer, max_length=512)
-    pipe_end_time = time.time()
-
-    model_load_time = model_end_time - model_start_time
-    tokenizer_load_time = tokenizer_end_time - tokenizer_start_time
-    pipeline_load_time = pipe_end_time - pipe_start_time
-
-    # Generate prompt responses and collect data
-    epoch_record = generate_prompt_responses(input_data, pipe, model_load_time, tokenizer_load_time, pipeline_load_time)
-
-    # Print, Save, Plot based on user choice
-    print("Select the output options (for mulitple options, separate by comma e.g. 1,2:")
-    print("1. Printed Output")
-    print("2. File of Printed Output")
-    print("3. Plots of Output")
-    print("4. epoch_record.csv File")
-    print("5. epoch_record.json File")
-    user_output_choice = input()
-    user_output_choice = user_output_choice.split(',')
+    print("Setting up environment, loading models and generating responses...")
+    print()
+
+    with tqdm(total=4, desc="Loading Models", bar_format="{desc}: {percentage:3.0f}%|{bar:20}{r_bar}") as pbar:
+
+        # Load tokenizer, model, and pipeline, and store those loading times
+        pbar.set_description_str("Loading Tokenizer")
+        tokenizer_start_time = time.time()
+        tokenizer = AutoTokenizer.from_pretrained(input_data['model_id'])
+        tokenizer_end_time = time.time()
+        pbar.update(1)
+
+        pbar.set_description_str("Loading Model")
+        model_start_time = time.time()
+        model = AutoModelForSeq2SeqLM.from_pretrained(input_data['model_id'])
+        model_end_time = time.time()
+        pbar.update(1)
+
+        pbar.set_description_str("Creating Pipeline")
+        pipe_start_time = time.time()
+        pipe = pipeline(task='text2text-generation', model=model, tokenizer=tokenizer, max_length=512)
+        pipe_end_time = time.time()
+        pbar.update(1)
+
+        model_load_time = model_end_time - model_start_time
+        tokenizer_load_time = tokenizer_end_time - tokenizer_start_time
+        pipeline_load_time = pipe_end_time - pipe_start_time
+
+        # Generate prompt responses and collect data
+        pbar.set_description_str("Generating responses")
+        epoch_record = generate_prompt_responses(input_data, pipe, model_load_time, tokenizer_load_time, pipeline_load_time)
+        pbar.update(1)
+
+    valid_choices = ['1', '2', '3', '4', '5','6']
+    
+    while True:
+        print("Select the output options (for multiple options, separate by comma e.g. 1,2):")
+        print("1. Printed Output")
+        print("2. File of Printed Output")
+        print("3. Plots of Output")
+        print("4. epoch_record.csv File")
+        print("5. epoch_record.json File")
+        print("6. Markdown Output")  # Add this option for Markdown output
+        user_output_choice = input().strip()
+        user_output_choices = user_output_choice.split(',')
+
+        if all(choice in valid_choices for choice in user_output_choices):
+            break
+        else:
+            print("Invalid choice. Please try again.")
+    
+    print()
 
     if '1' in user_output_choice:
         print_output(epoch_record)
 
     if '2' in user_output_choice:
         print_output_to_file(epoch_record)
 
@@ -279,11 +336,17 @@
         df = pd.DataFrame.from_dict(epoch_record, orient='index')
         df.to_csv("epoch_record.csv", index=False)
 
     if '5' in user_output_choice:
         # Save epoch_record as JSON
         with open("epoch_record.json", "w") as jsonfile:
             json.dump(epoch_record, jsonfile)
+    if '6' in user_output_choice:
+        # Save output to Markdown
+        save_output_to_markdown(epoch_record)
+
+
+    
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

