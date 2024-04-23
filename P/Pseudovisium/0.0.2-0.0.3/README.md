# Comparing `tmp/Pseudovisium-0.0.2.tar.gz` & `tmp/Pseudovisium-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pseudovisium-0.0.2.tar", last modified: Thu Apr 18 09:29:18 2024, max compression
+gzip compressed data, was "Pseudovisium-0.0.3.tar", last modified: Tue Apr 23 09:38:37 2024, max compression
```

## Comparing `Pseudovisium-0.0.2.tar` & `Pseudovisium-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-18 09:29:18.189999 Pseudovisium-0.0.2/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.2/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-18 09:29:18.189773 Pseudovisium-0.0.2/PKG-INFO
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-18 09:29:18.188159 Pseudovisium-0.0.2/Pseudovisium/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.2/Pseudovisium/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    58479 2024-04-17 14:18:02.000000 Pseudovisium-0.0.2/Pseudovisium/pseudovisium_generate.py
--rw-r--r--   0 k23030440   (504) staff       (20)    14626 2024-04-16 20:47:21.000000 Pseudovisium-0.0.2/Pseudovisium/pseudovisium_merge.py
--rw-r--r--   0 k23030440   (504) staff       (20)    43149 2024-04-17 07:10:22.000000 Pseudovisium-0.0.2/Pseudovisium/pseudovisium_qc.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-18 09:29:18.189442 Pseudovisium-0.0.2/Pseudovisium.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-18 09:29:18.000000 Pseudovisium-0.0.2/Pseudovisium.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-18 09:29:18.000000 Pseudovisium-0.0.2/Pseudovisium.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-18 09:29:18.000000 Pseudovisium-0.0.2/Pseudovisium.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-18 09:29:18.000000 Pseudovisium-0.0.2/Pseudovisium.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-18 09:29:18.000000 Pseudovisium-0.0.2/Pseudovisium.egg-info/top_level.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       14 2024-04-08 13:33:17.000000 Pseudovisium-0.0.2/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-18 09:29:18.190124 Pseudovisium-0.0.2/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-18 09:29:08.000000 Pseudovisium-0.0.2/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.308315 Pseudovisium-0.0.3/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.3/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-23 09:38:37.308100 Pseudovisium-0.0.3/PKG-INFO
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.306480 Pseudovisium-0.0.3/Pseudovisium/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.3/Pseudovisium/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    59722 2024-04-22 10:42:50.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_generate.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    14626 2024-04-16 20:47:21.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_merge.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    58609 2024-04-23 09:35:07.000000 Pseudovisium-0.0.3/Pseudovisium/pseudovisium_qc.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-23 09:38:37.307826 Pseudovisium-0.0.3/Pseudovisium.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-23 09:38:37.000000 Pseudovisium-0.0.3/Pseudovisium.egg-info/top_level.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)     3058 2024-04-23 09:35:49.000000 Pseudovisium-0.0.3/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-23 09:38:37.308377 Pseudovisium-0.0.3/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-23 09:38:13.000000 Pseudovisium-0.0.3/setup.py
```

### Comparing `Pseudovisium-0.0.2/LICENSE` & `Pseudovisium-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.2/PKG-INFO` & `Pseudovisium-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.2/Pseudovisium/pseudovisium_generate.py` & `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,38 @@
         tuple: A tuple containing the temporary directory path and the total number of batches created.
 
     """
 
 
     tmp_dir = tempfile.mkdtemp(prefix="tmp_hexa")
     print(f"Created temporary directory {tmp_dir}")
+    #if csv_file is .gz, then open it with gzip
+    if csv_file.endswith('.gz'):
+        with gzip.open(csv_file, 'rt') as file:
+            reader = csv.DictReader(file)
+            header = next(reader)  # Read the header row
+            batch_num = 0
+
+            while True:
+                batch = list(itertools.islice(reader, batch_size))
+                if not batch:
+                    break  # Exit the loop if batch is empty
+
+                batch_file = os.path.join(tmp_dir, f"batch_{batch_num}.csv")
+                with open(batch_file, 'w', newline='') as batch_csv:
+                    writer = csv.writer(batch_csv)
+                    writer.writerow(fieldnames)  # Write header using the provided fieldnames
+                    writer.writerows([[row[field] for field in fieldnames] for row in batch])  # Write rows
+
+                batch_num += 1
+                print(f"Created batch {batch_num}")
+
+        print(f"Finished preprocessing. Total batches created: {batch_num}")
+        return tmp_dir, batch_num
+
 
     with open(csv_file, 'r') as file:
         reader = csv.DictReader(file)
         header = next(reader)  # Read the header row
         batch_num = 0
 
         while True:
@@ -704,17 +728,22 @@
     #get all unique feature_names
     features = list(set(feature for hexagon_counts in hexagon_counts.values() for feature in hexagon_counts))
 
     # Create a list of rows with repeated features and 'Gene Expression' column
     rows = [[feature, feature, 'Gene Expression'] for feature in features]
 
     print("Creating features.tsv.gz file in spatial folder.")
-    with gzip.open(folderpath + '/features.tsv.gz', 'wt', newline='') as f_out:
+    with open(folderpath + '/features.tsv', 'wt', newline='', encoding='utf-8') as f_out:
         writer = csv.writer(f_out, delimiter='\t')
         writer.writerows(rows)
+    
+    # Create a features.tsv.gz file
+    with open(folderpath + '/features.tsv', 'rb') as f_in, gzip.open(folderpath + '/features.tsv.gz', 'wb') as f_out:
+        f_out.writelines(f_in)
+        
 
  ############################################## ##############################################
     
 
     print("Putting together the matrix.mtx file")
     matrix_data = []
     batch_size_n_hexagons = 500
```

### Comparing `Pseudovisium-0.0.2/Pseudovisium/pseudovisium_merge.py` & `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_merge.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.2/Pseudovisium/pseudovisium_qc.py` & `Pseudovisium-0.0.3/Pseudovisium/pseudovisium_qc.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,29 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 from io import BytesIO
 import base64
 import scipy.stats as stats
 from concurrent.futures import ProcessPoolExecutor
 from tqdm import tqdm
+import os
+import datetime
+import matplotlib.pyplot as plt
+from matplotlib.collections import PathCollection
+from adjustText import adjust_text
+from io import BytesIO
+import base64
 
 
+def generate_qc_report(folders, output_folder="/Users/k23030440/", gene_names=["RYR3", "AQP4", "THBS1"], include_morans_i=False,max_workers=4):
+    #if any entry in folders lacks final /, then add
+    folders = [folder if folder[-1]=="/" else folder + "/" for folder in folders]
+    #same with output_folder
+    output_folder = output_folder if output_folder[-1]=="/" else output_folder + "/"
 
-def generate_qc_report(folders, output_folder="/Users/k23030440/", gene_names=["RYR3", "AQP4", "THBS1"], include_morans_i=False):
     replicates_data = []
     for folder in folders:
         # Extract the dataset name from the folder path
         dataset_name = folder.split("/")[-2]
 
         # Load files
         tissue_positions_list = pd.read_csv(folder + "spatial/tissue_positions_list.csv", header=None)
@@ -35,64 +46,67 @@
         features.columns = ["Gene_ID", "Gene_Name", "Type"]
         features["index_col"] = features.index + 1
         barcodes = pd.read_csv(folder + "barcodes.tsv", header=None, sep="\t")
         barcodes.columns = ["Barcode_ID"]
         barcodes["index_col"] = barcodes.index + 1
 
         arguments = json.load(open(folder + "arguments.json"))
-
-        "count_colname": "NA", "smoothing": 0.0, "quality_per_hexagon": true, "quality_per_probe": true,
         #if cell_id_colname is not NA, then we have cell info
         cell_info= True if arguments["cell_id_colname"]!="NA" else False
         quality_per_hexagon = arguments["quality_per_hexagon"]
         quality_per_probe = arguments["quality_per_probe"]
 
         if quality_per_hexagon:
             hexagon_quality = pd.read_csv(folder + "spatial/quality_per_hexagon.csv", header=None)
             #name cols as barcode, quality, count
             hexagon_quality.columns = ["Hexagon_ID", "Quality", "Count"]
-            #add 1
-            hexagon_quality["Hexagon_ID"] = hexagon_quality["Hexagon_ID"] + 1
             #add dataset name
             hexagon_quality["Dataset"] = dataset_name
             hexagons_above_100 = hexagon_quality[hexagon_quality["Count"]>100]
             hexagons_q_below_20 = hexagons_above_100[hexagons_above_100["Quality"]<20]
             pct_hexagons_q_below_20 = len(hexagons_q_below_20)/len(hexagons_above_100)
+            
 
         if quality_per_probe:
             probe_quality = pd.read_csv(folder + "spatial/quality_per_probe.csv", header=None)
             #name cols as barcode, quality, count
-            probe_quality.columns = ["Probe_name", "Quality", "Count"]
+            probe_quality.columns = ["Probe_ID", "Quality", "Count"]
             probe_quality["Dataset"] = dataset_name
-            non_ctrl_probes = probe_quality[~probe_quality["Probe_name"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
+            non_ctrl_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")]
             non_ctrl_probes_q_below_20 = non_ctrl_probes[non_ctrl_probes["Quality"]<20]
             pct_non_ctrl_probes_q_below_20 = len(non_ctrl_probes_q_below_20)/len(non_ctrl_probes)
             
         
         if cell_info:
             pv_cell_hex = pd.read_csv(folder + "spatial/pv_cell_hex.csv", header=None)
             pv_cell_hex.columns = ["Cell_ID", "Hexagon_ID", "Count"]
             pv_cell_hex["Hexagon_ID"] = pv_cell_hex["Hexagon_ID"] + 1
 
 
 
+
         arguments = json.load(open(folder + "arguments.json"))
         hexagon_size = arguments["hexagon_size"]
         image_pixels_per_um = arguments["image_pixels_per_um"]
 
         tissue_positions_list = tissue_positions_list[tissue_positions_list["in_tissue"] == 1]
         tissue_positions_list["barcode_id"] = [barcodes[barcodes["Barcode_ID"] == barcode].index_col.values[0] for barcode in tissue_positions_list["barcode"]]
         in_tissue_barcodes = tissue_positions_list["barcode"].index + 1
 
         n_barcodes_per_tissue = len(tissue_positions_list)
 
         # Join the x and y columns from tissue_positions_list based on Barcode_ID and barcode_id
         matrix_joined = pd.merge(matrix, tissue_positions_list[["barcode_id", "x", "y"]], left_on="Barcode_ID", right_on="barcode_id")
         matrix_joined = pd.merge(matrix_joined, features[["Gene_ID", "index_col"]], left_on="Gene_ID", right_on="index_col")
 
+        if quality_per_hexagon:
+            #in hexagon_quality keep only rows where hexagon_id is in index_col
+            hexagon_quality = hexagon_quality[hexagon_quality["Hexagon_ID"].isin(matrix_joined["barcode_id"])]
+            matrix_joined = pd.merge(matrix_joined, hexagon_quality, left_on="barcode_id", right_on="Hexagon_ID")
+
         # Calculate key metrics
         grouped_matrix = matrix_joined.groupby("Barcode_ID")["Counts"].sum()
         number_of_hex_above_100 = np.sum(grouped_matrix > 50)
 
         grouped_matrix = matrix_joined.groupby("Gene_ID_y")["Barcode_ID"].count()
         pct5_plex = np.sum(grouped_matrix > 0.05 * n_barcodes_per_tissue)
         probe_names = grouped_matrix[grouped_matrix > 0.05 * n_barcodes_per_tissue].index.values
@@ -101,89 +115,158 @@
         median_counts = np.median(grouped_matrix)
         cv_counts = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
         grouped_matrix = matrix_joined.groupby("Barcode_ID")["Gene_ID_y"].count()
         median_features = np.median(grouped_matrix)
         cv_features = np.std(grouped_matrix) / np.mean(grouped_matrix)
 
-        number_of_genes = len(features[~features["Gene_ID"].str.contains("control|blank|Control|Blank|BLANK")])
+        number_of_genes = len(features[~features["Gene_ID"].str.contains("control|ctrl|pos|neg|Ctrl|blank|Control|Blank|BLANK")])
 
         neg_control_probes = features[features["Gene_ID"].str.contains("Probe")].index + 1
         neg_control_counts = np.sum(matrix[matrix["Gene_ID"].isin(neg_control_probes)]["Counts"])
         total_counts = np.sum(matrix["Counts"])
         prop_neg_control = neg_control_counts / total_counts
         if cell_info:
-            pv_cell_hex_assigned = pv_cell_hex[pv_cell_hex["Cell_ID"] != "UNASSIGNED"]
+            pv_cell_hex_assigned = pv_cell_hex[(pv_cell_hex["Cell_ID"] != "UNASSIGNED") & (pv_cell_hex["Cell_ID"] != -1)]
             grouped_pv_cell_hex_assigned = pv_cell_hex_assigned.groupby("Hexagon_ID")["Cell_ID"].count()
             median_cells_per_hex = np.median(grouped_pv_cell_hex_assigned)
 
             counts_per_cell = pv_cell_hex_assigned.groupby("Cell_ID")["Count"].sum()
             median_counts_per_cell = np.median(counts_per_cell)
 
+            pv_cell_hex_unassigned = pv_cell_hex[(pv_cell_hex["Cell_ID"] != "UNASSIGNED") | (pv_cell_hex["Cell_ID"] != -1)]
+            #merge with grouped_pv_cell_hex_assigned
+            grouped_pv_cell_hex_assigned_sum = pv_cell_hex_assigned.groupby("Hexagon_ID")["Count"].sum()
+            merged_assigned_unassigned = pd.merge(grouped_pv_cell_hex_assigned_sum,pv_cell_hex_unassigned,left_on="Hexagon_ID",right_on="Hexagon_ID",how="inner")
+            merged_assigned_unassigned = merged_assigned_unassigned.rename(columns={"Count_x":"Assigned_count","Count_y":"Unassigned_count"})
+            merged_assigned_unassigned = merged_assigned_unassigned.fillna(0)
+            #add pct_unassigned
+            merged_assigned_unassigned["pct_unassigned"] = merged_assigned_unassigned["Unassigned_count"]/(merged_assigned_unassigned["Assigned_count"]+merged_assigned_unassigned["Unassigned_count"])
+            #merge with matrix
+            merged_assigned_unassigned = pd.merge(merged_assigned_unassigned,tissue_positions_list,left_on="Hexagon_ID",right_on="barcode_id",how="inner",suffixes=('_a', '_b'))
+            median_unassigned_pct = np.median(merged_assigned_unassigned["pct_unassigned"])
+
+
+            # merge tissue_positions_list with pv_cell_hex
+            tissue_positions_pv_cell_hex = pd.merge(tissue_positions_list, pv_cell_hex, left_on="barcode_id", right_on="Hexagon_ID", how="inner")
+            #sum up the number of Cell_ID in every Hexagon_ID but keep x and y intact
+            tissue_positions_pv_cell_hex_sum = tissue_positions_pv_cell_hex.groupby(["x","y"]).agg({"Cell_ID":"count","Hexagon_ID":"first"}).reset_index()
+            #remove multi level index
+            tissue_positions_pv_cell_hex_sum.reset_index(inplace=True)
+            #rename Cell_ID to count
+            tissue_positions_pv_cell_hex_sum.rename(columns={"Cell_ID":"counts"},inplace=True)
+            density_cv = np.std(tissue_positions_pv_cell_hex_sum["counts"])/np.mean(tissue_positions_pv_cell_hex_sum["counts"])
+            density_morans_i = get_morans_i("density", tissue_positions_pv_cell_hex_sum, tissue_positions_list,max_workers=max_workers) 
+            
+
+
+
+
         plot_df = not_working_probe_based_on_sum(matrix_joined, sample_id=dataset_name)
         not_working_probes = plot_df[plot_df["Probe category"]=="Bad"].index.values
         n_probes_not_working = len(not_working_probes)
         
         
 
         replicate_data = {
             "dataset_name": dataset_name,
             "metrics_table_data": {
                 "Number of hexagons with at least 100 counts": int(number_of_hex_above_100),
                 "Number of genes in at least 5% of hexagons": int(pct5_plex),
                 "Median counts per hexagon": int(median_counts),
                 "Median features per hexagon": int(median_features),
                 "Number of genes": int(number_of_genes),
-                "Proportion of neg_control probes": prop_neg_control,
+                "Proportion of neg_control probes": np.round(prop_neg_control, 3),
                 "Number of bad probes (Sum)": n_probes_not_working,
                 "Features CV": np.round(cv_features, 3),
                 "Counts CV": np.round(cv_counts, 3),
-                "Features Morans I": np.round(get_morans_i("features", matrix_joined, tissue_positions_list),3),
-                "Counts Morans I": np.round(get_morans_i("counts", matrix_joined, tissue_positions_list),3)
+                "Features Morans I": np.round(get_morans_i("features", matrix_joined, tissue_positions_list,max_workers=max_workers),3),
+                "Counts Morans I": np.round(get_morans_i("counts", matrix_joined, tissue_positions_list,max_workers=max_workers),3)
             },
             "matrix_joined": matrix_joined,
             "features": features,
             "tissue_positions_list": tissue_positions_list,
             "hexagon_size": hexagon_size,
             "image_pixels_per_um": image_pixels_per_um,
             "barcodes": barcodes,
             "probe_sum_stripplot_df":plot_df
         }
 
         if include_morans_i:
-            replicate_data["morans_i"] = get_morans_i("all", matrix_joined, tissue_positions_list)
+            replicate_data["morans_i"] = get_morans_i("all", matrix_joined, tissue_positions_list,max_workers=max_workers)
             plot_df_morans_i = not_working_probe_based_on_morans_i(replicate_data["morans_i"], sample_id=dataset_name)
             not_working_probes = plot_df_morans_i[plot_df_morans_i["Probe category"]=="Bad"].index.values
             n_probes_not_working = len(not_working_probes)
             #add to replicate_data metrics_table_data
             replicate_data["metrics_table_data"]["Number of bad probes (Morans I)"] = n_probes_not_working
             replicate_data["morans_i_stripplot_df"] = plot_df_morans_i
 
         if cell_info:
             replicate_data["metrics_table_data"]["Median cells per hexagon"] = int(median_cells_per_hex)
             replicate_data["metrics_table_data"]["Median counts per cell"] = int(median_counts_per_cell)
+            replicate_data["metrics_table_data"]["Median pct unassigned"] = np.round(median_unassigned_pct, 3)
+            replicate_data["merged_assigned_unassigned"] = merged_assigned_unassigned
+            replicate_data["cell_density_df"] = tissue_positions_pv_cell_hex_sum
+
+            replicate_data["metrics_table_data"]["Density CV"] = np.round(density_cv, 3)
+            replicate_data["metrics_table_data"]["Density Morans I"] = np.round(density_morans_i, 3)
 
         if quality_per_hexagon:
             replicate_data["metrics_table_data"]["Pct hexagons with quality below 20"] = np.round(pct_hexagons_q_below_20, 3)
             replicate_data["hexagon_quality"] = hexagon_quality
+            replicate_data["metrics_table_data"]["Quality Morans I"] = np.round(get_morans_i("Quality", matrix_joined, tissue_positions_list,max_workers=max_workers),3)
+
+
         if quality_per_probe:
             replicate_data["metrics_table_data"]["Pct non-ctrl probes with quality below 20"] = np.round(pct_non_ctrl_probes_q_below_20, 3)
             replicate_data["probe_quality"] = probe_quality
+            plot_df_quality_per_probe = not_working_probe_based_on_quality(probe_quality, sample_id=dataset_name)
+            replicate_data["probe_quality_stripplot_df"] = plot_df_quality_per_probe
 
         replicates_data.append(replicate_data)
 
-    html_code = generate_dashboard_html(replicates_data, gene_names, include_morans_i)
+    html_code = generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info)
 
     # Save HTML code to a file
     with open(output_folder + "metrics_dashboard.html", "w", encoding="utf-8") as html_file:
         html_file.write(html_code)
         print("HTML file generated successfully!")
+    
+    #in the same output folder generate a folder called pv_qc_ date
+    data_output_folder = output_folder + "pv_qc_" + str(datetime.datetime.now().date())
+    #if that dir exists_ add a number to the end
+    i=1
+    while os.path.exists(data_output_folder):
+        data_output_folder = output_folder + "pv_qc_" + str(datetime.datetime.now().date()) + "_" + str(i)
+        i+=1
+    os.mkdir(data_output_folder)
+
+    #save the metrics table as a csv
+    metrics_table = pd.DataFrame([replicate_data["metrics_table_data"] for replicate_data in replicates_data])
+    #add a column for the dataset name
+    metrics_table["Dataset"] = [replicate_data["dataset_name"] for replicate_data in replicates_data]
+    metrics_table.to_csv(data_output_folder + "/metrics_table.csv", index=False)
+
+    #save probe_quality as a csv
+    if quality_per_probe:
+        probe_quality = pd.concat([replicate_data["probe_quality_stripplot_df"] for replicate_data in replicates_data])
+        probe_quality.to_csv(data_output_folder + "/probe_quality.csv", index=False)
+
+    #save morans i values for each gene
+    if include_morans_i:
+        morans_i = pd.concat([replicate_data["morans_i_stripplot_df"] for replicate_data in replicates_data])
+        morans_i.to_csv(data_output_folder + "/morans_i.csv", index=False)
+
+    #save sum of probes stripplot
+    sum_stripplot = pd.concat([replicate_data["probe_sum_stripplot_df"] for replicate_data in replicates_data])
+    sum_stripplot.to_csv(data_output_folder + "/sum_stripplot.csv", index=False)
+
 
 
-def generate_dashboard_html(replicates_data, gene_names, include_morans_i):
+def generate_dashboard_html(replicates_data, gene_names, include_morans_i,quality_per_hexagon,quality_per_probe,cell_info):
     metrics_html = """
         <div id="metric-details">
             <table>
                 <thead>
                     <tr>
                         <th>Metric</th>
     """
@@ -264,22 +347,67 @@
         </div>
         """
         if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
             nfeature_hexagon_plots_html += """
             </div>
             """
 
+    if cell_info:
+        cell_density_hexagon_plots_html = ""
+        for i, replicate_data in enumerate(replicates_data):
+            if i % 3 == 0:
+                cell_density_hexagon_plots_html += f"""
+                <div class="row">
+                """
+            cell_density_df= replicate_data["cell_density_df"]
+            hexagon_html = hexagon_plot_to_html(cell_density_df, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "Density", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Density Morans I"])
+            cell_density_hexagon_plots_html += f"""
+            <div class="col">
+                <h3>{replicate_data['dataset_name']}</h3>
+                {hexagon_html}
+            </div>
+            """
+            if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
+                cell_density_hexagon_plots_html += """
+                </div>
+                """
+
+
+
+
+    if quality_per_hexagon:
+        quality_hexagon_plots_html = ""
+        for i, replicate_data in enumerate(replicates_data):
+            if i % 3 == 0:
+                quality_hexagon_plots_html += f"""
+                <div class="row">
+                """
+            hexagon_quality = get_quality_per_hexagon(replicate_data['matrix_joined'])
+            hexagon_html = hexagon_plot_to_html(hexagon_quality, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "Quality", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Quality Morans I"])
+            quality_hexagon_plots_html += f"""
+            <div class="col">
+                <h3>{replicate_data['dataset_name']}</h3>
+                {hexagon_html}
+            </div>
+            """
+            if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
+                quality_hexagon_plots_html += """
+                </div>
+                """
+
+                
+
     total_hexagon_plots_html = ""
     for i, replicate_data in enumerate(replicates_data):
         if i % 3 == 0:
             total_hexagon_plots_html += f"""
             <div class="row">
             """
         total_counts_per_hexagon = get_total_counts_per_hexagon(replicate_data['matrix_joined'])
-        hexagon_html = hexagon_plot_to_html(total_counts_per_hexagon, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "nFeature", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Counts Morans I"])
+        hexagon_html = hexagon_plot_to_html(total_counts_per_hexagon, replicate_data['hexagon_size'], replicate_data['image_pixels_per_um'], "Total exp", replicate_data['dataset_name'],replicate_data['metrics_table_data']["Counts Morans I"])
         total_hexagon_plots_html += f"""
         <div class="col">
             <h3>{replicate_data['dataset_name']}</h3>
             {hexagon_html}
         </div>
         """
         if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
@@ -365,14 +493,32 @@
         </div>
         """
         if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
             sums_i_stripplot_html += """
             </div>
             """
 
+    quality_stripplot_html = ""
+    if quality_per_probe:
+        for i, replicate_data in enumerate(replicates_data):
+            if i % 3 == 0:
+                quality_stripplot_html += f"""
+                <div class="row">
+                """
+            plot_df = replicate_data['probe_quality_stripplot_df']
+            quality_stripplot_html += f"""
+            <div class="col">
+                <h3>{replicate_data['dataset_name']}</h3>
+                {probe_stripplot(plot_df, sample_id=replicate_data['dataset_name'],legend=True, col_to_plot="Quality")}
+            </div>
+            """
+            if (i + 1) % 3 == 0 or i == len(replicates_data) - 1:
+                quality_stripplot_html += """
+                </div>
+                """
 
     html_code = f"""
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
@@ -420,16 +566,19 @@
                     <option value="plot">Hexagon Plots</option>
                     <option value="sums-comparison">Sums Comparison</option>
                     <option value="abundance-correlation-heatmap">Abundance Correlation Heatmap</option>
                     {'<option value="morans-i-heatmap">Morans I Heatmap</option>' if include_morans_i else ""}
                     {'<option value="morans-i-stripplot">Morans I Stripplot</option>' if include_morans_i else ""}
                     <option value="sums-i-stripplot">Sums I Stripplot</option>
                     <option value="nfeature_hexagon_plots">nFeature hexagon plots</option>
+                    {'<option value="quality_hexagon_plots">Quality hexagon plots</option>' if quality_per_hexagon else ""}
                     <option value="total_hexagon_plots">Total hexagon plots</option>
                     {'<option value="morans-i-comparison">Pairwise Morans I Plots</option>' if include_morans_i else ""}
+                    {'<option value="probe_quality_stripplot">Probe Quality Stripplot</option>' if quality_per_probe else ""}
+                    {'<option value="cell_density_hexagon_plots">Cell Density Hexagon Plots</option>' if cell_info else ""}
                 </select>
             </div>
             <div id="metric-details-container">
                 {metrics_html}
             </div>
             <div id="plot" class="plot-container">
                 {hexagon_plots_html}
@@ -448,34 +597,46 @@
             </div>
             <div id="sums-i-stripplot" class="plot-container">
                 {sums_i_stripplot_html}
             </div>
             <div id="nfeature_hexagon_plots" class="plot-container">
                 {nfeature_hexagon_plots_html}
             </div>
+            <div id="quality_hexagon_plots" class="plot-container">
+                {quality_hexagon_plots_html}
+            </div>
             <div id="total_hexagon_plots" class="plot-container">
                 {total_hexagon_plots_html}
             </div>
             <div id="morans-i-comparison" class="plot-container">
                 {morans_i_comparison_html}
             </div>
+            <div id="probe_quality_stripplot" class="plot-container">
+                {quality_stripplot_html}
+            </div>
+            <div id="cell_density_hexagon_plots" class="plot-container">
+                {cell_density_hexagon_plots_html}
+            </div>
         </div>
 
         <script>
             const select = document.getElementById('metrics-select');
             const metricDetailsContainer = document.getElementById('metric-details-container');
             const plotContainer = document.getElementById('plot');
             const sumsComparisonContainer = document.getElementById('sums-comparison');
             const abundanceCorrelationHeatmapContainer = document.getElementById('abundance-correlation-heatmap');
             const moransIHeatmapContainer = document.getElementById('morans-i-heatmap');
             const moransIStripplotContainer = document.getElementById('morans-i-stripplot');
             const sumsIStripplotContainer = document.getElementById('sums-i-stripplot');
             const nfeatureHexagonContainer = document.getElementById('nfeature_hexagon_plots');
+            const qualityHexagonContainer = document.getElementById('quality_hexagon_plots');
             const totalHexagonContainer = document.getElementById('total_hexagon_plots');
             const moransIComparisonContainer = document.getElementById('morans-i-comparison');
+            const probeQualityStripplotContainer = document.getElementById('probe_quality_stripplot');
+            const cellDensityHexagonContainer = document.getElementById('cell_density_hexagon_plots');
 
 
             function updateMetricDetails() {{
                 const selectedMetric = select.value;
                 const plotContainers = document.querySelectorAll('.plot-container');
 
                 // Hide all plot containers
@@ -498,19 +659,28 @@
                     moransIHeatmapContainer.style.display = 'block';
                 }} else if (selectedMetric === 'morans-i-stripplot') {{
                     moransIStripplotContainer.style.display = 'block';
                 }} else if (selectedMetric === 'sums-i-stripplot') {{
                     sumsIStripplotContainer.style.display = 'block';
                 }} else if (selectedMetric === 'nfeature_hexagon_plots') {{
                     nfeatureHexagonContainer.style.display = 'block';
+                }} else if (selectedMetric === 'quality_hexagon_plots') {{
+                    qualityHexagonContainer.style.display = 'block';
                 }} else if (selectedMetric === 'total_hexagon_plots') {{
                     totalHexagonContainer.style.display = 'block';
                 }} else if (selectedMetric === 'morans-i-comparison') {{
                     moransIComparisonContainer.style.display = 'block';
                 }}
+                else if (selectedMetric === 'probe_quality_stripplot') {{
+                    probeQualityStripplotContainer.style.display = 'block';
+                }}
+                else if (selectedMetric === 'cell_density_hexagon_plots') {{
+                    cellDensityHexagonContainer.style.display = 'block';
+                }}
+
             }}
 
             select.addEventListener('change', updateMetricDetails);
 
             // Initial update
             updateMetricDetails();
         </script>
@@ -548,38 +718,107 @@
     plot_df["Sample"] = sample_id
     #order based on probe category
     plot_df = plot_df.sort_values("Probe category")
     return plot_df
 
 
 
+import numpy as np
+import matplotlib.pyplot as plt
+from adjustText import adjust_text
+from io import BytesIO
+import base64
+
+
 def probe_stripplot(plot_df, col_to_plot="log_counts", sample_id="Sample 1", legend=False):
-    stripplot = sns.stripplot(data=plot_df, x="Sample", y=col_to_plot, hue="Probe category", jitter=True, alpha=0.5, size=5)
-    # Remove x axis label
-    stripplot.set(xlabel="")
-    # Add a legend
-    if legend:
-        stripplot.legend(loc='upper left')
-    else:
-        stripplot.legend().remove()
+    fig, ax = plt.subplots(figsize=(2, 2.5))
+    # Define jitter amount
+    jitter = 0.1
+
+    # Create a dictionary to store x and y values for each point
+    points = {"x": [], "y": [], "cat": [], "index": []}
+
+    # Assign x and y values with jitter for each point
+    for index, row in plot_df.iterrows():
+        cat = row["Probe category"]
+        x = 0 + np.random.uniform(-jitter, jitter)
+        y = row[col_to_plot]
+        points["x"].append(x)
+        points["y"].append(y)
+        points["cat"].append(cat)
+        points["index"].append(index)
+
+    # Plot the points for each category
+    for cat in ["Neg_control", "Good", "Bad"]:
+        mask = [c == cat for c in points["cat"]]
+        ax.scatter([x for x, m in zip(points["x"], mask) if m],
+                   [y for y, m in zip(points["y"], mask) if m],
+                   alpha=0.8, label=cat)
+
     # Draw a straight line at the mean of the neg controls
-    stripplot.axhline(np.mean(plot_df[plot_df["Probe category"] == "Neg_control"][col_to_plot]), color="red")
+    neg_control_mean = np.mean(plot_df[plot_df["Probe category"] == "Neg_control"][col_to_plot])
+    ax.axhline(neg_control_mean, color="red", linestyle="--")
+
+    # Add labels for the top 10 lowest score Bad probes
+    bad_probes = plot_df[plot_df["Probe category"] == "Bad"].sort_values(col_to_plot).head(10)
+    colname = "gene" if "gene" in plot_df.columns else "Probe_ID"
+
+    texts = []
+    for index, row in bad_probes.iterrows():
+        x = points["x"][points["index"].index(index)]
+        y = points["y"][points["index"].index(index)]
+        txt = row[colname]
+        texts.append(ax.text(x, y, txt, fontsize=8, ha='left', va='center'))
 
-    plt.gcf().set_size_inches(3, 2.5)
+    adjust_text(texts, arrowprops=dict(arrowstyle="-", color='black', lw=0.5))
+
+    # Remove x-axis ticks and label
+    ax.set_xticks([])
+    ax.set_xlabel("")
+    #add y label based on col_to_plot
+    ax.set_ylabel(col_to_plot)
+
+    # Add a legend if requested
+    if legend:
+        ax.legend(fontsize='small', loc='upper left', bbox_to_anchor=(1, 1))
 
     # Convert the plot to HTML
     img_buffer = BytesIO()
-    # Use stripplot.figure to access the figure object
-    stripplot.figure.savefig(img_buffer, format='png')
+    fig.savefig(img_buffer, format='png', bbox_inches='tight')
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
     html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
 
-    plt.close(stripplot.figure)
+    plt.close(fig)
     return html_fig
 
+def not_working_probe_based_on_quality(probe_quality, sample_id="Sample1"):
+    probe_quality_neg_probes = probe_quality[probe_quality["Probe_ID"].str.contains("control|blank|Control|Blank|BLANK")]
+    probe_quality_true_probes = probe_quality[~probe_quality["Probe_ID"].str.contains("control|blank|Control|Blank|BLANK")]
+    plot_df = probe_quality.reset_index(drop=True)
+    plot_df["Probe category"] = [1 if gene in probe_quality_neg_probes.Probe_ID.values else 0 for gene in plot_df.Probe_ID.values]
+
+    #iterate through the true probes and see whether they are significantly outside of the distribution of the neg probes
+    for gene in probe_quality_true_probes.Probe_ID.values:
+        plot_df_gene_index = plot_df[plot_df["Probe_ID"]==gene].index[0]
+        quality = plot_df[plot_df["Probe_ID"]==gene]["Quality"]
+        neg_probes_quality = plot_df[plot_df["Probe category"]==1]["Quality"]
+        mean = np.mean(neg_probes_quality)
+        std = np.std(neg_probes_quality)
+        p_val = stats.norm.cdf(quality, loc=mean, scale=std)
+        p_val = 1-p_val
+        if p_val*len(probe_quality_true_probes)<0.05:
+            plot_df.loc[plot_df_gene_index,"Probe category"] = 2
+        
+    plot_df["Probe category"] = ["Neg_control" if x==1 else "Bad" if x==0 else "Good" for x in plot_df["Probe category"]]
+    plot_df["Sample"] = sample_id
+    plot_df = plot_df.sort_values("Probe category")
+    return plot_df
+
+
+
 
 def not_working_probe_based_on_morans_i(morans_table, sample_id="Sample1"):
     morans_table_neg_probes = morans_table[morans_table.gene.str.contains("control|blank|Control|Blank|BLANK")]
     morans_table_true_probes = morans_table[~morans_table.gene.str.contains("control|blank|Control|Blank|BLANK")]     
 
     #create a plot_df that is grouped_matrix and a column specifying whether the gene is a neg control or not
     plot_df = morans_table.reset_index(drop=True)
@@ -611,14 +850,28 @@
 
 
 def get_total_counts_per_hexagon(matrix_joined):
     total_counts_per_hexagon = matrix_joined.groupby(['x', 'y'])['Counts'].sum().reset_index()
     total_counts_per_hexagon = total_counts_per_hexagon.rename(columns={"Counts": "counts"})
     return total_counts_per_hexagon
 
+def get_quality_per_hexagon(matrix_joined):
+    hexagon_quality = matrix_joined.groupby("Barcode_ID").agg({"Quality":"first","x":"first","y":"first"})
+    hexagon_quality = hexagon_quality.reset_index()
+    #rename Quality to counts
+    hexagon_quality = hexagon_quality.rename(columns={"Quality": "counts"})
+    return hexagon_quality
+
+
+from shapely.geometry import Point
+import geopandas as gpd
+from libpysal import weights
+from esda import Moran
+import numpy as np
+import pandas as pd
 
 # Functions used in generate_qc_report
 def get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=False):
     matrix_subset = matrix_joined[matrix_joined["Gene_ID_y"] == gene_name]
     matrix_subset.reset_index(drop=True, inplace=True)
     x = tissue_positions_list["x"]
     y = tissue_positions_list["y"]
@@ -705,27 +958,36 @@
         # Reorder
         sums1 = sums1.sort_values("Gene_ID_y")
         sums2 = sums2.sort_values("Gene_ID_y")
 
         sums_df = pd.merge(sums1, sums2, on="Gene_ID_y", suffixes=("_1", "_2"))
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.scatter(sums_df["Counts_1"], sums_df["Counts_2"], alpha=0.3, s=20)
-        ax.set_xlabel(f"Log10 Total expression {dataset1_name}", fontsize=12)
-        ax.set_ylabel(f"Log10 Total expression {dataset2_name}", fontsize=12)
-        ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=14)
+        ax.set_xlabel(f"Log10 Total expression {dataset1_name}", fontsize=8)
+        ax.set_ylabel(f"Log10 Total expression {dataset2_name}", fontsize=8)
+        ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=10)
         corr = sums_df["Counts_1"].corr(sums_df["Counts_2"])
-        ax.text(np.median(sums_df["Counts_1"]), np.quantile(sums_df["Counts_2"], 0.95), f"Pearson correlation: {corr:.2f}", fontsize=10)
+        ax.text(np.quantile(sums_df["Counts_1"], 0.3), np.quantile(sums_df["Counts_2"], 0.95),
+                f"Pearson correlation: {corr:.2f}", fontsize=8)
+
         sums_df["diff"] = np.abs(sums_df["Counts_1"] - sums_df["Counts_2"])
         sums_df = sums_df.sort_values("diff", ascending=False)
+
+        texts = []
         for i in range(10):
-            ax.text(sums_df["Counts_1"].iloc[i], sums_df["Counts_2"].iloc[i], sums_df["Gene_ID_y"].iloc[i], fontsize=10)
+            x = sums_df["Counts_1"].iloc[i]
+            y = sums_df["Counts_2"].iloc[i]
+            txt = sums_df["Gene_ID_y"].iloc[i]
+            texts.append(ax.text(x, y, txt, fontsize=10))
+
+        adjust_text(texts, arrowprops=dict(arrowstyle="-", color='black', lw=0.5))
 
         # Convert the plot to HTML
         img_buffer = BytesIO()
-        fig.savefig(img_buffer, format='png')
+        fig.savefig(img_buffer, format='png', bbox_inches='tight')
         img_str = base64.b64encode(img_buffer.getvalue()).decode()
         html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
 
         plt.close(fig)  # Close the plot to free memory
 
         return html_fig
 
@@ -757,36 +1019,58 @@
                 corr_matrix.iloc[j, i] = corr
             else:
                 corr_matrix.iloc[i, j] = 0.0
                 corr_matrix.iloc[j, i] = 0.0
             
     #make diagonal 1
     np.fill_diagonal(corr_matrix.values, 1)
-    print(corr_matrix)
-    fig_dimension = len(replicates_data) * 0.5
+    
+    fig_dimension = len(replicates_data)
 
     clustermap = sns.clustermap(corr_matrix, cmap='coolwarm', annot=True, fmt='.2f', figsize=(fig_dimension, fig_dimension))
 
     # Convert the plot to HTML
     img_buffer = BytesIO()
     clustermap.savefig(img_buffer, format='png')
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
     html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
 
     plt.close(clustermap.figure)
     return html_fig
 
 
+def get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=False):
+    matrix_subset = matrix_joined[matrix_joined["Gene_ID_y"] == gene_name]
+    matrix_subset.reset_index(drop=True, inplace=True)
+    x = tissue_positions_list["x"]
+    y = tissue_positions_list["y"]
+    counts = np.zeros(len(tissue_positions_list))
+    for i in range(len(matrix_subset)):
+        count = matrix_subset["Counts"][i]
+        barcode_id = matrix_subset["Barcode_ID"][i]
+        x_, y_ = matrix_subset["x"][i], matrix_subset["y"][i]
+        x = np.append(x, x_)
+        y = np.append(y, y_)
 
+        if normalised:
+            count = count / np.sum(matrix_joined[matrix_joined["Barcode_ID"] == barcode_id]["Counts"])
 
-# Importing process_gene from the specified file path /Users/k23030440/gene_processing.py
-#set the path to the file
-import sys
-sys.path.append("/Users/k23030440")
-from gene_processing import process_gene
+        counts = np.append(counts, count)
+    df = pd.DataFrame({"x": x, "y": y, "counts": counts})
+    return df.sort_values("counts", ascending=False).drop_duplicates(subset=["x", "y"])
+
+
+def process_gene(gene, matrix_joined, tissue_positions_list):
+    gene_df = get_df_for_gene(matrix_joined, tissue_positions_list, gene, normalised=True)
+    points = [Point(xy) for xy in zip(gene_df['x'], gene_df['y'])]
+    gene_gdf = gpd.GeoDataFrame(gene_df, geometry=points)
+    w = weights.KNN.from_dataframe(gene_gdf, k=6)
+    w.transform = 'R'
+    mi = Moran(gene_df["counts"], w, permutations=0)
+    return {"gene": gene, "Morans_I": mi.I}
 
 def get_morans_i(gene_name, matrix_joined, tissue_positions_list, max_workers=4):
     if gene_name == "all":
         unique_genes = matrix_joined["Gene_ID_y"].unique()
         #remove those unique genes which have less than total 100 counts
         lowly_expressed_genes = matrix_joined.groupby("Gene_ID_y")["Counts"].sum()
         lowly_expressed_genes = lowly_expressed_genes[lowly_expressed_genes<100].index.values
@@ -807,24 +1091,44 @@
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
         w = weights.KNN.from_dataframe(gene_gdf, k=6)
         w.transform = 'R'
         mi = esda.Moran(mat["Gene_ID_y"], w, permutations=0)
         return mi.I
     
+    elif gene_name == "density":
+        mat = matrix_joined.copy()
+        points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
+        gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
+        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w.transform = 'R'
+        mi = esda.Moran(mat["counts"], w, permutations=0)
+        return mi.I
+    
     elif gene_name == "counts":
         mat = matrix_joined.groupby("Barcode_ID").sum()
         mat["x"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["x"].values[0])
         mat["y"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["y"].values[0])
         points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
         gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
         w = weights.KNN.from_dataframe(gene_gdf, k=6)
         w.transform = 'R'
         mi = esda.Moran(mat["Counts"], w, permutations=0)
         return mi.I
+
+    elif gene_name == "Quality":
+        mat = matrix_joined.groupby("Barcode_ID").agg({"Quality":"mean"})
+        mat["x"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["x"].values[0])
+        mat["y"] = mat.index.to_series().apply(lambda barcode: matrix_joined[matrix_joined["Barcode_ID"]==barcode]["y"].values[0])
+        points = [Point(xy) for xy in zip(mat['x'], mat['y'])]
+        gene_gdf = gpd.GeoDataFrame(mat, geometry=points)
+        w = weights.KNN.from_dataframe(gene_gdf, k=6)
+        w.transform = 'R'
+        mi = esda.Moran(mat["Quality"], w, permutations=0)
+        return mi.I
     
     else:
         gene_df = get_df_for_gene(matrix_joined, tissue_positions_list, gene_name, normalised=True)
         points = [Point(xy) for xy in zip(gene_df['x'], gene_df['y'])]
         gene_gdf = gpd.GeoDataFrame(gene_df, geometry=points)
         w = weights.KNN.from_dataframe(gene_gdf, k=6)
         w.transform = 'R'
@@ -852,19 +1156,19 @@
 
         return html_fig
     else:
         morans_i_df = pd.merge(morans_i1, morans_i2, on="gene", suffixes=("_1", "_2"))
         morans_i_df = morans_i_df[morans_i_df["gene"].isin(common_probes)]
         fig, ax = plt.subplots(figsize=(4, 4))
         ax.scatter(morans_i_df["Morans_I_1"], morans_i_df["Morans_I_2"], alpha=0.3, s=20)
-        ax.set_xlabel(f"Moran's I {dataset1_name}", fontsize=12)
-        ax.set_ylabel(f"Moran's I {dataset2_name}", fontsize=12)
-        ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=14)
+        ax.set_xlabel(f"Moran's I {dataset1_name}", fontsize=8)
+        ax.set_ylabel(f"Moran's I {dataset2_name}", fontsize=8)
+        ax.set_title(f"{dataset1_name} vs {dataset2_name}", fontsize=10)
         corr = morans_i_df["Morans_I_1"].corr(morans_i_df["Morans_I_2"])
-        ax.text(0.5, 0.1, f"Pearson correlation: {corr:.2f}", fontsize=10, ha='center')
+        ax.text(0.5, 0.1, f"Pearson correlation: {corr:.2f}", fontsize=8, ha='center')
         morans_i_df["diff"] = np.abs(morans_i_df["Morans_I_1"] - morans_i_df["Morans_I_2"])
         morans_i_df = morans_i_df.sort_values("diff", ascending=False)
         for i in range(10):
             ax.text(morans_i_df["Morans_I_1"].iloc[i], morans_i_df["Morans_I_2"].iloc[i], morans_i_df["gene"].iloc[i], fontsize=10)
 
         # Convert the plot to HTML
         img_buffer = BytesIO()
@@ -903,15 +1207,15 @@
             else:
                 corr_matrix.iloc[i, j] = 0.0
                 corr_matrix.iloc[j, i] = 0.0
 
     #make diagonal 1
     np.fill_diagonal(corr_matrix.values, 1)
     print(corr_matrix)
-    fig_dimension = len(replicates_data) * 0.5
+    fig_dimension = len(replicates_data) 
     clustermap = sns.clustermap(corr_matrix, cmap='coolwarm', annot=True, fmt='.2f', figsize=(fig_dimension, fig_dimension))
 
     # Convert the plot to HTML
     img_buffer = BytesIO()
     clustermap.savefig(img_buffer, format='png')
     img_str = base64.b64encode(img_buffer.getvalue()).decode()
     html_fig = f'<img src="data:image/png;base64,{img_str}"/>'
@@ -923,14 +1227,15 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Generate QC report for Pseudovisium output.")
     parser.add_argument("--folders", "-f", nargs="+", help="List of folders containing Pseudovisium output", required=True)
     parser.add_argument("--output_folder", "-o", default="/Users/k23030440/", help="Output folder path")
     parser.add_argument("--gene_names", "-g", nargs="+", default=["RYR3", "AQP4", "THBS1"], help="List of gene names to plot")
     parser.add_argument("--include_morans_i", "-m", action="store_true", help="Include Moran's I features tab")
+    parser.add_argument("-max_workers", "--mw", type=int, default=4, help="Number of workers to use for parallel processing")
     args = parser.parse_args()
 
-    generate_qc_report(args.folders, args.output_folder, args.gene_names, args.include_morans_i)
+    generate_qc_report(args.folders, args.output_folder, args.gene_names, args.include_morans_i, max_workers=args.mw)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `Pseudovisium-0.0.2/Pseudovisium.egg-info/PKG-INFO` & `Pseudovisium-0.0.3/Pseudovisium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.2/setup.py` & `Pseudovisium-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="Pseudovisium",
     version=VERSION,
```

