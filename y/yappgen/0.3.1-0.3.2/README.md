# Comparing `tmp/yappgen-0.3.1.tar.gz` & `tmp/yappgen-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappgen-0.3.1.tar", last modified: Fri Mar  3 07:46:08 2023, max compression
+gzip compressed data, was "yappgen-0.3.2.tar", last modified: Tue Apr 23 13:52:25 2024, max compression
```

## Comparing `yappgen-0.3.1.tar` & `yappgen-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-03-03 07:46:08.304202 yappgen-0.3.1/
--rw-r--r--   0 bertrand   (501) staff       (20)    26526 2022-03-02 12:31:43.000000 yappgen-0.3.1/LICENSE
--rw-r--r--   0 bertrand   (501) staff       (20)     1115 2023-03-03 07:46:08.304259 yappgen-0.3.1/PKG-INFO
--rw-r--r--   0 bertrand   (501) staff       (20)      803 2023-03-03 07:37:49.000000 yappgen-0.3.1/README.md
-drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-03-03 07:46:08.300863 yappgen-0.3.1/bin/
--rwxr-xr-x   0 bertrand   (501) staff       (20)     6130 2022-08-25 15:25:57.000000 yappgen-0.3.1/bin/fphtrain
--rw-r--r--   0 bertrand   (501) staff       (20)     5021 2022-08-25 15:25:57.000000 yappgen-0.3.1/bin/yapp
--rw-r--r--   0 bertrand   (501) staff       (20)      186 2023-03-03 07:46:08.304472 yappgen-0.3.1/setup.cfg
--rw-r--r--   0 bertrand   (501) staff       (20)      812 2023-03-03 07:35:36.000000 yappgen-0.3.1/setup.py
-drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-03-03 07:46:08.303325 yappgen-0.3.1/yapp/
--rw-r--r--   0 bertrand   (501) staff       (20)      138 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/__init__.py
--rw-r--r--   0 bertrand   (501) staff       (20)    36695 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/family_phaser.py
--rw-r--r--   0 bertrand   (501) staff       (20)     8032 2022-08-25 15:25:57.000000 yappgen-0.3.1/yapp/gamete.py
--rwxr-xr-x   0 bertrand   (501) staff       (20)    10173 2022-08-25 15:25:57.000000 yappgen-0.3.1/yapp/lmm.py
--rw-r--r--   0 bertrand   (501) staff       (20)     5681 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/mendel.py
--rw-r--r--   0 bertrand   (501) staff       (20)     6727 2022-08-25 15:25:57.000000 yappgen-0.3.1/yapp/origins.py
--rw-r--r--   0 bertrand   (501) staff       (20)    15828 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/pedigree.py
--rw-r--r--   0 bertrand   (501) staff       (20)    20470 2022-08-25 15:25:57.000000 yappgen-0.3.1/yapp/recombination.py
--rw-r--r--   0 bertrand   (501) staff       (20)     7182 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/sperm.py
--rw-r--r--   0 bertrand   (501) staff       (20)    11788 2022-08-25 15:25:57.000000 yappgen-0.3.1/yapp/vcf.py
--rw-r--r--   0 bertrand   (501) staff       (20)     5873 2023-03-03 07:35:36.000000 yappgen-0.3.1/yapp/wcsp.py
-drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-03-03 07:46:08.304074 yappgen-0.3.1/yappgen.egg-info/
--rw-r--r--   0 bertrand   (501) staff       (20)     1115 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/PKG-INFO
--rw-r--r--   0 bertrand   (501) staff       (20)      417 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/SOURCES.txt
--rw-r--r--   0 bertrand   (501) staff       (20)        1 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/dependency_links.txt
--rw-r--r--   0 bertrand   (501) staff       (20)        1 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/not-zip-safe
--rw-r--r--   0 bertrand   (501) staff       (20)      106 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/requires.txt
--rw-r--r--   0 bertrand   (501) staff       (20)        5 2023-03-03 07:46:08.000000 yappgen-0.3.1/yappgen.egg-info/top_level.txt
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 13:52:25.554038 yappgen-0.3.2/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    26526 2023-04-12 12:19:27.000000 yappgen-0.3.2/LICENSE
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     1116 2024-04-23 13:52:25.554038 yappgen-0.3.2/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      804 2024-04-23 13:44:26.000000 yappgen-0.3.2/README.md
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 13:52:25.554038 yappgen-0.3.2/bin/
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     6130 2023-04-12 12:19:27.000000 yappgen-0.3.2/bin/fphtrain
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5021 2023-04-12 12:19:27.000000 yappgen-0.3.2/bin/yapp
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      186 2024-04-23 13:52:25.554038 yappgen-0.3.2/setup.cfg
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      812 2024-04-23 13:44:26.000000 yappgen-0.3.2/setup.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 13:52:25.554038 yappgen-0.3.2/yapp/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      138 2024-04-23 13:50:53.000000 yappgen-0.3.2/yapp/__init__.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    36683 2024-04-23 13:46:45.000000 yappgen-0.3.2/yapp/family_phaser.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     8029 2024-04-23 13:48:37.000000 yappgen-0.3.2/yapp/gamete.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)    10173 2023-04-12 12:19:27.000000 yappgen-0.3.2/yapp/lmm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5672 2024-04-23 13:49:12.000000 yappgen-0.3.2/yapp/mendel.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     6724 2024-04-23 13:49:29.000000 yappgen-0.3.2/yapp/origins.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    15770 2024-04-23 13:44:26.000000 yappgen-0.3.2/yapp/pedigree.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    20467 2024-04-23 13:49:53.000000 yappgen-0.3.2/yapp/recombination.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     7182 2023-04-12 12:19:27.000000 yappgen-0.3.2/yapp/sperm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    11776 2024-04-23 13:50:19.000000 yappgen-0.3.2/yapp/vcf.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5873 2023-04-12 12:19:27.000000 yappgen-0.3.2/yapp/wcsp.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 13:52:25.554038 yappgen-0.3.2/yappgen.egg-info/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     1116 2024-04-23 13:52:25.000000 yappgen-0.3.2/yappgen.egg-info/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      417 2024-04-23 13:52:25.000000 yappgen-0.3.2/yappgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-04-23 13:52:25.000000 yappgen-0.3.2/yappgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2023-04-12 12:23:00.000000 yappgen-0.3.2/yappgen.egg-info/not-zip-safe
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      106 2024-04-23 13:52:25.000000 yappgen-0.3.2/yappgen.egg-info/requires.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        5 2024-04-23 13:52:25.000000 yappgen-0.3.2/yappgen.egg-info/top_level.txt
```

### Comparing `yappgen-0.3.1/LICENSE` & `yappgen-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/PKG-INFO` & `yappgen-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappgen
-Version: 0.3.1
+Version: 0.3.2
 Summary: Yet Another Phasing Program
 Home-page: https://forgemia.inra.fr/bertrand.servin/yapp
 Author: Bertrand Servin
 Author-email: bertrand.servin@inrae.fr
 License: LGPLv2.1
 Requires-Python: <3.10
 Description-Content-Type: text/markdown
@@ -22,8 +22,8 @@
 @BertrandServin). If you want to contribute ideas or code, you are
 welcome if you know python :)
 
 yapp and its utilities implement some models and methods that have been
 invented by other people. If you use yapp it is important that you
 acknowledge their work by citing the appropriate
 references. These will depend on the way you use the software, see the
-[documentation](https://yapp.readthedocs.io).
+[documentation](https://yapp-doc.netlify.app).
```

### Comparing `yappgen-0.3.1/README.md` & `yappgen-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 @BertrandServin). If you want to contribute ideas or code, you are
 welcome if you know python :)
 
 yapp and its utilities implement some models and methods that have been
 invented by other people. If you use yapp it is important that you
 acknowledge their work by citing the appropriate
 references. These will depend on the way you use the software, see the
-[documentation](https://yapp.readthedocs.io).
+[documentation](https://yapp-doc.netlify.app).
```

### Comparing `yappgen-0.3.1/bin/fphtrain` & `yappgen-0.3.2/bin/fphtrain`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/bin/yapp` & `yappgen-0.3.2/bin/yapp`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/setup.py` & `yappgen-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/yapp/family_phaser.py` & `yappgen-0.3.2/yapp/family_phaser.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         obj = cls(genotype)
         paternal_gamete = gamete.Gamete(paternal_hap)
         obj.update_paternal_gamete(paternal_gamete)
         maternal_gamete = gamete.Gamete(maternal_hap)
         obj.update_maternal_gamete(maternal_gamete)
         assert len(paternal_si) == obj.len
         assert len(maternal_si) == obj.len
-        obj.si_pat = np.array(paternal_si, dtype=np.int)
-        obj.si_mat = np.array(maternal_si, dtype=np.int)
+        obj.si_pat = np.array(paternal_si, dtype=int)
+        obj.si_mat = np.array(maternal_si, dtype=int)
         return obj
 
     @property
     def len(self):
         return len(self.g)
 
     @property
@@ -252,16 +252,16 @@
         # Compute Posterior probabilities
         post_si = fwd * rew
         post_si /= np.sum(post_si, axis=1, keepdims=True)  # required ?
 
         # 3. Viterbi Algorithm
         # viterbi variables
         delta = np.zeros((self.len, 2), dtype=np.float)
-        psi = np.zeros((self.len, 2), dtype=np.int)
-        soluce = np.empty(self.len, dtype=np.int)
+        psi = np.zeros((self.len, 2), dtype=int)
+        soluce = np.empty(self.len, dtype=int)
         # init
         delta[0, 0] = np.log(0.5 * emissions[0, 0])
         delta[0, 1] = np.log(0.5 * emissions[0, 1])
         # recursion
         for m in range(1, self.len):
             val_0 = [
                 delta[m - 1, 0] + np.log(transitions[m - 1, 0, 0]),
```

### Comparing `yappgen-0.3.1/yapp/gamete.py` & `yappgen-0.3.2/yapp/gamete.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(self, hap=None):
         self.haplotype = hap
 
     @staticmethod
     def valid_genotype(genotype):
         try:
-            geno = np.array(genotype, dtype=np.int)
+            geno = np.array(genotype, dtype=int)
         except ValueError:
             print("Genotype must be castable to a numpy array of integers")
             raise
         else:
             try:
                 assert len(geno.shape) == 1
             except AssertionError:
```

### Comparing `yappgen-0.3.1/yapp/lmm.py` & `yappgen-0.3.2/yapp/lmm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/yapp/mendel.py` & `yappgen-0.3.2/yapp/mendel.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cyvcf2 import VCF
 from . import vcf, pedigree
 
 logger = logging.getLogger(__name__)
 
 
 def genotype_vector(genotypes):
-    return np.array([vcf.geno2int(*g[:2]) for g in genotypes], dtype=np.int)
+    return np.array([vcf.geno2int(*g[:2]) for g in genotypes], dtype=int)
 
 
 def mendel_errors(args):
     genotypes, pairs = args
     pairs = np.array(pairs)
     genotypes = np.array(genotypes)
     from_genotypes = np.array(genotypes)[pairs[:, 0], :2]
@@ -101,18 +101,18 @@
     for node in ped:
         if indiv_idx[node.indiv] < 0:
             continue
         for c in node.children:
             if indiv_idx[c.indiv] < 0:
                 continue
             pairs.append((indiv_idx[node.indiv], indiv_idx[c.indiv]))
-    # pairs = np.array(pairs, dtype=np.int)
+    # pairs = np.array(pairs, dtype=int)
 
     geno_getter = ((s.genotypes, pairs) for s in myvcf)
-    merr = np.zeros((len(pairs), 2), dtype=np.int)
+    merr = np.zeros((len(pairs), 2), dtype=int)
     with Pool(args.c) as workers:
         for nerr, nobs in workers.imap_unordered(
             mendel_errors, geno_getter, chunksize=50
         ):
             merr[:, 0] += nerr
             merr[:, 1] += nobs
     tx_err = np.sum(merr[:, 0]) / np.sum(merr[:, 1])
```

### Comparing `yappgen-0.3.1/yapp/origins.py` & `yappgen-0.3.2/yapp/origins.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             return
         for reg in phaser.regions:
             logger.info(f"Working on region {reg}")
             logger.info("Grabbing data")
             segregations = np.array(phaser.data[f"phases/{reg}/segregations"])
             logger.info("Diving in")
             or_z = phaser.data["linkage"].create_group(reg)
-            origins = np.zeros_like(segregations, dtype=np.int)
+            origins = np.zeros_like(segregations, dtype=int)
             for node in phaser.pedigree:
                 node_idx = smpidx[node.indiv]
                 if node.father is None:
                     orig_0 = self.origins[node.indiv + "_p"]
                     origins[
                         node_idx,
                         0,
```

### Comparing `yappgen-0.3.1/yapp/pedigree.py` & `yappgen-0.3.2/yapp/pedigree.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,12 +507,11 @@
         individual in the pedigree
 
         """
         try:
             node = self.nodes[indiv]
         except KeyError:
             raise ValueError(f"Focal individual {indiv} not found in pedigree")
-        if len(self.nodes) > sys.getrecursionlimit():
-            sys.setrecursionlimit(len(self.nodes) + 1)
+        sys.setrecursionlimit(len(self.nodes) + 1)
         relatives = self._get_relatives(node)
         fam = Pedigree.from_pednodes(relatives)
         return fam
```

### Comparing `yappgen-0.3.1/yapp/recombination.py` & `yappgen-0.3.2/yapp/recombination.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             for indiv, par in self.parents.items():
                 logger.info(f"Parent {indiv}")
                 idx = smpidx[indiv]
                 par_resolved = (genotypes[idx] == 1) & (
                     (gametes[idx][0] > 0) | (gametes[idx][1] > 0)
                 )  # noqa
                 node = self.phaser.pedigree.nodes[indiv]
-                n_meio_info = np.zeros(len(pos) - 1, dtype=np.int)
+                n_meio_info = np.zeros(len(pos) - 1, dtype=int)
                 for c in node.children:
                     idx = smpidx[c.indiv]
                     par.meioses[c.indiv] = []
                     child_phased = (gametes[idx][0] > 0) | (gametes[idx][1] > 0)
                     combin_info = par_resolved & child_phased
                     infomk = combin_info.nonzero()[0]
                     if len(infomk) > 0:
```

### Comparing `yappgen-0.3.1/yapp/sperm.py` & `yappgen-0.3.2/yapp/sperm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/yapp/vcf.py` & `yappgen-0.3.2/yapp/vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,32 +200,32 @@
                             dtype=np.float,
                         )
                     )
                 else:
                     geno = [s.genotypes[i] for s in variants[r]]
                     if mode == "genotype":
                         fphdata[r][sid] = np.array(
-                            [geno2int(*g[:2]) for g in geno], dtype=np.int
+                            [geno2int(*g[:2]) for g in geno], dtype=int
                         )
                     elif mode == "inbred":
                         fphdata[r][sid] = np.array(
-                            [geno2hap(*g[:2]) for g in geno], dtype=np.int
+                            [geno2hap(*g[:2]) for g in geno], dtype=int
                         )
                     elif mode == "phased":
                         h1 = []
                         h2 = []
                         for g in geno:
                             if g[2]:
                                 h1.append(g[0])
                                 h2.append(g[1])
                             else:
                                 h1.append(-1)
                                 h2.append(-1)
-                        fphdata[r][sid + ".h1"] = np.array(h1, dtype=np.int)
-                        fphdata[r][sid + ".h2"] = np.array(h2, dtype=np.int)
+                        fphdata[r][sid + ".h1"] = np.array(h1, dtype=int)
+                        fphdata[r][sid + ".h2"] = np.array(h2, dtype=int)
     return {
         "regions": trueregions,
         "samples": smp,
         "variants": variants_summary,
         "data": fphdata,
     }
```

### Comparing `yappgen-0.3.1/yapp/wcsp.py` & `yappgen-0.3.2/yapp/wcsp.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.1/yappgen.egg-info/PKG-INFO` & `yappgen-0.3.2/yappgen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappgen
-Version: 0.3.1
+Version: 0.3.2
 Summary: Yet Another Phasing Program
 Home-page: https://forgemia.inra.fr/bertrand.servin/yapp
 Author: Bertrand Servin
 Author-email: bertrand.servin@inrae.fr
 License: LGPLv2.1
 Requires-Python: <3.10
 Description-Content-Type: text/markdown
@@ -22,8 +22,8 @@
 @BertrandServin). If you want to contribute ideas or code, you are
 welcome if you know python :)
 
 yapp and its utilities implement some models and methods that have been
 invented by other people. If you use yapp it is important that you
 acknowledge their work by citing the appropriate
 references. These will depend on the way you use the software, see the
-[documentation](https://yapp.readthedocs.io).
+[documentation](https://yapp-doc.netlify.app).
```

