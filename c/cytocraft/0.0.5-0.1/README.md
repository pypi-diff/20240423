# Comparing `tmp/cytocraft-0.0.5.tar.gz` & `tmp/cytocraft-0.1.tar.gz`

## Comparing `cytocraft-0.0.5.tar` & `cytocraft-0.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0    18340 2020-02-02 00:00:00.000000 cytocraft-0.0.5/tutorial.ipynb
--rw-r--r--   0        0        0  1206690 2020-02-02 00:00:00.000000 cytocraft-0.0.5/figure/Figure1.Overview.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/__init__.py
--rwxr-xr-x   0        0        0    28808 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/craft.py
--rwxr-xr-x   0        0        0     9092 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/model.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/plot.py
--rwxr-xr-x   0        0        0     3555 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/rigid.py
--rwxr-xr-x   0        0        0     7939 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/shape.py
--rwxr-xr-x   0        0        0    18668 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/simulation.py
--rwxr-xr-x   0        0        0    35848 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/stereopy.py
--rwxr-xr-x   0        0        0     3503 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/util.py
--rw-r--r--   0        0        0 10647400 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/gtf/AmexT_v47-AmexG_v6.0-DD.gene.gtf
--rw-r--r--   0        0        0 11511594 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/gtf/gencode.v44.basic.annotation.gene.gtf
--rw-r--r--   0        0        0 10634109 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/gtf/gencode.vM34.annotation.gene.gtf
--rwxr-xr-x   0        0        0  5275667 2020-02-02 00:00:00.000000 cytocraft-0.0.5/src/cytocraft/gtf/mice_genes.gtf
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cytocraft-0.0.5/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cytocraft-0.0.5/LICENSE
--rwxr-xr-x   0        0        0     1253 2020-02-02 00:00:00.000000 cytocraft-0.0.5/README.md
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 cytocraft-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 cytocraft-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0   190842 2020-02-02 00:00:00.000000 cytocraft-0.1/figure/Figure1.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/__init__.py
+-rwxr-xr-x   0        0        0    26767 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/craft.py
+-rwxr-xr-x   0        0        0     9092 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/model.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/plot.py
+-rwxr-xr-x   0        0        0     3555 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/rigid.py
+-rwxr-xr-x   0        0        0     7939 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/shape.py
+-rwxr-xr-x   0        0        0    18668 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/simulation.py
+-rwxr-xr-x   0        0        0    35848 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/stereopy.py
+-rwxr-xr-x   0        0        0     3503 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/util.py
+-rw-r--r--   0        0        0 10647400 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/gtf/AmexT_v47-AmexG_v6.0-DD.gene.gtf
+-rw-r--r--   0        0        0 11511594 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/gtf/gencode.v44.basic.annotation.gene.gtf
+-rw-r--r--   0        0        0 10634109 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/gtf/gencode.vM34.annotation.gene.gtf
+-rwxr-xr-x   0        0        0  5275667 2020-02-02 00:00:00.000000 cytocraft-0.1/src/cytocraft/gtf/mice_genes.gtf
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cytocraft-0.1/LICENSE
+-rwxr-xr-x   0        0        0     1197 2020-02-02 00:00:00.000000 cytocraft-0.1/README.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 cytocraft-0.1/pyproject.toml
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 cytocraft-0.1/PKG-INFO
```

### Comparing `cytocraft-0.0.5/src/cytocraft/craft.py` & `cytocraft-0.1/src/cytocraft/craft.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 Wi_filter = Wi[~np.isnan(Wi).any(axis=1), :]
             idx = int(find_subarray(Wi_filter, Wi[i * 2]) / 2)
             Xi = X[Mask[i, :], :]
             model = factor(Wi_filter)
             _, R, _ = numpy_svd_rmsd_rot(np.dot(model.Rs[idx], model.Ss[0]).T, Xi)
             Rotation[i] = R
         except Exception as err:
-            print("Cell ID" + str(CellUIDs[i]) + " is removed due to: ", err)
+            print("Cell No." + str(i + 1) + " is removed due to: ", err)
             pop_indices.append(i)
     for i in sorted(pop_indices, reverse=True):
         Rotation = np.delete(Rotation, obj=i, axis=0)
         W = np.delete(W, obj=i * 2 + 1, axis=0)
         W = np.delete(W, obj=i * 2, axis=0)
         adata = adata[~(adata.obs.index.values == str(CellUIDs[i])), :]
         del CellUIDs[i]
@@ -239,19 +239,18 @@
     new_array = array[:, keep_cols]
     Genes = list(np.array(Genes)[keep_cols])
 
     # return the new array
     return new_array, Genes
 
 
-def get_gene_chr(species):
+def gene_chr(species):
     if species == "Mouse" or species == "Mice":
         gtf_file = (
-            os.path.dirname(os.path.realpath(__file__))
-            + "/gtf/gencode.vM34.annotation.gene.gtf"
+            os.path.dirname(os.path.realpath(__file__)) + "/gtf/mice_genes.gene.gtf"
         )
     elif species == "Axolotls" or species == "Axolotl":
         gtf_file = (
             os.path.dirname(os.path.realpath(__file__))
             + "/gtf/AmexT_v47-AmexG_v6.0-DD.gene.gtf"
         )
     elif species == "Human" or species == "Monkey":
@@ -293,32 +292,29 @@
     for n, _ in tqdm(enumerate(GeneList)):
         for m, _ in enumerate(GeneList[: n + 1]):
             d = np.linalg.norm(X.iloc[n] - X.iloc[m])
             DM[n, m] = DM[m, n] = d
     return DM
 
 
-def RMSD_distance_matrix(Xs, GeneLists, keys, ngene=100, method=None):
+def RMSD_distance_matrix(Xs, GeneLists, keys, ngene=100):
     N = len(keys)
     DM = np.zeros((N, N))
 
     for n, key_n in tqdm(enumerate(keys)):
         for m, key_m in enumerate(keys[: n + 1]):
             intersected_values = np.intersect1d(GeneLists[key_n], GeneLists[key_m])[
                 :ngene
             ]
             boolean_arrays_n = np.in1d(GeneLists[key_n], intersected_values)
             boolean_arrays_m = np.in1d(GeneLists[key_m], intersected_values)
-            X_n = Xs[key_n][boolean_arrays_n]
-            X_m = Xs[key_m][boolean_arrays_m]
-            if method:
-                X_n = normalizeX(X_n, method=method)
-                X_m = normalizeX(X_m, method=method)
-            d1, _, _ = numpy_svd_rmsd_rot(X_n, X_m)
-            d2, _, _ = numpy_svd_rmsd_rot(mirror(X_n), X_m)
+            normalized_x_n = normalizeX(Xs[key_n][boolean_arrays_n], method="mean")
+            normalized_x_m = normalizeX(Xs[key_m][boolean_arrays_m], method="mean")
+            d1, _, _ = numpy_svd_rmsd_rot(normalized_x_n, normalized_x_m)
+            d2, _, _ = numpy_svd_rmsd_rot(mirror(normalized_x_n), normalized_x_m)
             DM[n, m] = DM[m, n] = min(d1, d2)
     return DM
 
 
 def mirror(X):
     mirrorX = np.copy(X)
     mirrorX[:, 2] = -mirrorX[:, 2]
@@ -497,23 +493,14 @@
     # gene column
     if "gene" in gem.columns:
         gem.rename(columns={"gene": "geneID"}, inplace=True)
 
     return gem
 
 
-def read_gem_as_adata(gem_path, sep="\t", SN="adata"):
-    data = read_gem(file_path=gem_path, bin_type="cell_bins", sep=sep)
-    data.tl.raw_checkpoint()
-    adata = stereo_to_anndata(
-        data, flavor="scanpy", sample_id=SN, reindex=False, output=None
-    )
-    return adata
-
-
 def change_last_true(arr):
     # Find the index of the last True value
     last_true_index = np.where(arr == True)[0][-1]
 
     # Set the value at that index to False
     arr[last_true_index] = False
 
@@ -594,191 +581,162 @@
     if method == "L2norm":
         return x / (np.linalg.norm(x) ** 2)
     elif method == "mean":
         r = mean_radius(x)
         return x / r
 
 
-def get_GeneUID(gem):
-    return list(
-        gem.groupby(["geneID"])["MIDCount"]
-        .count()
-        .reset_index(name="Count")
-        .sort_values(["Count"], ascending=False)
-        .geneID
-    )
-
-
-def get_CellUID(gem):
-    return list(gem.CellID.drop_duplicates())
-
-
-def run_craft(
+def craft(
     gem_path,
     species,
     seed,
+    threshold_for_gene_filter,
+    percent_of_gene_for_rotation_derivation,
     out_path,
     sep,
-    threshold_for_gene_filter=0.9,
-    threshold_for_rmsd=0.25,
-    Ngene_for_rotation_derivation=None,
-    percent_of_gene_for_rotation_derivation=0.001,
 ):
     # set seed
     random.seed(seed)
     np.random.seed(seed)
     #################### INIT ####################
     models = []
-    SN = os.path.basename(os.path.splitext(gem_path)[0])
+    filename, _ = os.path.splitext(gem_path)
+    SN = os.path.basename(filename)
     TID = generate_id()
     outpath = out_path + "/" + SN + "_" + TID + "/"
 
     # make dir
     Path(outpath).mkdir(parents=True, exist_ok=True)
     # start logging
     stdout = sys.stdout
     log_file = open(outpath + "/" + SN + "_" + TID + ".log", "w")
     sys.stdout = log_file
+
+    #################### PROCESSING #####################
     # read input gem
     gem = read_gem_as_csv(gem_path, sep=sep)
-    adata = read_gem_as_adata(gem_path, sep=sep, SN=SN)
-    GeneUIDs = get_GeneUID(gem)
-    if Ngene_for_rotation_derivation is None:
-        Ngene_for_rotation_derivation = int(
-            float(percent_of_gene_for_rotation_derivation) * len(GeneUIDs)
-        )
-    adata = craft(
-        gem=gem,
-        adata=adata,
-        species=species,
-        nderive=Ngene_for_rotation_derivation,
-        thresh=threshold_for_gene_filter,
-        thresh_rmsd=threshold_for_rmsd,
-        seed=seed,
-        samplename=SN,
-        outpath=outpath,
-    )
-
-    #################### SAVING #####################
-    adata.write_h5ad(filename=outpath + "adata.h5ad")
 
-    # stop logging
-    sys.stdout = stdout
-    log_file.close()
-
-
-def craft(
-    gem,
-    adata,
-    species,
-    nderive=10,
-    thresh=0.9,
-    thresh_rmsd=0.25,
-    seed=999,
-    samplename=None,
-    outpath=False,
-):
-    # set seed
-    random.seed(seed)
-    np.random.seed(seed)
-    TID = generate_id()
-    # run cytocraft
-    GeneUIDs = get_GeneUID(gem)
-    CellUIDs = get_CellUID(gem)
-
-    print("Speceis: " + species)
-    if samplename:
-        print("Sample Name: " + samplename)
+    GeneUIDs = list(
+        gem.groupby(["geneID"])["MIDCount"]
+        .count()
+        .reset_index(name="Count")
+        .sort_values(["Count"], ascending=False)
+        .geneID
+    )
+    CellUIDs = list(gem.CellID.drop_duplicates())
 
     print(
-        "Seed: "
+        "Speceis: "
+        + species
+        + "\n"
+        + "File Name:"
+        + filename
+        + "\n"
+        + "Seed: "
         + str(seed)
         + "\n"
         + "Cell Number: "
         + str(len(CellUIDs))
         + "\n"
         + "Gene Number: "
         + str(len(GeneUIDs))
         + "\n"
+        + "Sample Name: "
+        + SN
+        + "\n"
         + "Threshold for gene filter is: "
-        + str(thresh)
+        + str(threshold_for_gene_filter)
         + "\n"
-        + "Number of genes used for Rotation Derivation is: "
-        + str(nderive)
+        + "Proportion of genes used for Rotation Derivation is: "
+        + str(percent_of_gene_for_rotation_derivation)
         + "\n"
         + "Task ID: "
         + TID
         + "\n"
     )
+    Ngene_for_rotation_derivation = int(
+        percent_of_gene_for_rotation_derivation * len(GeneUIDs)
+    )
 
-    # processing gtf
-    gene_chr = get_gene_chr(species)
+    ### processing gtf
+    gene_chr = gene_chr(species)
 
+    ##### generate random RM and derive X
+    # adata
+    data = read_gem(file_path=gem_path, bin_type="cell_bins", sep=sep)
+    data.tl.raw_checkpoint()
+    adata = stereo_to_anndata(
+        data, flavor="scanpy", sample_id=SN, reindex=False, output=None
+    )
     # generate and normalize W
     W = genedistribution(gem, CellUIDs, GeneUIDs)
-    W, GeneUIDs = filterGenes(W, GeneUIDs, threshold=thresh)
+    W, GeneUIDs = filterGenes(W, GeneUIDs, threshold=threshold_for_gene_filter)
     W = normalizeW(W)
     # generate random Rotation Matrix
     RM = generate_random_rotation_matrices(int(W.shape[0] / 2))
     X, W, GeneUIDs = UpdateX(RM, W, GeneUIDs)
-    if outpath:
-        write_pdb(
-            X,
-            gene_chr,
-            GeneUIDs,
-            write_path=outpath,
-            sp=species,
-            seed=seed,
-            prefix=samplename + "_initial_chr",
-        )
-    # update X
+    write_pdb(
+        X,
+        gene_chr,
+        GeneUIDs,
+        write_path=outpath,
+        sp=species,
+        seed=seed,
+        prefix=SN + "_initial_chr",
+    )
+    ##### update X
     for loop in range(30):
-        ## step1: derive Rotation Matrix
+        # step1: derive Rotation Matrix
         Mask = MASK(
             gem,
             GeneIDs=GeneUIDs,
             CellIDs=CellUIDs,
-            Ngene=nderive,
+            Ngene=Ngene_for_rotation_derivation,
         )
         RM, W, CellUIDs, adata = DeriveRotation(W, X, Mask, CellUIDs, adata)
-        ## step2: update conformation X with RM and W
+        # step2: update conformation X with RM and W
         try:
             newX, W, GeneUIDs, X = UpdateX(RM, W, GeneUIDs, X)
         except np.linalg.LinAlgError:
             return "numpy.linalg.LinAlgError"
         rmsd, _, _ = numpy_svd_rmsd_rot(
             normalizeX(X, method="mean"), normalizeX(newX, method="mean")
         )
         print(
             "Distance between X_new and X_old for loop "
             + str(loop + 1)
             + " is: "
             + str(rmsd)
         )
-        if outpath:
-            write_pdb(
-                newX,
-                gene_chr,
-                GeneUIDs,
-                write_path=outpath,
-                sp=species,
-                seed=seed,
-                prefix=samplename + "_updated" + str(loop + 1) + "times_chr",
-            )
-        ## step3: check if conformation converges
+        write_pdb(
+            newX,
+            gene_chr,
+            GeneUIDs,
+            write_path=outpath,
+            sp=species,
+            seed=seed,
+            prefix=SN + "_updated" + str(loop + 1) + "times_chr",
+        )
+        ## keep looping until X converges
         X = newX
-        if rmsd < thresh_rmsd:
+        if rmsd < 0.25:
             break
+
+    #################### SAVING #####################
     print("Number of total Transcription centers is: " + str(X.shape[0]))
 
     adata.obsm["Rotation"] = RM
     adata.uns["X"] = pd.DataFrame(X, index=GeneUIDs)
     adata.uns["X"].columns = adata.uns["X"].columns.astype(str)
     adata.uns["W"] = W
-    return adata
+    adata.write_h5ad(filename=outpath + "adata.h5ad")
+
+    # stop logging
+    sys.stdout = stdout
+    log_file.close()
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Cytocraft Main Function")
 
     parser.add_argument(
         "gem_path",
@@ -800,42 +758,28 @@
         "-p",
         "--percent",
         type=float,
         help="percent of gene for rotation derivation, default: 0.001",
         default=0.001,
     )
     parser.add_argument(
-        "-n",
-        "--number",
-        type=int,
-        help="number of gene for rotation derivation, recommend: 10",
-        default=None,
-    )
-    parser.add_argument(
         "-t",
-        "--gene_filter_thresh",
+        "--threshold",
         type=float,
-        help="The maximum proportion of np.nans allowed in a column(gene) in W, default: 0.90",
+        help="The maximum proportion of np.nans allowed in a column(gene) in W",
         default=0.90,
     )
     parser.add_argument(
-        "-r",
-        "--rmsd_thresh",
-        type=float,
-        help="The maximum value of cvRMSD allowed in conformation convergence, default: 0.25",
-        default=0.25,
-    )
-    parser.add_argument(
         "--sep", type=str, help="input gem file separator", default="\t"
     )
     parser.add_argument(
         "-c",
         "--celltype",
         type=str,
-        help="Path of obs file containing cell types",
+        help="Path of file containing cell types",
     )
     parser.add_argument(
         "--ctkey",
         type=str,
         help="Key of celltype column in the annotation file",
     )
     parser.add_argument(
@@ -853,83 +797,65 @@
     )
 
     args = parser.parse_args()
 
     return args
 
 
-def split_gem(gem_path, celltype, ctkey, cikey, gsep):
-    split_gem_paths = {}
-    gem = read_gem_as_csv(gem_path, sep=gsep)
-    for ct in celltype[ctkey].drop_duplicates():
-        ct_legal = legalname(ct)
-        gem_ct_path = gem_path + "." + ctkey + "." + ct_legal + ".tsv"
-        split_gem_paths[ct] = gem_ct_path
-        print("split gem path of " + ct + " : " + gem_ct_path)
-        if cikey is not None:
-            cellids = celltype[celltype[ctkey] == ct][cikey].values.astype(str)
-        else:
-            cellids = celltype[celltype[ctkey] == ct].index.values.astype(str)
-        gem[gem.CellID.isin(cellids)].to_csv(gem_ct_path, sep="\t", index=False)
-    return split_gem_paths
-
-
 def main():
     #################### SETTINGS ####################
     args = parse_args()
     if args.seed is not None:
         seed = args.seed
     else:
         seed = random.randint(0, 1000)
 
-    #################### RUNNING #####################
+    #################### RUNNING ####################
     if args.celltype is not None:  # run multiple cell types
         print("Cell types have been set (path is %s)" % args.celltype + "\n")
-        # read gem and obs
-        obs = pd.read_csv(args.celltype, sep=args.csep, dtype=str)
-        # split gem
-        split_paths = split_gem(
-            args.gem_path,
-            celltype=obs,
-            ctkey=args.ctkey,
-            cikey=args.cikey,
-            gsep=args.sep,
-        )
-        # run cytocraft by order
-        for ct, ct_path in split_paths.items():
+        gem = read_gem_as_csv(args.gem_path, sep=args.sep)
+        celltype = pd.read_csv(args.celltype, sep=args.csep, dtype=str)
+        print(celltype[args.ctkey].drop_duplicates())
+        # process cell types
+        for ct in celltype[args.ctkey].drop_duplicates():
+            ct_legal = legalname(ct)
+            gem_ct_path = args.gem_path + "." + args.ctkey + "." + ct_legal + ".tsv"
+            print(args.cikey)
+            if args.cikey is not None:
+                cellids = celltype[celltype[args.ctkey] == ct][args.cikey].values
+            else:
+                cellids = celltype[celltype[args.ctkey] == ct].index.values.astype(str)
+                print(cellids)
+            gem[gem.CellID.isin(cellids)].to_csv(gem_ct_path, sep="\t", index=False)
             try:
-                run_craft(
-                    gem_path=ct_path,
-                    species=args.species,
-                    seed=seed,
-                    out_path=args.out_path,
+                craft(
+                    gem_ct_path,
+                    args.species,
+                    seed,
+                    args.threshold,
+                    args.percent,
+                    args.out_path,
                     sep="\t",
-                    threshold_for_gene_filter=args.gene_filter_thresh,
-                    threshold_for_rmsd=args.rmsd_thresh,
-                    Ngene_for_rotation_derivation=args.number,
-                    percent_of_gene_for_rotation_derivation=args.percent,
                 )
             except Exception as error:
                 print(error)
                 print(ct + ": conformation reconstruction failed.")
                 continue
             else:
                 print(ct + ": conformation reconstruction finished.")
     else:  # run single cell type
         try:
-            run_craft(
-                gem_path=args.gem_path,
-                species=args.species,
-                seed=seed,
-                out_path=args.out_path,
-                sep=args.sep,
-                threshold_for_gene_filter=args.gene_filter_thresh,
-                threshold_for_rmsd=args.rmsd_thresh,
-                Ngene_for_rotation_derivation=args.number,
-                percent_of_gene_for_rotation_derivation=args.percent,
+            craft(
+                args.gem_path,
+                args.species,
+                seed,
+                args.threshold,
+                args.percent,
+                args.out_path,
+                args.sep,
             )
         except Exception as error:
             print(error)
             print("conformation reconstruction failed.")
         else:
             print("conformation reconstruction finished.")
```

### Comparing `cytocraft-0.0.5/src/cytocraft/model.py` & `cytocraft-0.1/src/cytocraft/model.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/plot.py` & `cytocraft-0.1/src/cytocraft/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,14 @@
     labels,
     cmap="viridis",
     method="average",
     cthresh=4.8,
     font_scale=1,
     cbbox=(0.07, 0.84, 0.04, 0.12),
     lgbox=(0.86, 0.96, 0.01, 0.01),
-    ticks=[0, 0.5, 1, 1.5],
-    figsize=(8, 8),
-    dpi=300,
 ):
     clustergrid = sns.clustermap(
         D, xticklabels=labels, yticklabels=labels, method=method
     )
     plt.close()
 
     # Get clusters with threshold
@@ -70,27 +67,27 @@
     n_clusters = len(np.unique(clusters))
     color_map = sns.color_palette("rainbow", n_clusters)
 
     # Assign colors to clusters
     cluster_colors = [color_map[c - 1] for c in clusters]
 
     # Draw plot
-    sns.set(rc={"figure.dpi": dpi, "figure.figsize": figsize}, font_scale=font_scale)
+    sns.set(rc={"figure.dpi": 300, "figure.figsize": (8, 8)}, font_scale=font_scale)
 
     ax = sns.clustermap(
         D,
         xticklabels=labels,
         yticklabels=labels,
         cmap=cmap,
         method=method,
         row_colors=[cluster_colors],
         col_colors=[cluster_colors],
-        cbar_kws={"ticks": ticks},
+        cbar_kws={"ticks": [0, 0.5, 1, 1.5]},
     )
-    ax.ax_cbar.set_title("RMSD")
+    ax.ax_cbar.set_title("NRMSD")
     ax.ax_cbar.set_position(cbbox)
 
     # Add legend for row color bar
     from matplotlib.patches import Patch
 
     lut = dict(zip(clusters, cluster_colors))
     handles = [Patch(facecolor=lut[name]) for name in sorted(lut)]
@@ -105,21 +102,20 @@
     )
     legend.get_frame().set_facecolor("white")
 
 
 def plot_network(
     D,
     labels,
-    cmap="viridis",
+    cmap,
     csep="\n",
     solver="barnesHut",
-    corder=0,
+    corder=1,
     N_neighbor=3,
     html="test.html",
-    fontsize=15,
     width=1400,
     height=1000,
     edge_scale=150,
     edge_adjust=-60,
 ):
     from pyvis.network import Network
     from IPython.display import HTML
@@ -171,15 +167,15 @@
     net.show_buttons()
 
     json_obj = {
         "configure": {"enabled": True, "filter": ["nodes", "edges", "physics"]},
         "nodes": {
             "borderWidth": 3,
             "opacity": 1,
-            "font": {"size": fontsize, "strokeWidth": 5},
+            "font": {"size": 15, "strokeWidth": 5},
             "size": 0,
         },
         "edges": {
             "color": {"opacity": 0.7},
             "selfReferenceSize": 0,
             "selfReference": {"size": 0, "angle": 0.7853981633974483},
             "smooth": {"forceDirection": "vertical"},
```

### Comparing `cytocraft-0.0.5/src/cytocraft/rigid.py` & `cytocraft-0.1/src/cytocraft/rigid.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/shape.py` & `cytocraft-0.1/src/cytocraft/shape.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/simulation.py` & `cytocraft-0.1/src/cytocraft/simulation.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/stereopy.py` & `cytocraft-0.1/src/cytocraft/stereopy.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/util.py` & `cytocraft-0.1/src/cytocraft/util.py`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/gtf/AmexT_v47-AmexG_v6.0-DD.gene.gtf` & `cytocraft-0.1/src/cytocraft/gtf/AmexT_v47-AmexG_v6.0-DD.gene.gtf`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/gtf/gencode.v44.basic.annotation.gene.gtf` & `cytocraft-0.1/src/cytocraft/gtf/gencode.v44.basic.annotation.gene.gtf`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/gtf/gencode.vM34.annotation.gene.gtf` & `cytocraft-0.1/src/cytocraft/gtf/gencode.vM34.annotation.gene.gtf`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/src/cytocraft/gtf/mice_genes.gtf` & `cytocraft-0.1/src/cytocraft/gtf/mice_genes.gtf`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/LICENSE` & `cytocraft-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cytocraft-0.0.5/README.md` & `cytocraft-0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-# Cytocraft
-
 <p align="center">
-	<img src=https://github.com/YifeiSheng/Cytocraft/raw/main/figure/Figure1.Overview.png>
+	<img width="712" height="342" src=https://github.com/YifeiSheng/Cytocraft/blob/main/figure/Figure1.png>
 </p>
 
-## Overview
+# Cytocraft
 
 The Cytocraft package provides prediction of chromosome conformation based on spatial transcriptomic.
 
-## Installaion
-
-```
-pip install cytocraft
-```
-
 ## Quick Start
 
 ### Run Cytocraft
 
 This example shows the usage of Cytocraft.
 
 	python craft.py ./data/SS200000108BR_A3A4_scgem.Spinal_cord_neuron.csv ./results/ Mouse
 
 ## Usage
-```
-python craft.py [-h] [-p PERCENT] [-c CELLTYPE] [--ctkey CTKEY] [--cikey CIKEY] [--seed SEED] gem_path out_path {Human,Mouse,Axolotls,Monkey}
-```
+
+craft.py [-h] [-p PERCENT] [-c CELLTYPE] [--ctkey CTKEY] [--cikey CIKEY] [--seed SEED] gem_path out_path {Human,Mouse,Axolotls,Monkey}
+
 ### positional arguments:
 
   gem_path              `Path to gem file`
 
   out_path              `Output path to save results`
 
   {Human,Mouse,Axolotls,Monkey} `Species of the input data`
```

### Comparing `cytocraft-0.0.5/pyproject.toml` & `cytocraft-0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "/.git",
     "/demo",
   ]
 [tool.hatch.build.targets.wheel]
   packages = ["src/cytocraft"]
 [project]
   name = "cytocraft"
-  version = "0.0.5"
+  version = "0.1"
   dependencies = ["scanpy","shapely"]
   authors = [
     { name="Yifei Sheng", email="yfsheng6@gmail.com" },
     { name="Shiying Li", email="shiyingli7-c@my.cityu.edu.hk"},
     { name="Shuai Cheng Li", email="sc.li@cityu.edu.hk"},
   ]
   description = "The Cytocraft package provides prediction of chromosome conformation based on spatial transcriptomic."
```

### Comparing `cytocraft-0.0.5/PKG-INFO` & `cytocraft-0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cytocraft
-Version: 0.0.5
+Version: 0.1
 Summary: The Cytocraft package provides prediction of chromosome conformation based on spatial transcriptomic.
 Project-URL: Homepage, https://github.com/YifeiSheng/Cytocraft
 Project-URL: Issues, https://github.com/YifeiSheng/Cytocraft/issues
 Project-URL: Repository, https://github.com/YifeiSheng/Cytocraft.git
 Author-email: Yifei Sheng <yfsheng6@gmail.com>, Shiying Li <shiyingli7-c@my.cityu.edu.hk>, Shuai Cheng Li <sc.li@cityu.edu.hk>
 License: MIT license
 License-File: LICENSE
@@ -15,42 +15,34 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8
 Requires-Dist: scanpy
 Requires-Dist: shapely
 Description-Content-Type: text/markdown
 
-# Cytocraft
-
 <p align="center">
-	<img src=https://github.com/YifeiSheng/Cytocraft/raw/main/figure/Figure1.Overview.png>
+	<img width="712" height="342" src=https://github.com/YifeiSheng/Cytocraft/blob/main/figure/Figure1.png>
 </p>
 
-## Overview
+# Cytocraft
 
 The Cytocraft package provides prediction of chromosome conformation based on spatial transcriptomic.
 
-## Installaion
-
-```
-pip install cytocraft
-```
-
 ## Quick Start
 
 ### Run Cytocraft
 
 This example shows the usage of Cytocraft.
 
 	python craft.py ./data/SS200000108BR_A3A4_scgem.Spinal_cord_neuron.csv ./results/ Mouse
 
 ## Usage
-```
-python craft.py [-h] [-p PERCENT] [-c CELLTYPE] [--ctkey CTKEY] [--cikey CIKEY] [--seed SEED] gem_path out_path {Human,Mouse,Axolotls,Monkey}
-```
+
+craft.py [-h] [-p PERCENT] [-c CELLTYPE] [--ctkey CTKEY] [--cikey CIKEY] [--seed SEED] gem_path out_path {Human,Mouse,Axolotls,Monkey}
+
 ### positional arguments:
 
   gem_path              `Path to gem file`
 
   out_path              `Output path to save results`
 
   {Human,Mouse,Axolotls,Monkey} `Species of the input data`
```

