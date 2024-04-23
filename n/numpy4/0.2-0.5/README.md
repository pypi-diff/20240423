# Comparing `tmp/numpy4-0.2.tar.gz` & `tmp/numpy4-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy4-0.2.tar", last modified: Mon Apr 22 12:26:31 2024, max compression
+gzip compressed data, was "numpy4-0.5.tar", last modified: Tue Apr 23 14:17:39 2024, max compression
```

## Comparing `numpy4-0.2.tar` & `numpy4-0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 12:26:31.157322 numpy4-0.2/
--rw-rw-rw-   0        0        0      213 2024-04-22 12:26:31.154332 numpy4-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 12:26:31.111950 numpy4-0.2/numpy4/
--rw-rw-rw-   0        0        0     2187 2024-04-22 09:37:22.000000 numpy4-0.2/numpy4/ADS_SMOTE.py
--rw-rw-rw-   0        0        0     1566 2024-04-22 09:15:14.000000 numpy4-0.2/numpy4/ADS_dataCleaning.py
--rw-rw-rw-   0        0        0     3969 2024-04-22 09:42:33.000000 numpy4-0.2/numpy4/ADS_inferentialStats.py
--rw-rw-rw-   0        0        0     1286 2024-04-22 09:30:31.000000 numpy4-0.2/numpy4/ADS_outlierDetection.py
--rw-rw-rw-   0        0        0     1456 2024-04-22 09:13:21.000000 numpy4-0.2/numpy4/ADS_stats.py
--rw-rw-rw-   0        0        0     3432 2024-04-22 09:21:18.000000 numpy4-0.2/numpy4/ADS_superviseEval.py
--rw-rw-rw-   0        0        0     2235 2024-04-22 09:26:56.000000 numpy4-0.2/numpy4/ADS_timeSeries.py
--rw-rw-rw-   0        0        0      996 2024-04-22 09:22:47.000000 numpy4-0.2/numpy4/ADS_unsuperviseEval.py
--rw-rw-rw-   0        0        0     2686 2024-04-22 09:40:14.000000 numpy4-0.2/numpy4/ADS_visualization.py
--rw-rw-rw-   0        0        0     2082 2024-04-22 12:25:11.000000 numpy4-0.2/numpy4/DC_Bankers.py
--rw-rw-rw-   0        0        0     1260 2024-04-22 12:23:48.000000 numpy4-0.2/numpy4/DC_Berkley.py
--rw-rw-rw-   0        0        0     2479 2024-04-22 12:24:14.000000 numpy4-0.2/numpy4/DC_Bully.py
--rw-rw-rw-   0        0        0     1903 2024-04-22 12:24:33.000000 numpy4-0.2/numpy4/DC_RaymondTree.py
--rw-rw-rw-   0        0        0      985 2024-04-22 12:24:45.000000 numpy4-0.2/numpy4/DC_RicartAgrawala.py
--rw-rw-rw-   0        0        0     3564 2024-04-22 12:22:21.000000 numpy4-0.2/numpy4/DC_gc.py
--rw-rw-rw-   0        0        0     1383 2024-04-22 12:22:55.000000 numpy4-0.2/numpy4/DC_globalAvg.py
--rw-rw-rw-   0        0        0     1762 2024-04-22 12:19:22.000000 numpy4-0.2/numpy4/DC_ipc.py
--rw-rw-rw-   0        0        0     2541 2024-04-22 12:25:26.000000 numpy4-0.2/numpy4/DC_loadBalancing.py
--rw-rw-rw-   0        0        0       34 2024-04-22 12:25:53.000000 numpy4-0.2/numpy4/DC_multithreading.py
--rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy4-0.2/numpy4/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 12:26:31.152895 numpy4-0.2/numpy4.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-22 12:26:30.000000 numpy4-0.2/numpy4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2024-04-22 12:26:30.000000 numpy4-0.2/numpy4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 12:26:30.000000 numpy4-0.2/numpy4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-22 12:26:30.000000 numpy4-0.2/numpy4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 12:26:30.000000 numpy4-0.2/numpy4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 12:26:31.157322 numpy4-0.2/setup.cfg
--rw-rw-rw-   0        0        0      312 2024-04-22 12:26:19.000000 numpy4-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.979862 numpy4-0.5/
+-rw-rw-rw-   0        0        0      213 2024-04-23 14:17:39.977862 numpy4-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.950841 numpy4-0.5/numpy4/
+-rw-rw-rw-   0        0        0     2549 2024-04-23 14:09:01.000000 numpy4-0.5/numpy4/ADS_DataCleaning.py
+-rw-rw-rw-   0        0        0     2187 2024-04-22 09:37:22.000000 numpy4-0.5/numpy4/ADS_SMOTE.py
+-rw-rw-rw-   0        0        0     3969 2024-04-22 09:42:33.000000 numpy4-0.5/numpy4/ADS_inferentialStats.py
+-rw-rw-rw-   0        0        0     1286 2024-04-22 09:30:31.000000 numpy4-0.5/numpy4/ADS_outlierDetection.py
+-rw-rw-rw-   0        0        0     1707 2024-04-23 14:08:35.000000 numpy4-0.5/numpy4/ADS_stats.py
+-rw-rw-rw-   0        0        0     6252 2024-04-23 14:09:44.000000 numpy4-0.5/numpy4/ADS_superviseEval.py
+-rw-rw-rw-   0        0        0     2235 2024-04-22 09:26:56.000000 numpy4-0.5/numpy4/ADS_timeSeries.py
+-rw-rw-rw-   0        0        0      996 2024-04-22 09:22:47.000000 numpy4-0.5/numpy4/ADS_unsuperviseEval.py
+-rw-rw-rw-   0        0        0     2456 2024-04-23 14:09:25.000000 numpy4-0.5/numpy4/ADS_visualization.py
+-rw-rw-rw-   0        0        0     2082 2024-04-22 12:25:11.000000 numpy4-0.5/numpy4/DC_Bankers.py
+-rw-rw-rw-   0        0        0     1260 2024-04-22 12:23:48.000000 numpy4-0.5/numpy4/DC_Berkley.py
+-rw-rw-rw-   0        0        0     2479 2024-04-22 12:24:14.000000 numpy4-0.5/numpy4/DC_Bully.py
+-rw-rw-rw-   0        0        0     1903 2024-04-22 12:24:33.000000 numpy4-0.5/numpy4/DC_RaymondTree.py
+-rw-rw-rw-   0        0        0      985 2024-04-22 12:24:45.000000 numpy4-0.5/numpy4/DC_RicartAgrawala.py
+-rw-rw-rw-   0        0        0     3564 2024-04-22 12:22:21.000000 numpy4-0.5/numpy4/DC_gc.py
+-rw-rw-rw-   0        0        0     1383 2024-04-22 12:22:55.000000 numpy4-0.5/numpy4/DC_globalAvg.py
+-rw-rw-rw-   0        0        0     1762 2024-04-22 12:19:22.000000 numpy4-0.5/numpy4/DC_ipc.py
+-rw-rw-rw-   0        0        0     2541 2024-04-22 12:25:26.000000 numpy4-0.5/numpy4/DC_loadBalancing.py
+-rw-rw-rw-   0        0        0       34 2024-04-22 12:25:53.000000 numpy4-0.5/numpy4/DC_multithreading.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy4-0.5/numpy4/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.976861 numpy4-0.5/numpy4.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 14:17:39.979862 numpy4-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      312 2024-04-23 14:16:51.000000 numpy4-0.5/setup.py
```

### Comparing `numpy4-0.2/numpy4/ADS_SMOTE.py` & `numpy4-0.5/numpy4/ADS_SMOTE.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/ADS_inferentialStats.py` & `numpy4-0.5/numpy4/ADS_inferentialStats.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/ADS_outlierDetection.py` & `numpy4-0.5/numpy4/ADS_outlierDetection.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/ADS_stats.py` & `numpy4-0.5/numpy4/ADS_stats.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,94 @@
 import pandas as pd
 import numpy as np
+# from google.colab import drive
+# drive.mount('/content/drive')
 
-df = pd.read_csv('./ADS Datasets/supermarket_sales - Sheet1.csv')
+
+df = pd.read_csv(f'/content/supermarket_sales - Sheet1.csv')
 df.head()
 
+
 #Mean SD LQ UQ max min
 df.describe()
 
+
 #Count of null values
 df.info()
 
+
 #Median
-df.median()
+df.select_dtypes(include=['number']).median()
+
 
 #Mode
 print(df['Product line'].mode())
 print(df['City'].mode())
 print(df['Payment'].mode())
 print(df['Customer type'].mode())
 print(df['Gender'].mode())
 
 
 #Scatter plot
 import matplotlib.pyplot as plt
 plt.scatter(df['Tax 5%'], df['Unit price'], c ="blue")
 
+
 import matplotlib.pyplot as plt
 plt.scatter(df['gross income'], df['Unit price'], c ="blue")
 
 import matplotlib.pyplot as plt
 plt.scatter(df['Quantity'], df['Total'], c ="blue")
 
-
 #Box plot
 x2=df['Tax 5%']
 x4=df['gross income']
-x5=df['Rating']  
+x5=df['Rating']
 data = pd.DataFrame({ "Tax 5%": x2,"gross income": x4,"Rating": x5})
 
 # Plot the dataframe
 ax = data[[ 'Tax 5%','gross income','Rating']].plot(kind='box', title='boxplot')
 
+
+
 plt.boxplot(df['Total'])
 
 
 #Trimmed mean
 from scipy import stats
 stats.trim_mean(df['Total'], 0.1)
 
+
 #Summation
-df['total'].sum()
+
+df['Total'].sum()
 
 #Frequency
 count = df['Product line'].value_counts()
 print(count)
 
 #Variance
-df.var()
+df.select_dtypes(include=['number']).var()
 
 #Correlation matrix
-df.corr()
+df.select_dtypes(include=['number']).corr()
 
 #Standard error of mean
-df.sem()
+df.select_dtypes(include=['number']).sem()
 
-#sum of squares 
+#sum of squares
 sos=0
 for val in df['Total']:
   sos=val*val+sos
 print(sos)
 
 #Skewness
-df.skew()
+df.select_dtypes(include=['number']).skew()
 
 #kurtosis
 sr = pd.Series(df['Total'])
 print(sr.kurtosis())
 
 import seaborn as sns
 
-g=sns.distplot(df['Total'])
+g=sns.distplot(df['Total'])
+
```

### Comparing `numpy4-0.2/numpy4/ADS_timeSeries.py` & `numpy4-0.5/numpy4/ADS_timeSeries.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/ADS_unsuperviseEval.py` & `numpy4-0.5/numpy4/ADS_unsuperviseEval.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/ADS_visualization.py` & `numpy4-0.5/numpy4/ADS_visualization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import pandas as pd
 import numpy as np
-from google.colab import drive
-drive.mount('/content/drive')
-df = pd.read_csv('/content/drive/My Drive/ADS/supermarket_sales - Sheet1.csv')
+# from google.colab import drive
+# drive.mount('/content/drive')
+df = pd.read_csv('ADS Datasets/supermarket_sales - Sheet1.csv')
 
 
 df.head()
 
 
 
 #Scatter plot
 import matplotlib.pyplot as plt
 plt.scatter(df['Tax 5%'], df['Unit price'], c ="blue")
 
 
 #BoxPlot
-x2=df['Tax 5%']
-x4=df['gross income']
-x5=df['Rating']  
-data = pd.DataFrame({ "Tax 5%": x2,"gross income": x4,"Rating": x5})
 
-# Plot the dataframe
-ax = data[[ 'Tax 5%','gross income','Rating']].plot(kind='box', title='boxplot')
+ax = df[[ 'Tax 5%','gross income','Rating']].plot(kind='box', title='boxplot')
+
 
 
 #Distribution Chart / Distplot
 import seaborn as sns
 
 g=sns.distplot(df['Total'])
 
@@ -43,22 +39,17 @@
 # Histogram
 df['Rating'].hist()
 plt.show()
 
 
 lst = df['Product line'].unique()
 print(lst)
-# t=[0,0,0,0,0,0]
-# for i in df:
-#   print(i)
-#   if i[5] in lst:
-#     if i[5]=='Health and beauty':
-#       t[0]=t[0]+i[9]
 
-# print(t)
+print(df[df['Product line']=='Electronic accessories'].count())
+
 
 t=[23,17,35,29,12,41]
 plt.pie(t,labels=lst,autopct ='% 1.1f %%', shadow = True)
 plt.show()
 
 
 #Density Chart
@@ -77,37 +68,40 @@
 data = df
 data.head(5)
 plt.figure(figsize=(15,5))
 sns.rugplot(data=data, x ="Total")
 plt.show()
 
 
+
 #column chart
 # plot between 2 attributes
 df1 = df.head(10)
 df1.plot.bar()
 plt.bar(df1['Gender'], df1['Total'])
 plt.xlabel("Gender")
 plt.ylabel("Total")
 plt.show()
 
 
+
 import plotly.express as px
 df1=df.head(15)
 fig = px.line(df1, x="Date", y="Total", color='City')
 fig.show()
 
 
 #Bubble Chart
 import plotly.express as px
 
 fig = px.scatter(df1, x="Total", y="Tax 5%", size="Quantity", color="City", hover_name="Product line", log_x=True, size_max=60)
 fig.show()
 
 
+
 #Parallel
 import plotly.express as px
 df1 =df.sample(n=100)
 fig = px.parallel_coordinates(df1, color="Total",
                               dimensions=['Quantity','Unit price','Rating',],
                               color_continuous_scale=px.colors.diverging.Tealrose,
                               color_continuous_midpoint=2)
@@ -122,14 +116,15 @@
 # plotting the Curve
 x.plot()
  
 # Display
 plt.show()
 
 
+
 import plotly.express as px
 
 # df = px.data.medals_wide(indexed=True)
 fig = px.imshow(df1)
 fig.show()
```

### Comparing `numpy4-0.2/numpy4/DC_Bankers.py` & `numpy4-0.5/numpy4/DC_Bankers.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_Berkley.py` & `numpy4-0.5/numpy4/DC_Berkley.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_Bully.py` & `numpy4-0.5/numpy4/DC_Bully.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_RaymondTree.py` & `numpy4-0.5/numpy4/DC_RaymondTree.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_RicartAgrawala.py` & `numpy4-0.5/numpy4/DC_RicartAgrawala.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_gc.py` & `numpy4-0.5/numpy4/DC_gc.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_globalAvg.py` & `numpy4-0.5/numpy4/DC_globalAvg.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_ipc.py` & `numpy4-0.5/numpy4/DC_ipc.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4/DC_loadBalancing.py` & `numpy4-0.5/numpy4/DC_loadBalancing.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.2/numpy4.egg-info/SOURCES.txt` & `numpy4-0.5/numpy4.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 setup.py
+numpy4/ADS_DataCleaning.py
 numpy4/ADS_SMOTE.py
-numpy4/ADS_dataCleaning.py
 numpy4/ADS_inferentialStats.py
 numpy4/ADS_outlierDetection.py
 numpy4/ADS_stats.py
 numpy4/ADS_superviseEval.py
 numpy4/ADS_timeSeries.py
 numpy4/ADS_unsuperviseEval.py
 numpy4/ADS_visualization.py
```

