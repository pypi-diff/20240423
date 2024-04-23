# Comparing `tmp/auto_vtna-1.0.2.tar.gz` & `tmp/auto_vtna-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_vtna-1.0.2.tar", last modified: Sat Apr 20 16:05:52 2024, max compression
+gzip compressed data, was "auto_vtna-1.0.3.tar", last modified: Tue Apr 23 18:17:08 2024, max compression
```

## Comparing `auto_vtna-1.0.2.tar` & `auto_vtna-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.677625 auto_vtna-1.0.2/
--rw-rw-rw-   0        0        0      539 2024-04-20 16:05:52.676535 auto_vtna-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.655546 auto_vtna-1.0.2/auto_vtna/
--rw-rw-rw-   0        0        0   139857 2024-04-20 15:39:25.000000 auto_vtna-1.0.2/auto_vtna/Auto_VTNA_GUI.py
--rw-rw-rw-   0        0        0    22228 2024-04-18 20:28:15.000000 auto_vtna-1.0.2/auto_vtna/Automatic_VTNA.py
--rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.2/auto_vtna/Normal_VTNA.py
--rw-rw-rw-   0        0        0    45282 2024-04-20 15:02:10.000000 auto_vtna-1.0.2/auto_vtna/VTNA_functions.py
--rw-rw-rw-   0        0        0    50480 2024-04-20 15:38:27.000000 auto_vtna-1.0.2/auto_vtna/__init__.py
--rw-rw-rw-   0        0        0     3110 2024-04-20 15:39:25.000000 auto_vtna-1.0.2/auto_vtna/running_codes 23dec.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.673532 auto_vtna-1.0.2/auto_vtna.egg-info/
--rw-rw-rw-   0        0        0      539 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-20 16:05:52.000000 auto_vtna-1.0.2/auto_vtna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 16:05:52.677625 auto_vtna-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      963 2024-04-20 15:01:17.000000 auto_vtna-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:08.283836 auto_vtna-1.0.3/
+-rw-rw-rw-   0        0        0      539 2024-04-23 18:17:08.282839 auto_vtna-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:08.228299 auto_vtna-1.0.3/auto_vtna/
+-rw-rw-rw-   0        0        0   201947 2024-04-23 13:54:59.000000 auto_vtna-1.0.3/auto_vtna/Auto_VTNA_GUI.py
+-rw-rw-rw-   0        0        0    22230 2024-04-21 08:40:37.000000 auto_vtna-1.0.3/auto_vtna/Automatic_VTNA.py
+-rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.3/auto_vtna/Normal_VTNA.py
+-rw-rw-rw-   0        0        0    45282 2024-04-20 15:02:10.000000 auto_vtna-1.0.3/auto_vtna/VTNA_functions.py
+-rw-rw-rw-   0        0        0    51883 2024-04-22 20:40:40.000000 auto_vtna-1.0.3/auto_vtna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:08.278001 auto_vtna-1.0.3/auto_vtna.egg-info/
+-rw-rw-rw-   0        0        0      539 2024-04-23 18:17:07.000000 auto_vtna-1.0.3/auto_vtna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-23 18:17:07.000000 auto_vtna-1.0.3/auto_vtna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:17:07.000000 auto_vtna-1.0.3/auto_vtna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-23 18:17:07.000000 auto_vtna-1.0.3/auto_vtna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-23 18:17:07.000000 auto_vtna-1.0.3/auto_vtna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:17:08.284836 auto_vtna-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      963 2024-04-23 18:16:20.000000 auto_vtna-1.0.3/setup.py
```

### Comparing `auto_vtna-1.0.2/PKG-INFO` & `auto_vtna-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vtna
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.2/auto_vtna/Auto_VTNA_GUI.py` & `auto_vtna-1.0.3/auto_vtna/Auto_VTNA_GUI.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,34 @@
 import matplotlib
 matplotlib.use('Qt5Agg')
 import matplotlib.pyplot as plt
 import auto_vtna
 import tkinter as tk
 from auto_vtna.Normal_VTNA import Normal_VTNA
 from auto_vtna.VTNA_functions import VTNA_omissions
-from auto_vtna.Automatic_VTNA import Automatic_VTNA
 import copy
 import re
+import os
 import csv
 import tkinter as tk
 from tkinter import scrolledtext
+from auto_vtna.VTNA_functions import VTNA_tT, on_click, VTNA_new, score_fit,data_scaling_y, origin_line, simple_line
+import itertools
+from functools import partial
+from openpyxl.drawing.image import Image
+from io import BytesIO
+import matplotlib.ticker as tkr
+import warnings
+import time
+from polyfit import PolynomRegressor, Constraints
+from num2words import num2words
+from scipy.optimize import curve_fit
+
+global cancel_calculation
+cancel_calculation=False
 
 def extract_range_info(values,data):
     '''Function used in the range mode data cropping window to extract 
     inputted value ranges.
     Arguments: 
      - values: data croppting range mode window inputs.
      - data: kinetic data dictionary.'''
@@ -97,15 +111,15 @@
     try:
         float_value = float(string)
         return True
     except ValueError:
         return False
 
 def overlay_plot(kinetic_data,experiments,NS_dict,output_reaction_species,tt_scaler=1,y_unit='M',\
-                 size_scaler=1,grid=False,title=None,fit_metric='RMSE',constraint='monotonic',\
+                 size_scaler=1,grid=False,title=None,fit_metric='RMSE',constraint='Monotonic',\
                  deg=5,show_fit_function=False,show_overlay_score=False,DP_scaler=1,xtick_rotation=0,\
                  show_legend=True,legend_outside=False,extra_legend=True,line_scaler=1,
                  tT_notation='Normal'):
     ''' Creates a VTNA_selection dictionary for the GUI settings stored in the arguments
     "experiments", "NS_dict" and "output_reaction_species", calculates the transformed time axis 
     for the kinetic data "kinetic_data" and generates the overlay plot for the selected plot settings.
     '''
@@ -117,23 +131,705 @@
     for i in experiments:
         VTNA_selection_dictionary['RM'][i]=Default_VTNA_selection_dictionary['RM'][i]
     # Update the normalised species and output species for generating the overlay plot based on GUI selections.
     VTNA_selection_dictionary['normalised_species']=NS_dict
     VTNA_selection_dictionary['output_species']=output_reaction_species
     # Calculate the normalised time axis using Normal_VTNA from auto_vtna.
     Run_VTNA=Normal_VTNA(kinetic_data,VTNA_selection_dictionary)
-    if constraint=='through origin':
+    if constraint=='Via origin':
         constraint='origin'
+    elif constraint=='Monotonic':
+        constraint='monotonic'
     # Generate the overlay plot.
     Run_VTNA.plot_VTNA_with_overlay_score(y_unit=y_unit,size_scaler=size_scaler,grid=grid, \
                   xaxis_size_scaler=tt_scaler,title=title,fit_metric=fit_metric,constraint=constraint,\
                   deg=deg,show_fit_function=show_fit_function,show_overlay_score=show_overlay_score,\
                     DP_scaler=DP_scaler,xtick_rotation=xtick_rotation,show_legend=show_legend,
                     legend_outside=legend_outside,extra_legend=extra_legend,linewidth=line_scaler,
                     xaxis_notation=tT_notation)
+class Automatic_VTNA:
+    def __init__(self,data,VTNA_selection,order_range=[-1.5,2.5],resolution=10,deg=5, \
+                 fit_metric='SE',iterations=4,constraint='monotonic',score_interval=0.15,\
+                fixed_order_species=None,initial_mesh_denser=True):
+        # Initialise the class:
+        self.data=data.copy()
+        self.VTNA_selection=VTNA_selection.copy()
+        self.order_range=order_range
+        self.resolution=resolution
+        self.deg=deg
+        self.fit_metric=fit_metric
+        self.iterations=iterations
+        self.constraint=constraint
+        self.score_interval=score_interval
+        self.fixed_order_species=fixed_order_species
+        self.initial_mesh_denser=initial_mesh_denser
+        # Perform automatic VTNA calculation:
+        Calculation_results = VTNA_orders(self.data,self.VTNA_selection, \
+        self.order_range,self.resolution,self.deg,self.fit_metric,self.iterations,self.constraint, \
+        self.score_interval,self.fixed_order_species,self.initial_mesh_denser)
+        if Calculation_results!=None:
+            self.results, self.best_orders, self.interval, self.best_slope=Calculation_results
+        else:
+            self.results=None
+
+    def identify_error_intervals(self,score_interval=0.15):
+        """
+        Generates a Pandas dataframe containing the lowest and highest order value which is found in the \
+        list of order value combinations that give an overlay score within "score_interval" of the optimal overlay \
+        score. The score_interval can be set to any value above 0. 
+        """
+        # Get the column names except the rightmost one
+        col_names = self.results.columns[:-1]
+        # Create an empty list to store lists of column values
+        combined_values = [[] for _ in range(len(self.results))]
+        # Iterate through each row of the DataFrame
+        for index, row in self.results.iterrows():
+            # Iterate through each column except the rightmost one
+            for col_name in col_names:
+                # Append the value of each column to the corresponding list
+                combined_values[index].append(row[col_name])
+        # Convert the list of lists into a numpy 2D array
+        order_combinations = np.array(combined_values)
+        # Extract the rightmost column as a numpy array
+        FQs = self.results.iloc[:, -1].values
+        # Obtain the minimum point order combination (minium FQ for variance, RMSE and SE, max FQ for R2).
+        minFQ=min(FQs)
+        if self.fit_metric=='R2':
+            minFQ=max(FQs)
+        # Identify order combinations with overlay scores up to "score_interval" higher than that of the best order:
+        if self.fit_metric=='R2':
+            good_order_combos=[order_combinations[i] for i in range(len(order_combinations)) if FQs[i]>minFQ*(1-score_interval)]
+        else: 
+            good_order_combos=[order_combinations[i] for i in range(len(order_combinations)) if FQs[i]<minFQ*(1+score_interval)]
+        # Identify the smallest and largest order values in the good order combinations list for each normalised species.
+        largest_values=[max(column) for column in zip(*good_order_combos)]
+        smallest_values=[min(column) for column in zip(*good_order_combos)]
+        intervals=list(zip(smallest_values, largest_values))
+        intervals=np.array(list(zip(smallest_values, largest_values)))
+        # Define a list of the normalised reaction species that haven't been fixed. 
+        if type(self.fixed_order_species)!=list:
+            fixed_order_list=[self.fixed_order_species]
+        else:
+            fixed_order_list=self.fixed_order_species
+        # Define the list of normalised species and generate the overlay score interval dictionary. 
+        normalised_species=[i for i in list(self.VTNA_selection['normalised_species'].keys()) if i not in fixed_order_list]
+        interval_dict={'Normalised species':normalised_species,f'Lower order limit {score_interval*100}%':intervals[:,0],f'Upper order limit {score_interval*100}%':intervals[:,1]}
+        return pd.DataFrame(interval_dict)
+
+    def plot_orders_vs_overlay(self,points=False,size_scaler=1,size_scaler2=1,title=None,zoom=False,grid=False,color_scaler=1,
+    fixed_cbar_resolution=None,interval=False,y_unit='M',title_fontsize=12,overlay_score_range_max=None,
+    overlay_score_range_min=None,show_legend_main=True,show_legend_popup=True,decimals_in_colorbar=3,annotate_optimum=True,
+    specified_score_interval=None):
+        """
+        Creates a graph or contour plot visualising the overlay score versus order value matrix \
+        for one and two normalised reaction species respectively. If the overlay score versus \
+        order value matrix involves 3 or more normalised species, no plot is created. The graph \
+        or contour plots can be clicked upon to generate the VTNA overlay plot corresponding to \
+        the order values of the click. 
+        Args:
+            points (bol): Set to True to visualise the order value data points for which overlay \
+            scores have been determined. 
+            size_scaler (int or float): Factor by which the size of the order value versus overlay \
+            score plot is adjusted. 
+            size_scaler2 (int or float): Factor by which the size of the VTNA overlay plot generated \
+            by clicking on the original plot is adjusted. 
+            title (str): The title of the order value versus overlay score plot.
+            zoom (int or float): Width of order values around the optimial order point that will be \
+            included in the order value versus overlay score plot.
+            grid (bol): Set to True to include a grid in the order value versus overlay score plot.
+            color_scaler (int or float, ∈<0,1]): Number between 1 and 0 which determines the factor by \
+            which the contour plot color bar range is truncated. NB: This will give white sections that \
+            are off the contour plot color map.
+            resolution_contour (float): Difference in overlay score between separate color shades in \
+            the contour plot. 
+            interval (bol): Set to True to show each order combination datapoint within the interval_score \
+            times the best overlay score value away from the optimal order value point. 
+            y_unit (str): The concentration unit of the output concentration profiles. Gets included in the \
+            yaxis title. 
+            title_fontsize (int): Fontsize of the title of the order value versus overlay score plot.
+            overlay_score_range_max (None or float): The maximum overlay score value to be shown in the plot \
+            either as a contour plot color bar (2 NS) or the y axis of an ordinary graph (1 NS).
+            overlay_score_range_min (None or float): The minimum overlay score value to be shown in the plot \
+            either as a contour plot color bar (2 NS) or the y axis of an ordinary graph (1 NS).
+            show_legend_main (bol): Set to True to show the legend of the overlay score versus order plot. 
+            show_legend_popup (bol): Set to True to show the legend of the VTNA overlay plots generated by \
+            mouseclicks on the overlay score versus order plot. 
+            decimals_in_colorbar (int): The number of decimals to be shown in the colorbar of an overlay score \
+            versus order contour plot. 
+            annotate_optimum (bol): Set to True to show the order values of the optimum point of an overlay score \
+            versus order contour plot. 
+
+        """
+        #if color_scaler>1 or color_scaler<=0:
+        #    raise ValueError('color_scaler should be set to ∈<0,1]')
+        # Find the species corresponding to the x or x and y axis:
+        axis_species=[i.replace('order in ','') for i in list(self.results.columns)[:-1]]
+        output_species=self.VTNA_selection['output_species']
+        analysis_columns=self.results.columns
+        no_normalised_species=len(analysis_columns)-1
+        # Create string to include information about reaction species with fixed order value(s) during the 
+        # automatic VTNA calculation.
+        fixed_order_string=''
+        if self.fixed_order_species!=None:
+            if type(self.fixed_order_species)==str:
+                fixed_order_string=fixed_order_string+f"\nFixed order for {self.fixed_order_species}: {self.VTNA_selection['normalised_species'][self.fixed_order_species]}"
+            else:
+                for i in self.fixed_order_species:
+                    fixed_order_string=fixed_order_string+f"\nFixed order for {i}: {self.VTNA_selection['normalised_species'][i]}."
+        if interval==True:
+            # Identify the score interval from the calculation or from the specified_score_interval argument.
+            score_interval=self.score_interval
+            if specified_score_interval!=None:
+                if float(specified_score_interval)>0:
+                    score_interval=float(specified_score_interval)
+                else:
+                    warnings.warn("The specified score interval must be a number above 0. The calculation value will be used instead.")
+        if no_normalised_species>2:
+            return ValueError('The overlay score : order value matrix can only be visualized for 1 or 2 varying normalised reaction species.')
+        if no_normalised_species==1:
+            x_best=self.best_orders[0]
+            # Define x values as orders and y values as fit metric values.
+            x_s=np.array(self.results[analysis_columns[0]])
+            y_s=np.array(self.results[analysis_columns[1]])
+            # Sort the order values from smallest to largest to get one continuous plt line. 
+            xy=list(itertools.zip_longest(x_s,y_s))
+            xy.sort()
+            # Redefine sorted x and y values
+            y=[y[1] for y in xy]
+            x=[x[0] for x in xy]
+            # Find the finest orders interval used to find minimum point
+            resolution_orders=str(format(x_s[-1]-x_s[-2],".12f"))
+            # Find the index for first non 0 digit in resolution
+            for i in range(len(resolution_orders)):
+                if resolution_orders[i]!='.' and resolution_orders[i]!='0':
+                    break
+            # Increase i by 1 if first character in order is '-'
+            if str(x_best)[0]=='-':
+                i=i+1
+            # Create figure with size scaled by size_scaler
+            fig, ax = plt.subplots(figsize=(6*size_scaler,4*size_scaler))
+            # Plot the fit metric values obtained at each order.
+            ax.plot(x,y,marker='o',linestyle='-',markersize=5)
+            # Plot the minimum point and insert label information for legend.
+            minimum_info=f'Best order: {f"%.{i-1}f" % round(x_best,i-1)}\nUncertainty: {f"%.{i}f" % round(float(resolution_orders[:(i+2)]),i)}\nMinimum {self.fit_metric}: {f"%.{i+2}f" % round(min(y),i+2)}'
+            optimum_value=min(y)
+            if self.fit_metric=='R2':
+                minimum_info=f'Best order: {f"%.{i-1}f" % round(x_best,i-1)}\nUncertainty: {f"%.{i}f" % round(float(resolution_orders[:(i+2)]),i)}\nMaximum {self.fit_metric}: {f"%.{i+2}f" % round(max(y),i+2)}'
+                optimum_value=max(y)
+            minimum_info=minimum_info+fixed_order_string
+            plt.plot(x_best,optimum_value,color='orange',marker='o',label=minimum_info)
+            # Define the x and y axis labels. 
+            ax.set_xlabel(f'{analysis_columns[0]}',fontsize=12)
+            ax.set_ylabel(f'Overlay score: {self.fit_metric}',fontsize=12)
+            # Change the x- and y-axis limits in case zoom has been applied. 
+            if zoom!=False:
+                x1=x_best-zoom/2
+                x2=x_best+zoom/2
+                plt.xlim(x1,x2)
+                y2=[i for i in y if x[y.index(i)]<x2 and x[y.index(i)]>x1]
+                y1=min(y2)
+                y2=max(y2)
+                leeway=(y2-y1)*0.1
+                ax.set_ylim(y1-leeway,y2+leeway)
+            # Plot a horizontal line showing the datapoints within the interval_score*best overlay score range of the minimum point.
+            if interval==True:
+                interval_limit=min(y)+min(y)*score_interval
+                if self.fit_metric=='R2':
+                    interval_limit=max(y)-max(y)*score_interval
+                ax.plot([self.order_range[0],self.order_range[1]],[interval_limit,interval_limit],linestyle='--',label=f"{float(score_interval)*100}% from optimal point.")
+            # Set the figure title. 
+            if title==None:
+                fig.suptitle(f'VTNA overlay score versus orders for the formation of {output_species}',fontsize=title_fontsize,y=0.95)
+            else:
+                fig.suptitle(title,fontsize=title_fontsize,y=0.95)
+            # Apply legend and grid if selected.
+            if show_legend_main:
+                ax.legend()
+            if grid==True:
+                plt.grid()
+            # Define the ylimits if overlay score range max or min have been defined. 
+            if overlay_score_range_max!=None:
+                ax.set_ylim(top=overlay_score_range_max)
+            if overlay_score_range_min!=None:
+                ax.set_ylim(bottom=overlay_score_range_min)
+        # Code for contour plot to illustrate the overlay score across order values if there are 2 normalised species. 
+        if no_normalised_species==2:
+            # Obtain the order value arrays x_s and y_s and the overlay scores z_s.
+            z_s=np.array(self.results[analysis_columns[2]])
+            x_s=np.array(self.results[analysis_columns[0]])
+            y_s=np.array(self.results[analysis_columns[1]])
+            # Define the x and y values of the minimum point (or maximum for R2).
+            x_best=self.best_orders[0]
+            y_best=self.best_orders[1]
+            # Create figure with size scaled by size_scaler.
+            fig, ax = plt.subplots(figsize=(6*size_scaler,5*size_scaler))
+            # Identify the max and min fit metric values for setting up color grid for contour plot.
+            min_z=min(z_s)
+            max_z=max(z_s)
+            # Find the finest orders interval used to find minimum point.
+            resolution_orders=str(format(y_s[-1]-y_s[-2],".12f"))
+            # Find the index for first non 0 digit in resolution_orders.
+            for i in range(len(resolution_orders)):
+                if resolution_orders[i]!='.' and resolution_orders[i]!='0':
+                    break
+            # Define q and w to determine number of digits to show for each minimum point order.
+            q,w=i,i
+            # Increase q and w by 1 if first character in respective order is '-'
+            if str(x_best)[0]=='-':
+                q=1+i
+            if str(y_best)[-1]=='-':
+                w=1+i
+            if points==True:
+                # Plot the data points used to generate the countour plot.
+                ax.plot(x_s,y_s,'or',markersize=0.5)
+            # Plot the datapoints with an overlay score off the minimum point (or max for R2) score.
+            
+            if interval==True:
+                if self.fit_metric!='R2':
+                    x_interval=[x_s[i] for i in range(len(x_s)) if z_s[i]<(score_interval+1)*min(z_s)]
+                    y_interval=[y_s[i] for i in range(len(y_s)) if z_s[i]<(score_interval+1)*min(z_s)]
+                else:
+                    x_interval=[x_s[i] for i in range(len(x_s)) if z_s[i]>(-score_interval+1)*min(z_s)]
+                    y_interval=[y_s[i] for i in range(len(y_s)) if z_s[i]>(-score_interval+1)*min(z_s)]
+                # Plot the identified interval datapoints in green.
+                ax.plot(x_interval,y_interval,markersize=0.7,linestyle='',marker='x',color='b',  
+                        label=f'Orders within {score_interval*100}% of optimal O.S.',zorder=2)
+            # Print axis labels with species_order from data to assign normalised species.
+            ax.set_xlabel(f'{analysis_columns[0]}')
+            ax.set_ylabel(f'{analysis_columns[1]}')
+            # Plot the data point corresponding to the best VTNA alignment and use label to provide information.
+            if self.fit_metric=='R2':
+                ax.plot(x_best,y_best,marker='x',color='k',linestyle='',label = f'Best orders: ({round(x_best, q-1):.{int(q-1)}f},{round(y_best, w-1):.{int(w-1)}f})\nUncertainty: {resolution_orders[:(i+2)]}\nMaximum {self.fit_metric}: {round(max(z_s), i+2):.{int(i+2)}f}{fixed_order_string}')
+            else:
+                ax.plot(x_best,y_best,marker='x',color='k',linestyle='',label=f'Best orders: ({round(x_best, q-1):.{int(q-1)}f},{round(y_best, w-1):.{int(w-1)}f})\nUncertainty: {resolution_orders[:(i+2)]}\nMinimum {self.fit_metric}: {round(min(z_s), i+2):.{int(i+2)}f}{fixed_order_string}')
+            # If zoom argument applied, apply xlim and ylim around the minimum point and find the lowest z_value in that interval.
+            min_z=min(z_s)
+            max_z=max(z_s)
+            z_range=max_z-min_z
+            max_z=max(z_s)-z_range*(1-color_scaler)
+            # If the overlay score range max or min arguments have been defined, prepare the relevant variables.
+            cbar_fixing=False
+            if overlay_score_range_max!=None:
+                cbar_fixing=True
+                max_z=overlay_score_range_max
+            if overlay_score_range_min!=None:
+                cbar_fixing=True
+                min_z=overlay_score_range_min
+            if zoom!=False:
+                if cbar_fixing==True:
+                    warnings.warn("overlay_score_range_max and overlay_score_range_min is ignored when zoom isn't set to False.")
+                # Define x and y limits to zoom in closer to the minimum point
+                min_z=min(z_s)
+                ax.set_xlim(x_best-zoom/2,x_best+zoom/2)
+                ax.set_ylim(y_best-zoom/2,y_best+zoom/2)
+                # Obtain the z_s values in the new domain.
+                z_s2=[i for i in z_s if x_s[list(z_s).index(i)]<(x_best+zoom/2) and x_s[list(z_s).index(i)]>(x_best-zoom/2) \
+                       and y_s[list(z_s).index(i)]<(y_best+zoom/2) and y_s[list(z_s).index(i)]>(y_best-zoom/2)] 
+                # Define the maximum fit metric value in this interval and the difference between this and the minimum value
+                max_z=max(z_s2)
+                z_range=max_z-min_z
+                # Use color_scaler to define to adjust the maximum value of the colorbar
+                max_z=max_z-z_range*(1-color_scaler)
+            # Define the order value range of the plot
+            delta_order=max(x_s)-min(x_s)
+            # Define appropriate colorbar values if R2 is used as fit metric
+            if self.fit_metric=='R2':
+                max_z=max(z_s)
+                max_z=max_z+(1-max_z)*0.2
+                min_z=min_z+z_range*(1-color_scaler)
+            if fixed_cbar_resolution!=None:
+                resolution_cbar=float(fixed_cbar_resolution)
+            else:
+                resolution_cbar=abs((max_z-min_z)/30)
+            clev = np.arange(min_z,max_z,resolution_cbar)
+            # Create contour plot.
+            CS = ax.tricontourf(x_s, y_s, z_s, clev,cmap=plt.cm.viridis_r)
+            if self.fit_metric=='R2':
+                CS = ax.tricontourf(x_s, y_s, z_s, clev,cmap=plt.cm.viridis)
+            cbar=fig.colorbar(CS,orientation='vertical',label=f'Overlay score: {self.fit_metric}',ax=ax,format=tkr.FormatStrFormatter(f'%.{decimals_in_colorbar}g'))
+            legend_loc='best'
+            if zoom==False:
+                best_value_x=x_best+0.045
+                best_value_y=y_best+0.045
+                if best_value_y-min(y_s)<best_value_y-max(y_s):
+                    legend_loc='upper '
+                else: 
+                    legend_loc='lower '
+                if best_value_x-min(x_s)<best_value_x-max(x_s):
+                    legend_loc=legend_loc+'right'
+                else:
+                    legend_loc=legend_loc+'left'
+            if show_legend_main:
+                ax.legend(loc=legend_loc)
+            # Define the title of the figure.
+            if title==None:
+                fig.suptitle(f'VTNA overlay score versus orders for the formation of {output_species}',fontsize=title_fontsize,y=0.95)
+            else:
+                fig.suptitle(title,fontsize=title_fontsize,y=0.95)
+            # Annotate the minimum point to show its order values. 
+            # Adjust position according to the "zoom" value and delta_order if zoom isn't set to False
+            if annotate_optimum:
+                if zoom!=False:
+                    ax.annotate(f'{f"%.{q}f" % round(x_best,q)}, {f"%.{w}f" % round(y_best,w)}',(x_best+0.045*zoom/delta_order, y_best+0.045*zoom/delta_order))
+                if zoom==False:
+                    ax.annotate(f'{f"%.{q}f" % round(x_best,q)}, {f"%.{w}f" % round(y_best,w)}',(best_value_x,best_value_y))
+        # Create a new click function with inputs.
+        on_click_with_inputs = partial(on_click,data=self.data,VTNA_selection=self.VTNA_selection,y_unit=y_unit,\
+        size_scaler=size_scaler2,fit_metric=self.fit_metric,deg=self.deg,constraint=self.constraint,fixed_order_species=self.fixed_order_species,
+        axis_species=axis_species,show_legend=show_legend_popup)
+        # Bind the on_click function to the mouse click event.
+        cid = fig.canvas.mpl_connect('button_press_event', on_click_with_inputs)
+        # Show the plot.
+        plt.tight_layout()
+        if grid==True:
+            plt.grid()
+        image_stream = BytesIO()
+        plt.savefig(image_stream, format='png', bbox_inches='tight', pad_inches=0)
+        image_stream.seek(0)
+        img = Image(image_stream)
+        plt.show()
+        return img
+
+def VTNA_orders(data,VTNA_selection,order_range=[-1.5,2.5],resolution=8,deg=5,fit_metric='RMSE',iterations=6,constraint='monotonic',
+                score_interval=0.15,fixed_order_species=None,initial_mesh_denser=True):
+        """
+        Calculates the overlay score across different reaction order values for each normalised species in the \
+        VTNA_selection dictionary for the kinetic data "data". First, a uniform order grid is defined by the order_range and \
+        resolution arguments. Then, VTNA_omissions is applied to remove experiments or datapoints within experiments \
+        as defined in VTNA_selection. Next, the average output species concentration profiles are normalised to \
+        1. Then, numpy arrays containing the data required for variable time normalisation using the trapezoid \
+        rule is defined with padding to ensure compatibility with numpy and inputed to explore_orders() to calculate \
+        the overlay score for each order combination by calculating the normalised time axis with VTNA_tT() \
+        and performing a global fit of each time normalised output concentration profile with a fitting method defined by \
+        keyword arguments "deg" and "constraint". Explore_orders() then returns the overlay scores, each order combination \
+        investigated and the best order combination overall. Next, another order grid with values around each minimum order value \
+        is defined and explored by explore_orders() which calculates the overlay score for each combination. The new minimum \
+        point is then used to define an even more fine order combination grid which is again given to explore_orders(). This \
+        is repeated "iterations" number of time to improve the precision of the assigned order values. In the end, a \
+        pandas DataFrame conatining the order values for each normalised species and the resulting overlay scores is \
+        returned with the best order values and the intervals within which the overlay score deviates from the optimum \
+        value by a factor of less than the "score_interval" value and the best order values found.
+        Args:
+            data (dict): Kinetic data as a dictionary of Pandas dataframes.
+            VTNA_selection (dict): Dictionary containing information about how to carry out automatic VTNA.
+            order_range (list): Minimum and maximum order value used to define the initial order value grid. 
+            resolution (int): Number of datapoints included in the order value grids in each explore_orders() iteration.
+            deg (int): Polynomial degree used in the global fitting prodecure to calculate the overlay score. 
+            fit_metric (str): Goodness-of-fit metric chosen to define the overlay score value. Either 'R2', 'RMSE' or 'SE'. \
+            otherwise variance is used.
+            iterations (int): The number of times explore_orders() is called after the first order grid has been investigated.
+            constraint (str): Defines the constraint of the global fit used by explore_orders() to calculate the overlay score. \
+            Can be set to 'monotonic' for monotonic fitting (default), None for ordinary polynomial fitting or 'origin' for \
+            linear fit through origin.
+            score_interval: Defines the cutoff minimum_overlay_score + minimum_overlay_score*score_interval (max for R2) for \
+            quoting the range of order values that give overlay scores close to that of the best order values to quantify how \
+            well defined best order values are. 
+            fixed_order_species (list or None): List containing the normalised reaction species for which \
+            time axis should be normalised with a fixed value (as defined in the VTNA selection dictionary). \
+            This can be done to lower the dimensionality of the overlay score versus order matrix. 
+            initial_mesh_denser (bol): Determines whether the initial order value mesh should be denser than the \
+            resolution argument by a factor of 1.5 (True) or the same as the resolution parameter (False).
+        """
+        # Check that the constraint argument is specified correctly.
+        if constraint!=None and constraint!='origin' and constraint!='monotonic':
+            raise ValueError("Constraint can only be set to 'origin' for linear fit through origin, 'monotonic' for \
+                          monotonic fit or None for ordinary polynomial fit")
+        # Check the intial time:
+        start_time=time.time()
+        print('Auto-VTNA calculation underway.')
+        # Check if the number of fixed order species is greater than the number of normalised reaction species.
+        if fixed_order_species!=None:
+            no_fixed_order_species=len(fixed_order_species)
+            if type(fixed_order_species)==str:
+                no_fixed_order_species=1
+            if no_fixed_order_species>=len(VTNA_selection['normalised_species'].items()):
+                raise ValueError("The number of fixed order species can't be the same as or lower than the \
+    number of normalised reaction species in the VTNA selection dictionary.")
+        # Obtain deepcopy of the kinetic data and VTNA selection dictionary to avoid alterations. 
+        data_copy=copy.deepcopy(data)
+        selection_copy=copy.deepcopy(VTNA_selection)
+        # Access one of the experimental dataframes.
+        example_RM=list(data_copy.keys())[0]
+        # Define the time axis key as t.
+        t=data_copy[example_RM].keys()[0] 
+        # Use the selected resolution and order range to define a list of order combinations. 
+        # Resultion is increased by 50% for the first order exploration.
+        if initial_mesh_denser:
+            resolution_scaler=1.5
+        else:
+            resolution_scaler=1
+        orders=np.linspace(order_range[0],order_range[1],round(resolution*resolution_scaler))
+        # Edit the kinetic data according to the VTNA selection dictionary and add a scaled output values column.
+        data_omissions=VTNA_omissions(data_copy,selection_copy)
+        data_scaled=data_scaling_y(data_omissions,selection_copy)
+        # Collect the time, normalised species and output species concentration data into designated lists.
+        output_lists=[]
+        NS_lists=[]
+        time_lists=[]
+        normalised_species=list(selection_copy['normalised_species'].keys())
+        # Check that the reaction species listed in 'fixed_order_species' are present as normalised reaction 
+        # species in the VTNA selection dictionary. Remove these reaction species from the normalised_species list. 
+        if fixed_order_species!=None:
+            # Make fixed_order_species into a list if only one reaction species string is defined. 
+            if type(fixed_order_species)==str:
+                fixed_order_species=[fixed_order_species]
+            # Cancel calculation if fixed order reaction species have been selected that are not defined
+            # as normalised reaction species in the VTNA selection dictionary. 
+            if all(species in normalised_species for species in fixed_order_species)!=True:
+                raise ValueError("All reaction species listed in 'fixed_order_species' must be present as a normalised \
+                species in the selection dictionary")
+            # Remove the fixed reaction species from the normalised_species list.
+            normalised_species=[i for i in normalised_species if i not in fixed_order_species]
+            # Generate a list of the fixed order values from the VTNA selection dictionary. 
+            fixed_orders=[selection_copy['normalised_species'][i] for i in fixed_order_species]
+            NS_lists_fixed_orders=[]
+        # Find the number of normalised species and add a duplicate of orders to order_combinations for each.
+        no_orders=len(normalised_species)
+        order_combinations=[]
+        for i in range(no_orders):
+            order_combinations.append(orders)
+        # Obtain the names of the experiment datasets in the data dictionary.
+        experiments=list(data_copy.keys())
+        # If selected experiments are defined in the selection dictionary, use these experiment names instead.
+        if 'RM' in list(selection_copy.keys()):
+            experiments=list(selection_copy['RM'].keys())
+        # Extract the information required for time variable normalisation and fitting across order combinations. 
+        counter=0
+        for i in normalised_species:
+            NS_nested_list=[]
+            for exp in experiments:
+                # Obtain the concentration profiles for each of the normalised reaction species i from each experiment exp.
+                NS_nested_list.append(list(data_scaled[str(exp)][i].to_numpy()))
+                # Collect the time and scaled output concentration values for each experiment once. 
+                if counter==0:
+                    time_lists.append(list(data_scaled[str(exp)][t].to_numpy()))
+                    output_lists.append(list(data_scaled[str(exp)]['output_scaled'].to_numpy()))
+            counter=1
+            NS_lists.append(NS_nested_list)
+        # Extract the integral factors from the kinetic data for the normalised reaction species with fixed order values. 
+        if fixed_order_species!=None:
+            counter=0
+            for i in fixed_order_species:
+                NS_nested_list_fixed_orders=[]
+                for exp in experiments:
+                    # Obtain the concentration profiles for each of the normalised reaction species i from each experiment exp.
+                    NS_nested_list_fixed_orders.append(list(data_scaled[str(exp)][i].to_numpy()))
+                NS_lists_fixed_orders.append(NS_nested_list_fixed_orders)
+        # Find the number of time points for the kinetic data of each experiment.
+        dimensions=[len(l) for l in time_lists]
+        # Make the time and normalised species concentration lists from each experiment the same length by padding with 1.
+        # Padding is done with 1 rather than 0 to avoid warning messages from trying to raise 0 to negative powers. 
+        if all(l==dimensions[0] for l in dimensions)==False:
+            max_dim=max(dimensions)
+            # Add 0 to the end of each time list which is shorter than the longest list.
+            time_lists = [sublist + [1] * (max_dim - len(sublist)) for sublist in time_lists]
+            # For each nested list containing the concentration profiles for a given normalised species across all experiments, perform padding. 
+            for nl in range(len(NS_lists)):
+                NS_lists[nl]=[sublist + [1] * (max_dim - len(sublist)) for sublist in NS_lists[nl]]
+            if fixed_order_species!=None:
+                # For each nested list containing the concentration profiles for a given normalised species with fixed reaction orders 
+                # across all experiments, perform padding. 
+                for nl in range(len(NS_lists_fixed_orders)):
+                    NS_lists_fixed_orders[nl]=[sublist + [1] * (max_dim - len(sublist)) for sublist in NS_lists_fixed_orders[nl]]
+        # Now that the time and normalised species lists are padded, they are converted into 2d and 3d arrays respectively. 
+        NS_lists=np.array(NS_lists)
+        # Use the convolve function for each 2d array in the 3d array to obtain the average normalised species raised to their respective order values.
+        dNS_lists=np.apply_along_axis(lambda x: np.convolve(x, [0.5,0.5], mode='valid'), axis=-1, arr=NS_lists)
+        time_lists=np.array(time_lists)
+        # Obtain the dt values for each time list.
+        dt_lists=np.diff(np.array(time_lists), axis=1)
+        # Multiply each dt with the integral fastors from the fixed reaction order reaction species. 
+        if fixed_order_species!=None:
+            NS_lists_fixed_orders=np.array(NS_lists_fixed_orders)
+            # Turn zeros into very small values to avoid errors. 
+            dNS_lists_fixed_orders=np.apply_along_axis(lambda x: np.convolve(x, [0.5,0.5], mode='valid'), axis=-1, arr=NS_lists_fixed_orders)
+            order_array=np.array(fixed_orders)[:, np.newaxis,np.newaxis]
+            # Raise the concentration values of each experiment dataset's normalised species. 
+            dNS_lists_fixed_orders_updated=np.power(dNS_lists_fixed_orders, order_array)
+            # Multiply together the 2d normalised species arrays and then multiply with the dt values.
+            dt_lists=np.apply_along_axis(lambda x: np.prod(x, axis=0), axis=0, arr=dNS_lists_fixed_orders_updated)*dt_lists
+        # Access the output concentration data of the first experiment to judge if increasing or decreasing monotonic fitting should be applied. 
+        fit_direction='inc'
+        if (output_lists[0][0]-output_lists[0][-1])>0:
+            fit_direction='dec'
+        # Perform first order exploration using "orders". 
+        exploration1=explore_orders(dt_lists,output_lists,dNS_lists,dimensions,order_combinations,fit_metric,deg,constraint,fit_direction)
+        if exploration1==None:
+            return None
+        best_orders=exploration1[-1]
+        print(f'Best reaction order(s) from the 1st order exploration: {best_orders}')
+        # Save the order combination tuples and overlay scores obtained in the first order exploration.
+        FQs=exploration1[0]
+        order_combinations=exploration1[1]
+        # The zoom factor is defined as 140% of the difference between adjacent orders in the first reaction order grid applied if resolution>5. 
+        # If the resolution is 4 or 5, the zoom factor is defined as the 110% and 120% of the difference between adjacent orders.  
+        mesh_resolution=abs(orders[0]-orders[1])
+        multipliers = {x: 1.1 if x == 4 else 1.2 if x == 5 else 1.4 for x in range(4, 10000)}
+        zoom_factor=mesh_resolution*multipliers[resolution]
+        # Perform a number of additional order explorations given by "interations" to increase the precision of the optimal orders. 
+        for i in range(iterations):
+            # Define resolution 2 to alternate between odd and even number of values in order value mesh.
+            if i//2*2==i:
+                resolution2=resolution+1
+            else:
+                resolution2=resolution
+            orders_new=[]
+            # Define a new set of order combinations arround the optimal order values from the first order exploration. 
+            for k in range(no_orders):
+                orders_new.append(np.linspace(best_orders[k]-zoom_factor,best_orders[k]+zoom_factor,resolution2))
+            # Perform new order exploration of the new order value combinations. 
+            exploration=explore_orders(dt_lists,output_lists,dNS_lists,dimensions,orders_new,fit_metric,deg,constraint,fit_direction)
+            if exploration==None:
+                return None
+            best_orders=exploration[-1]
+            print(f'Best reaction order(s) from the {num2words(i+2, to="ordinal_num")} order exploration: {best_orders}')
+            # Add datapoints from the latest order exploration to the FQ and order_combinations list. 
+            FQs=FQs+exploration[0]
+            order_combinations=order_combinations+exploration[1]
+            # Define the new zoom factor as before to increase the fineness of the subsequent order value grid. 
+            mesh_resolution=abs(exploration[1][-1][-1]-exploration[1][-2][-1])
+            zoom_factor=mesh_resolution*multipliers[resolution+1 if resolution2==resolution else resolution]
+        # Obtain the minimum point order combination (minium FQ for variance, RMSE and SE, max FQ for R2).
+        minFQ=min(FQs)
+        if fit_metric=='R2':
+            minFQ=max(FQs)
+        index_best_order=FQs.index(minFQ)
+        best_orders_3=order_combinations[index_best_order]
+        # Identify order combinations with overlay scores up to "score_interval" higher than that of the best order:
+        if fit_metric=='R2':
+            good_order_combos=[order_combinations[i] for i in range(len(order_combinations)) if FQs[i]>minFQ*(1-score_interval)]
+        else: 
+            good_order_combos=[order_combinations[i] for i in range(len(order_combinations)) if FQs[i]<minFQ*(1+score_interval)]
+        # Identify the smallest and largest order values in the good order combinations list for each normalised species.
+        largest_values=[max(column) for column in zip(*good_order_combos)]
+        smallest_values=[min(column) for column in zip(*good_order_combos)]
+        intervals=list(zip(smallest_values, largest_values))
+        intervals=np.array(list(zip(smallest_values, largest_values)))
+        interval_dict={'Normalised species':normalised_species,f'Lower order limit {score_interval*100}%':intervals[:,0],f'Upper order limit {score_interval*100}%':intervals[:,1]}
+        # Create Dataframe for overlay scores against reaction order values.
+        result_dict={}
+        order_combinations_array=np.array(order_combinations)
+        for i in range(len(normalised_species)):
+            result_dict[f'order in {normalised_species[i]}']=order_combinations_array[:,i]
+        result_dict[f'{fit_metric} overlay score']=FQs
+        # Check the final time and print the time taken for the calculation
+        end_time=time.time()
+        total_time=end_time-start_time
+        print(f'The calculation is complete. Time elapsed: {round(total_time,1)} seconds')
+        # If the fit degree is set to 0, find the slope of the fit when optimal order values are applied. 
+        # The x and y axis are not scaled.
+        slope=None
+        if deg==1:
+            counter=0
+            # Update the selection dictonary with the best reaction order values. 
+            for species in normalised_species:
+                if type(fixed_order_species)==list:
+                    if species in fixed_order_species:
+                        continue
+                selection_copy["normalised_species"][species]=float(best_orders_3[counter])
+                counter+=1
+            output_species=selection_copy['output_species']
+            tables=VTNA_new(data_copy,selection_copy)
+            Data_points_y=[]
+            Data_points_t=[]
+            # Collect all the non-scaled datapoints from the normal VTNA calculation. 
+            for i in tables.keys():
+                x_values=[float(j) for j in tables[i]['tT'].to_numpy()]
+                Data_points_t=Data_points_t+x_values
+                ys=[float(j) for j in tables[i][output_species].to_numpy()]
+                Data_points_y=Data_points_y+ys
+            # Perform the linear fit to determine the slope of the fitted line.  
+            if constraint=='origin':
+                params = curve_fit(origin_line, Data_points_t, Data_points_y)
+                slope=params[0][0]
+            else:
+                polyfit=np.polyfit(Data_points_t,Data_points_y,deg=deg)
+                slope=polyfit[0] 
+        return pd.DataFrame(result_dict),best_orders_3,pd.DataFrame(interval_dict),slope
+
+def explore_orders(dt_lists,output_lists,dNS_lists,dimensions,orders,fit_metric,deg,constraint,fit_direction):
+    """
+    Calculates the normalised time axis of each order combination by calling VTNA_tT() with the \
+    condensed kinetic data NS_lists and time_lists. Then performs the specified global fitting \
+    procedure to calculate the overlay score as the goodness of fit measure "fit_metric". Returns \
+    the overlay scores, order combinations and the order combination giving the best overlay score. 
+    Args:
+        time_lists (list of lists): Padded list containing time points from each experiment.
+        output_lists (list of lists): List containing lists of output concentration profiles from each experiment. 
+        NS_lists (list of list of lists): List containing the lists of padded concentration profile lists for \
+        each normalised reaction species for each experiment.
+        Dimensions (list of int): The number of rows in the DataFrame of each experiment in "data". Used to remove padded values. 
+        orders (list of numpy arrays): List of numpy arrays containing the order values to be investigated for each \
+        normalised reaction species.
+        fit_metric (str): Goodness-of-fit metric chosen to define the overlay score value. Either 'R2', 'RMSE' or 'SE'. \
+        otherwise variance is used.
+        deg (int): Polynomial degree used in the global fitting prodecure to calculate the overlay score. 
+        constraint (str): Defines the constraint of the global fit used by explore_orders() to calculate the overlay score. \
+        Can be set to 'monotonic' for monotonic fitting (default), None for ordinary polynomial fitting or 'origin' for \
+        linear fit through origin.
+        fit_direction (str): The direction of the monotonic fitting procedure, either "inc" or "dec" as determined in \
+        VTNA_orders()
+    """
+    # Define the cancel_calculation as global
+    global cancel_calculation
+    # Nested function for calculating the normalised time axis
+    if constraint=='monotonic':
+        # Prepare "polyestimator" for performing monotonic fit with selected degree.
+        polyestimator = PolynomRegressor(deg=deg, regularization = None, lam = 0)
+        monotone_constraint = Constraints(monotonicity=fit_direction)
+    # Define accumulator for goodness of fit measures.
+    FQs=[]
+    # Get every combination of orders as list of tuples.
+    order_pairs=list(itertools.product(*orders))
+    # Collapse the output list of lists to use in fitting.
+    y=list(itertools.chain(*output_lists))
+    for i in order_pairs:
+        if cancel_calculation==True:
+            cancel_calculation=False
+            print("Calculation interrupted by user.")
+            return None
+        # Obtain the normalised time axis by calling VTNA_tT().
+        tT=VTNA_tT(dt_lists,dNS_lists,i).tolist()
+        # conncatenate the list of transformed time axis lists while removing padded values using the dimensions list 
+        tT=list(itertools.chain(*[tT[i][:dimensions[i]] for i in range(len(dimensions))]))
+        # Perform the polynomial fit of "deg" order using the specified fit method and evaluate fitted function at the relevant "tT" values. 
+        # Then evaluate the goodness-of-fit by the selected fit metric and add it to the FQs list.
+        if constraint=='origin':
+            tT_2=[i/max(tT) for i in tT]
+            if deg==1:
+                params = curve_fit(origin_line, tT_2, y)
+                a=params[0]
+                y_pred=a*tT_2
+                a
+            else:
+                print('for fit through zero, use deg=1')
+                return 
+            FQ=score_fit(y,y_pred,fit_metric)
+            FQs.append(FQ)
+        if constraint=='monotonic': 
+            tT_2=np.array([i/max(tT) for i in tT]).reshape((-1,1))    
+            polyestimator.fit(tT_2, y, loss = 'l2', constraints={0: monotone_constraint})       
+            pred_y = polyestimator.predict(tT_2)
+            # Call the score_fit function to evalue the goodness-of-fit using the fit measurement "fit_metric".
+            FQ=score_fit(y,pred_y,fit_metric)
+            FQs.append(FQ)
+        if constraint==None:
+            tT_2=[i/max(tT) for i in tT]
+            polyfit=np.polyfit(tT_2,y,deg=deg)
+            pred_y=np.polyval(polyfit,tT_2)
+            FQ=score_fit(y,pred_y,fit_metric)
+            FQs.append(FQ)
+    # Obtain the best fit metric value (min for SE, RMSE and variance, max for R2)
+    minFQ=min(FQs)
+    if fit_metric=='R2':
+        minFQ=max(FQs)
+    # Identify the reaction orderds corresponding to the order minimum point
+    index_best_order=FQs.index(minFQ)
+    best_orders=order_pairs[index_best_order]
+    return FQs, order_pairs, best_orders
     
 class CalculationThread(threading.Thread):
 # NB: this class function was created and annotated using OpenAI's ChatGTP. 
     def __init__(self, target, args=()):
         # Initialize the thread with a target function and its arguments
         super().__init__(target=target, args=args)
         # Initialize a variable to store the result of the calculation
@@ -148,29 +844,37 @@
             if self._target:
                 # Call the target function with its arguments and store the result
                 self._result = self._target(*self._args, **self._kwargs)
         finally:
             # Clean up references to the target function and its arguments
             del self._target, self._args, self._kwargs
 
-def run_calculation_in_thread(window, data, selected_sheet, selected_columns, selected_result_columns, calculation_settings):
+def run_calculation_in_thread(window, data, selected_sheet, selected_columns, selected_result_column, calculation_settings):
+    global cancel_calculation
     # NB: this function was created and annotated using OpenAI's ChatGTP. 
     # Create a thread for the calculation
-    calculation_thread = CalculationThread(target=run_calculation, args=(data, selected_sheet, selected_columns, selected_result_columns, calculation_settings))
+    calculation_thread = CalculationThread(target=run_calculation, args=(data, selected_sheet, selected_columns, selected_result_column, calculation_settings))
     calculation_thread.start()
     # Update the GUI to indicate that the calculation is underway
-    popup_layout = [[sg.Text("Calculation is underway. Please wait...")]]
+    popup_layout = [[sg.Text("Calculation is underway. Please wait...")],[sg.Button('Stop calculation',key='Cancel')]]
     popup_window = sg.Window("Please Wait", popup_layout, finalize=True)
     # Maintain an infinite loop to process events until the window is shut down.
+    cancelled=False
     while True:
         # Read events from the popup window with a timeout of 100 milliseconds
         event, values = popup_window.read(timeout=100)  
         # Check if the popup window is closed or the calculation thread has finished
+        if event=='Cancel':
+            popup_window.close()
+            cancel_calculation=True
+            break
         if event == sg.WIN_CLOSED or not calculation_thread.is_alive():
             break
+    if cancelled:
+        return None
     # Close the popup window
     popup_window.close()
     # Wait for the calculation thread to complete
     calculation_thread.join()
     # Retrieve the return values from the calculation thread
     calculation_result = calculation_thread.result
     return calculation_result
@@ -181,25 +885,28 @@
      is used to also show the mass balance for the data.'''
     if settings['mode']=='Together':
         plot_mode='together'
     elif settings['mode']=='Scroll':
         plot_mode='scrollable'
     else:
         plot_mode='separate'
-    legend_outside=True if settings['legend_position']=='outside' else False
+    legend_outside=True if settings['legend_position']=='Outside' else False
     if stochiometry_list != None:
-        # Obtain species and stochiometry lists from dict input.
-        species = list(stochiometry_list.keys())
-        stochiometry = list(float(i) for i in stochiometry_list.values())
-        # plot the data with mass balance. 
-        auto_vtna.plot_data_MB(data, species, stochiometry, ylim=settings['ylim'],
-                t_unit=settings['t_unit'],y_unit=settings['y_unit'],
-                fig_size_scaler=settings['size_scaler'],plot_mode=plot_mode,
-                DP_scaler=settings['DP_scaler'],legend_outside=legend_outside,
-                linewidth=settings['linewidth'])
+        try:
+            # Obtain species and stochiometry lists from dict input.
+            species = list(stochiometry_list.keys())
+            stochiometry = list(float(i) for i in stochiometry_list.values())
+            # plot the data with mass balance. 
+            auto_vtna.plot_data_MB(data, species, stochiometry, ylim=settings['ylim'],
+                    t_unit=settings['t_unit'],y_unit=settings['y_unit'],
+                    fig_size_scaler=settings['size_scaler'],plot_mode=plot_mode,
+                    DP_scaler=settings['DP_scaler'],legend_outside=legend_outside,
+                    linewidth=settings['linewidth'])
+        except ValueError as e:
+            sg.popup_error(f"Invalid input: {e}")
     else:
         # Plot the data without mass balance shown. 
         auto_vtna.plot_data(data, ylim=settings['ylim'],
                 t_unit=settings['t_unit'],y_unit=settings['y_unit'],
                 fig_size_scaler=settings['size_scaler'],plot_mode=plot_mode,
                 DP_scaler=settings['DP_scaler'],legend_outside=legend_outside,
                 linewidth=settings['linewidth'])
@@ -216,55 +923,61 @@
     "Checks if a variable can be converted to an integer."
     try:
         int(value)
         return True
     except ValueError:
         return False
 
-def run_calculation(data, selected_experiments,selected_columns, selected_result_columns, calculation_settings):
+def run_calculation(data, selected_experiments,selected_columns, selected_result_column, calculation_settings):
     '''Runs calculation by preparing the applied calculation settings to be inputted into 
     Auto-VTNA.'''
     # Create a VTNA selection dictonary.
     VTNA_selection_dict=auto_vtna.make_VTNA_selection(data)
     # Add the normalised species selected in the GUI with orders of 1 as placeholders.
     VTNA_selection_dict['normalised_species']={}
     for molecule in selected_columns:
         VTNA_selection_dict['normalised_species'][molecule]=1
     # Define the experiments selected in the GUI that will be included in the calculation.
     VTNA_selection_dict['RM']={}
     for i in selected_experiments:
         VTNA_selection_dict['RM'][i]={}
         VTNA_selection_dict['RM'][i]["omissions"]=None
     # Define the output species specified in the GUI.
-    VTNA_selection_dict['output_species']=selected_result_columns[0]
+    VTNA_selection_dict['output_species']=selected_result_column[0]
     # Define the fixed order species with their selected order values. 
     fixed_order_species=calculation_settings["fixed_order_species"]
     if fixed_order_species!=None:
         for (i,j) in fixed_order_species.items():
             if i in selected_columns:
                 VTNA_selection_dict['normalised_species'][i]=j
     # Make a keyword argument for the fixed order species. 
     if fixed_order_species!=None:
         fixed_order_species=list(fixed_order_species.keys())
     # Define the constraint argument based on the selected in teh calculation_settings dictionary. 
     constraint=calculation_settings['constraint']
-    if calculation_settings['constraint']=='through origin':
+    if calculation_settings['constraint']=='Via origin':
         constraint='origin'
+    if calculation_settings['constraint']=='Monotonic':
+        constraint='monotonic'
     if calculation_settings['constraint']=='None':
         constraint=None
     if calculation_settings['initial_mesh_denser']=='False':
         initial_mesh_denser=False
     else:
         initial_mesh_denser=True
     # Set up the automatic VTNA calculation. 
-    VTNA_auto_calculation=Automatic_VTNA(data,VTNA_selection_dict,order_range=calculation_settings["order_range"],
+    Calculation_result=Automatic_VTNA(data,VTNA_selection_dict,order_range=calculation_settings["order_range"],
     resolution=calculation_settings["resolution"],deg=calculation_settings["deg"],fit_metric=calculation_settings["fit_metric"],
     iterations=calculation_settings["iterations"], constraint=constraint,score_interval=calculation_settings["score_interval"],
     fixed_order_species=fixed_order_species,initial_mesh_denser=initial_mesh_denser)
-    return VTNA_auto_calculation
+    if str(type(Calculation_result.results))!='NoneType':
+        VTNA_auto_calculation=Calculation_result
+        return VTNA_auto_calculation
+    else:
+        return None
 
 def check_kinetic_data(kinetic_data):
     '''Code to apply the check_kinetic_data() function from Auto-VTNA 
     and generate a text box for the resulting report.'''
     # NB: this code was written with help from OpenAI's ChatGTP. 
     # Check if the kinetic data is loaded correctly. 
     result_string = auto_vtna.check_kinetic_data(kinetic_data,bold_and_red=False,print_report=False)
@@ -325,15 +1038,15 @@
     matplotlib.pyplot'''
     # NB: this code was written with help from OpenAI's ChatGTP.
     # Ensure that all exisiting plots are closed to avoid bugs.
     plt.close('all')
     # Obtain the intial concentrations for each experiment in the kinetic dataset. 
     initial_concs_df= auto_vtna.initial_concs(kinetic_data)
     # Format numeric values with scientific notation and specified significant figures
-    initial_concs_df_formatted = initial_concs_df.applymap(
+    initial_concs_df_formatted = initial_concs_df.map(
         lambda x: apply_best_number_format(x, significant_figures) if isinstance(x, (int, float)) else x)
     # Create the pyplot figure.
     fig, ax = plt.subplots(figsize=(12*fig_size, 5*fig_size))
     ax.axis('off')  # Turn off axis
     # Create a table and add it to the axis.
     table = ax.table(cellText=initial_concs_df_formatted.values, colLabels=initial_concs_df_formatted.columns,
      cellLoc='center', loc='center', cellColours=[['#e0e0e0']*len(initial_concs_df_formatted.columns)]*len(initial_concs_df_formatted),
@@ -380,96 +1093,103 @@
     # Apply tight layout and show the table. 
     plt.tight_layout()
     plt.show()
 
 def plot_concentration_profiles(kinetic_data, selected_species,settings):
     '''Plots concentration profiles using the plot_data_together function from
     auto_vtna. Applies keyword arguments based on the plot settings dictionary.'''
-    legend_outside=True if settings['legend_position']=='outside' else False
+    legend_outside=True if settings['legend_position']=='Outside' else False
     # Ensure that all exisiting plots are closed to avoid bugs.
     plt.close('all')
     auto_vtna.plot_data_together(kinetic_data, selected_species,ylim=settings['ylim'],
      y_unit=settings['y_unit'], t_unit=settings['t_unit'],legend_outside=legend_outside,
      fig_size_scaler=settings['size_scaler'],DP_scaler=settings['DP_scaler'],linewidth=settings['linewidth'])
     
 def main():
     # NB: some parts of the main GUI code was written with help from OpenAI's ChatGTP.
+    # Define the cancel_calculation as global
+    global cancel_calculation
     img = None # Placeholder for overlay score versus order plot image.
     fixed_orders={} # Placeholder for fixed_orders dictionary
     enable_plot_button = False  # Flag to track whether the calculation has been run
     # Define settings dictionaries for automatic VTNA calculation, the overlay score versus order plot, 
     # data visualisation functions and normal VTNA overlay plot settings. 
     calculation_settings = {"order_range": [-1.5, 2.5], "resolution": 7, "deg": 5, "fit_metric": 'RMSE',
-                            "iterations": 7, "constraint": 'monotonic', "score_interval": 0.15,
+                            "iterations": 7, "constraint": 'Monotonic', "score_interval": 0.15,
                             "fixed_order_species": None,"initial_mesh_denser":'True'}
     order_vs_overlay_plot_settings = {"y_unit":'M',"size_scaler1":1,"popup_scaler":1,"colour_scaler":1,
                             "contour_resolution":None,"datapoints":False,"interval":False,"zoom":'None',
                             "contour_cbar_max":None,"contour_cbar_min":None, "custom_title":None,"show_legend_popup":True,
-                            'show_legend_main':True,'decimals_cbar':3,'annotate':True,"plot_score_interval":None}
-    data_plotting_settings={"ylim":None,"t_unit":None,'y_unit':'M',"size_scaler":1,'DP_scaler':1,"mode":'Together',\
-                            "significant_figs":3,'legend_position':'Inside','linewidth':1}
+                            'show_legend_main':True,'decimals_cbar':3,'annotate':True,"score_interval":0.15}
+    data_plotting_settings={"ylim":None,"t_unit":None,'y_unit':'M',"size_scaler":1,'DP_scaler':1,"mode":'Scroll',\
+                            "SF":3,'legend_position':'Outside','linewidth':1}
     overlay_plot_settings={'y_unit':'M',"size_scaler":1,"tt_scaler":1,"grid":False,"custom_title":None,"check_score":False,\
-                           "check_fit":False,"constraint":'monotonic','deg':5,"fit_metric":'RMSE',
+                           "check_fit":False,"constraint":'Monotonic','deg':5,"fit_metric":'RMSE',
                            'score_settings_visibility':False,'DP_scaler':1,'xtick_rotation':0,'legend':True,
                            'legend_position':'Inside','extra_legend':'True','save':False,'saved_values':{},'line_scaler':1,
                            'tT_notation':'Automatic'}
+    # Save the standard settings for resetting the settings window to default values. 
+    default_overlay_plot_settings=overlay_plot_settings.copy()
+    default_order_vs_overlay_plot_settings=order_vs_overlay_plot_settings.copy()
+    default_data_plotting_settings=data_plotting_settings.copy()
+    default_calculation_settings=calculation_settings.copy()
     # Define placeholder dict for the Automatic VTNA results. 
     auto_vtna_results={"best_order_dict":{'':'','\t':'','\r':''},"order_vs_overlay_table":None,"interval_table":None,"plot_image":None}
     # Define other miscellaneous placeholders.
     best_order_dict={}
     best_order_dict_rounded={}
     omission_dictionary=None
     omission_range_dictionary={}
     omission_range_dictionary["range_type"]='Percentage'
     omission_mode='Datapoint mode'
     Plot_concentration_profiles_selected_experiments=False
     # Define the layout of the main GUI window.
     layout = [
         [sg.Frame("Load Kinetic Data", layout=[
-            [sg.Text("Use Excel File:"),
+            [sg.Text("Use Excel file:"),
             sg.InputText(key="file_path", enable_events=True, size=(12, 1)), 
             sg.FileBrowse(),sg.Text("Or:"),sg.Button("Use CSVs",key="Select CSVs")]
         ])],
-        [sg.Button("Check Data",key="Check Kinetic Data", disabled=True),
-         sg.Button("Visualise Data",key="Inspect Kinetic Data", disabled=True),
-         sg.Button("Crop Data", key="Crop Kinetic Data", disabled=True),
+        [sg.Button("Check data",key="Check Kinetic Data", disabled=True),
+         sg.Button("Visualise data",key="Inspect Kinetic Data", disabled=True),
+         sg.Button("Crop data", key="Crop Kinetic Data", disabled=True),
          sg.Combo(['Range mode', 'Datapoint mode'], default_value=omission_mode,key="crop_mode", enable_events=True, readonly=True,size=(12,1))],
-        [sg.Frame("Select experiments", layout=[
+        [sg.Frame("Select Experiments", layout=[
             [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE, size=(22, 5), key="experiments")]
         ]),
         sg.Frame("Select Normalised Species", layout=[
             [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE, size=(21, 5), key="columns")]
         ])],
-        [sg.Frame("Select output species", layout=[
-            [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_SINGLE, size=(20, 1), key="result_columns")]
+        [sg.Frame("Select Output Species", layout=[
+            [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_SINGLE, size=(20, 1), key="result_column")]
         ]),
-        sg.Frame("VTNA overlay plot", layout=[
+        sg.Frame("VTNA Overlay Plot", layout=[
             [sg.Button("Generate plot", key="Generate Overlay Plot", disabled=True),
-            sg.Button("Plot Settings", key="Overlay Plot Settings", disabled=True)]
+            sg.Button("Plot settings", key="Overlay Plot Settings", disabled=True)]
         ])],
         [sg.Frame("Automatic VTNA", layout=[
             [sg.Button(" Run ", key='Run Auto VTNA' ,disabled=True),
             sg.Button(" Calculation ⚙", key="calculation_settings", disabled=True),
             sg.Button(" Save \U0001F4BE ", key="Save Results", disabled=not enable_plot_button)],
-            [sg.Button("Plot Results", disabled=not enable_plot_button),
-            sg.Button("Plot ⚙", key="Plot Settings", disabled=not enable_plot_button),
+            [sg.Button("Plot results", disabled=not enable_plot_button),
+            sg.Button("Plot ⚙", key="Plot settings", disabled=not enable_plot_button),
             sg.Button("Show +Info", key="extra_info", disabled=not enable_plot_button)]
         ]),
         sg.Table(values=[[key, value] for key, value in auto_vtna_results["best_order_dict"].items()],
                 headings=['Compound', 'Order'],
                 auto_size_columns=False,
                 justification='right',
                 num_rows=min(5, len(auto_vtna_results["best_order_dict"])),
                 col_widths=[8, 5],
                 key='-TABLE-')],
         [sg.Column([
-        [sg.pin(sg.Text('placeholder',key="Overlay Score",enable_events=True,visible=False,metadata=False,font=11))],
-        [sg.pin(sg.Text("Intervals of order values less than",key="Rest of string",enable_events=True,visible=False,metadata=False,font=11)),
-        sg.pin(sg.InputText(key="interval_score", size=(4, 1),default_text=calculation_settings['score_interval']*100,enable_events=True,visible=False,metadata=False,font=11)),
-        sg.pin(sg.Text("% from optimum:",key="Rest of string 2",enable_events=True,visible=False,metadata=False,font=11))]], element_justification='left'),
+        [sg.pin(sg.Text('placeholder',key="Overlay Score",enable_events=True,visible=False,metadata=False,font=('Any',8)))],
+        [sg.pin(sg.Text("Intervals of order values less than",key="Rest of string",enable_events=True,visible=False,metadata=False,font=('Any',8))),
+        sg.pin(sg.InputText(key="interval_score", size=(4, 1),default_text=calculation_settings['score_interval']*100,enable_events=True,visible=False,metadata=False,font=('Any',8))),
+        sg.pin(sg.Text("% from optimum:",key="Rest of string 2",enable_events=True,visible=False,metadata=False,font=('Any',8)))]], element_justification='left'),
         sg.Column([[sg.pin(sg.Button('Refresh',key='refresh_interval_table',enable_events=True,visible=False,metadata=False))]])],
         [sg.pin(sg.Table(values={},headings=['Normalised species','Lower order limit','Upper order limit'],auto_size_columns=False,col_widths=[14,13,13],key='interval_table',visible=False))]
     ]
     window = sg.Window("Automatic VTNA Calculator", layout)
     # Generate and close a matplotlib pyplot graph to avoid GUI resolution bug.
     plt.plot([1,2],[1,2])
     plt.close()
@@ -509,102 +1229,154 @@
                         omission_mode='Datapoint mode'
                     # Update the "crop_mode" value. 
                     window["crop_mode"].update(value=omission_mode)
                     # Obtain information from the dataset. 
                     time_label=list(data.values())[0].columns[0]
                     experiments = list(data.keys())
                     columns = data[experiments[0]].columns[1:].tolist()  # Exclude the first column
+                    # Create a list of reaction species that have concentration profiles that change over time. 
+                    reaction_species_not_constant=data[experiments[0]].columns[1:].tolist()
+                    for exp in data.keys():
+                        for species in columns:
+                            # Avoid trying to remove a constant species twice. 
+                            if species in reaction_species_not_constant:
+                                # Define the list of concentration values for the relevant species in the relevant experiment. 
+                                values=list(data[exp][species].to_numpy())
+                                # If all values are the same, remove this species from the not constant list
+                                if all([species==values[0] for species in values]):
+                                    reaction_species_not_constant.remove(species)
                     fixed_order_species = data[experiments[0]].columns[1:].tolist()  # All reaction species
                     # Update the window to add information from the selected kinetic dataset and enable buttons for analysis.
                     window["experiments"].update(values=experiments)
                     window["columns"].update(values=columns)
-                    window["result_columns"].update(values=columns)
+                    window["result_column"].update(values=reaction_species_not_constant)
                     window["Run Auto VTNA"].update(disabled=False)  # Enable the "Run Automatic VTNA" button
                     window["calculation_settings"].update(disabled=False)  # Enable the "Calculation Settings" button
                     window["Check Kinetic Data"].update(disabled=False)
                     window["Inspect Kinetic Data"].update(disabled=False)
                     window["Generate Overlay Plot"].update(disabled=False)
                     window["Overlay Plot Settings"].update(disabled=False)
                     window["Crop Kinetic Data"].update(disabled=False)
                 # Raise any errors:
                 except PermissionError as e:
                     sg.popup_error(f"Error opening file (make sure it is not open): {e}")
                     continue
+                except ValueError as e:
+                    sg.popup_error(f"Error: {e}")
+                    continue
+                except KeyError as e:
+                    sg.popup_error(f"Error: {e}")
+                    continue
         # Update the omission_mode variable if the user changes this setting in the main GUI window.
         elif event == "crop_mode":
             omission_mode=values["crop_mode"]
         # Save the results from the automatic VTNA calculation. 
         elif event == "Save Results":
             # Define the layout of the save results pop-up menu. 
+
+            [sg.Column([[sg.Text("Show main plot legend:")],[sg.Text("Show error interval:")],[sg.Text("Overlay score interval: ")],[sg.Text("Main figure size scaler:")]]),
+                    sg.Column([[sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['show_legend_main']),key='show_legend_main', enable_events=True, readonly=True,size=(6,1))],
+                               [sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['interval']),key="interval", enable_events=True, readonly=True,size=(6,1))],
+                               [sg.InputText(key="score_interval", size=(6, 1),default_text=order_vs_overlay_plot_settings["score_interval"])],
+                               [sg.InputText(key="size_scaler1", size=(6, 1),default_text=float(order_vs_overlay_plot_settings["size_scaler1"]))]])],
+
             layout_save = [
-                [sg.Text("Filename:"), sg.InputText(key="filename", size=(5, 1))],
-                [sg.Text("File type:"), sg.Combo(['csv', 'xlsx'], default_value='xlsx', key="filetype", readonly=True)],
-                [sg.Button("OK"), sg.Button("Cancel")]
-            ]
+                [sg.Column([[sg.Text("Filename:")],[sg.Text("File type:")],[sg.Text("Folder location:")]]),
+                sg.Column([[sg.InputText(key="filename", size=(5, 1),enable_events=True)],
+                [sg.Combo(['csv', 'xlsx'], default_value='xlsx', key="filetype", readonly=True,enable_events=True)],
+                [sg.InputText(key="folder", size=(21, 1),enable_events=True,default_text='Default: folder of .exe file')]
+                ])],
+                [sg.Button('OK'),sg.Button("Select file location")]]
             # Create the save results pop-up menu.
             window_save = sg.Window("Save file settings", layout_save)
             # Apply event loop to process user inputs. 
             while True:
                 event_save, values_save = window_save.read()
                 if event_save == sg.WINDOW_CLOSED or event_save == 'Cancel':
                     window_save.close()
                     break
+                elif event_save == "Select file location":
+                    # Create a popup window to allow the user to select file type (csv or xlsx), 
+                    # file location and file name. 
+                    file_path_save = sg.popup_get_file('Save As', save_as=True, no_window=True,file_types=(("Excel File", "*.xlsx"), ("CSV File", "*.csv")))
+                    # Use the inputted file path to define the file name, the extension and the folder location.
+                    filename = os.path.splitext(os.path.basename(file_path_save))[0]
+                    file_extension = os.path.splitext(file_path_save)[1].replace('.','')
+                    folder_location = os.path.dirname(file_path_save)
+                    # Update the save window with the relevant info.
+                    window_save["filetype"].update(value=file_extension)
+                    window_save["filename"].update(value=filename)
+                    window_save["folder"].update(value=folder_location)
                 elif event_save == 'OK':
                     # use try and exception to enable error messages that don't terminate the GUI.
                     try:
                         if values_save['filename'] is None or values_save['filename'] == '':
                             raise ValueError("Define a filename to continue.")
                         elif values_save['filetype'] is None or window_save['filetype']=='':
                             raise ValueError("Define a filetype to continue.")
+                        # Define the file path to use to save the results from the automatic VTNA calculation. 
+                        if values_save['folder'] in ['Default: folder of .exe file','']:
+                            file_path_save=f"{values_save['filename']}.{values_save['filetype']}"
+                        else:
+                            # Use the path chosen by the user in the popup_get_file window.
+                            file_path_save=f"{values_save['folder']}/{values_save['filename']}.{file_extension}"
                         # Create a report containing information about the automatic VTNA calculation.
-                        filetype = values_save["filetype"]
-                        filename = values_save['filename']
+                        # First, include the path to the inputted kinetic data file. 
                         files_calculation_nested = [['', files_calculation]]
                         if type(files_calculation) != str:
                             files_calculation_nested = [['', i] for i in files_calculation]
                         files_calculation_nested.insert(0, ["Kinetic data is loaded from:"])
+                        # Identify the list of fixed order normalised species. 
                         fixed_order_species_name=VTNA_auto_calculation.fixed_order_species
                         if fixed_order_species_name==None:
                             fixed_order_species_name='None'
+                        # Identify the fitting constraint of the calculation. 
                         constraint = VTNA_auto_calculation.constraint if VTNA_auto_calculation.constraint not in [None,''] else 'None'
+                        # Create a page containing inputs for the automatic VTNA calculation. 
                         page1 = [
                             ["FITTING METHOD:"],
                             ["  - Fitting constraint:", constraint ],
                             ["  - Degree of fitting polynomial:", VTNA_auto_calculation.deg],
                             ["  - Goodness-of-fit measurement:", VTNA_auto_calculation.fit_metric],
                             ["OTHER CALCULATION SETTINGS:"],
                             ["  - Order value range:", VTNA_auto_calculation.order_range],
                             ["  - Order intervals:", f"{float(VTNA_auto_calculation.score_interval) * 100}% from optimal GOF."],
                             ["  - Algorithm iterations:", VTNA_auto_calculation.iterations],
                             ["  - Density of order value grid:", VTNA_auto_calculation.resolution],
+                            ["  - First order grid more dense:",str(VTNA_auto_calculation.initial_mesh_denser)],
                             ["  - Fixed order species:", fixed_order_species_name],
                             ["VTNA SELECTION DICTIONARY:"]
                         ]
+                        # Create a list with the contents of the VTNA selection dictionary. 
                         selection_list = list(VTNA_auto_calculation.VTNA_selection.items())
+                        # Create a list containing the experiment names and their omissions settings. 
                         s0_2=[['RM']]
                         for key, value in selection_list[0][-1].items():
                             RM_omissions=[key]
                             if list(list(value.items())[0])[1]!=None:
                                 RM_omissions=RM_omissions+[list(list(value.items())[0])[0]]+list(list(value.items())[0])[1]
                             else:
                                 RM_omissions=RM_omissions+[list(list(value.items())[0])[0]]+['None']
                             s0_2.append(RM_omissions)
+                        # Create a list containing all the normalised species defined for the calculation. 
                         s1_2 = [['normalised_species']]
                         s1_2.extend(["  - "+key, value] for key, value in selection_list[2][1].items())
                         selection_list[2] = s1_2
                         selection_list=s0_2+[selection_list[1]]+s1_2
+                        # Combine the 3 lists to define the first page of the results file. 
                         page1 = files_calculation_nested + page1 + selection_list
+                        # Convert the nested list to a pandas dataframe object. 
                         page1_df = pd.DataFrame(page1)
                     except ValueError as e:
                         sg.popup_error(f"Invalid input: {e}")
                         continue
-                    if filetype == 'csv':
+                    if values_save['filetype'] == 'csv':
                         # Create a report for a CSV file if this has been selected by the user.
                         try:
-                            with open(f'{filename}.csv', 'w', newline='') as csvfile:
+                            with open(file_path_save, 'w', newline='') as csvfile:
                                 csv_writer = csv.writer(csvfile)
                                 # Write page1
                                 csv_writer.writerows(page1)
                                 # Write VTNA_auto_calculation.interval
                                 csv_writer.writerow([])
                                 csv_writer.writerow([f'{str(float(VTNA_auto_calculation.score_interval)*100)}% order intervals.'])
                                 VTNA_auto_calculation.interval.to_csv(csvfile, index=False, header=True)
@@ -614,111 +1386,112 @@
                                 VTNA_auto_calculation.results.to_csv(csvfile, index=False, header=True)
                         except Exception as e:
                             sg.popup_error(f"Filename permission error (close CSV file with the same name): {e}")
                             continue
                     else:
                         try:
                             # Create a sheet for the page1_df information.
-                            with pd.ExcelWriter(f'{filename}.xlsx', engine='xlsxwriter') as writer:
+                            with pd.ExcelWriter(file_path_save, engine='xlsxwriter') as writer:
                                 page1_df.to_excel(writer, index=False, header=False, sheet_name='Calculation settings')
                             # Create a sheet for the uncertainty intervals of each normalised species.
-                            with pd.ExcelWriter(f'{filename}.xlsx', engine='openpyxl', mode='a') as writer:
+                            with pd.ExcelWriter(file_path_save, engine='openpyxl', mode='a') as writer:
                                 VTNA_auto_calculation.interval.to_excel(writer, index=False, header=True, sheet_name=f'{str(float(VTNA_auto_calculation.score_interval)*100)}% order intervals.')
                             # Create a sheet for the overlay score versus order matrix. 
-                            with pd.ExcelWriter(f'{filename}.xlsx', engine='openpyxl', mode='a') as writer:
+                            with pd.ExcelWriter(file_path_save, engine='openpyxl', mode='a') as writer:
                                 VTNA_auto_calculation.results.to_excel(writer, index=False, header=True, sheet_name='Overlay score vs. order matrix')
                             if img is not None:
                                 # Add the image of the recently generated overlay score versus order plot.
                                 writer.book.create_sheet('Overlay score vs. order plot')
-                                writer.book.save(f'{filename}.xlsx')
+                                writer.book.save(file_path_save)
                                 sheet = writer.sheets['Overlay score vs. order plot']
                                 sheet.add_image(img, 'A1')
-                                writer.book.save(f'{filename}.xlsx')
+                                writer.book.save(file_path_save)
                         except Exception as e:
                             sg.popup_error(f"Filename permission error (close excel file with same name): {e}")
                             continue
                     window_save.close()
                     break
 
         elif event == "Run Auto VTNA":
             # Get selected sheet, columns, and result columns
             selected_sheet = values["experiments"]
             selected_columns = values["columns"]
-            selected_result_columns = values["result_columns"]
-            if selected_sheet and selected_columns and selected_result_columns:
+            selected_result_column = values["result_column"]
+            if selected_sheet and selected_columns and selected_result_column:
                 # Check that the number of fixed order species is lower than the total number of selected normalised species. 
                 count=len(selected_columns)
                 if type(calculation_settings["fixed_order_species"])==dict:
                     # Raise an error if any fixed order species are not selected as normalised species. 
                     if not all([i in list(selected_columns) for i in list(calculation_settings["fixed_order_species"].keys())]):
                         sg.popup_error("All selected fixed reaction species must also be selected as normalised species.")
                         continue
                     for i in selected_columns:
                         if i in list(calculation_settings["fixed_order_species"].keys()):
                             count+=-1
                 if count>=1:
                         # Run the automatic VTNA calculation in thread to calculate the time passed for the calculation. 
-                        VTNA_auto_calculation = run_calculation_in_thread(window, data, selected_sheet, selected_columns, selected_result_columns, calculation_settings)
-                        best_order_dict={}
-                        # Store the best order information from the calculation. 
-                        for i in range(len(VTNA_auto_calculation.best_orders)):
-                            best_order_dict[f"{VTNA_auto_calculation.results.columns[i].replace('order in ','')}"]=VTNA_auto_calculation.best_orders[i]
-                        orders_last_species=VTNA_auto_calculation.results.iloc[:,-2].to_numpy()
-                        resolution_orders=str(format(orders_last_species[-1]-orders_last_species[-2],".12f"))
-                        best_order_dict_rounded={}
-                        # Make a rounded version of the best order dictionary. 
-                        for i in range(len(resolution_orders)):
-                            if resolution_orders[i]!='.' and resolution_orders[i]!='0':
-                                break
-                        for species,best_order in best_order_dict.items():
-                            best_rounded=f'{round(best_order, i-1):.{int(i-1)}f}'
-                            best_order_dict_rounded[species]=best_rounded
-                        # Update the auto_vtna_result dictionary.
-                        auto_vtna_results["best_order_dict"]=best_order_dict
-                        auto_vtna_results["order_vs_overlay_table"]=VTNA_auto_calculation.results
-                        auto_vtna_results["interval_table"]=VTNA_auto_calculation.interval
-                        if VTNA_auto_calculation:
-                            # Inform the user that the automatic VTNA calculation is complete. 
-                            sg.popup("Calculation complete.",auto_close=True, auto_close_duration=2)
-                            window['-TABLE-'].update(values=[[key, value] for key, value in best_order_dict_rounded.items()])
-                            enable_plot_button = True  # Enable the "Plot Results" button
-                            # Enable buttons for plottin the results of the automatic VTNA calculation. 
-                            window["Plot Results"].update(disabled=not enable_plot_button)
-                            window["Save Results"].update(disabled=not enable_plot_button)
-                            window["Plot Settings"].update(disabled=not enable_plot_button)
-                            window["extra_info"].update(disabled=False)
-                            # Identify the best overlay score.
-                            if calculation_settings['fit_metric']=='R2':
-                                best_OS=round(max(VTNA_auto_calculation.results[f"{VTNA_auto_calculation.fit_metric} overlay score"]),5)
-                            else:
-                                best_OS=round(min(VTNA_auto_calculation.results[f"{VTNA_auto_calculation.fit_metric} overlay score"]),6)  
-                            overlay_score_string=f"Overlay score ({calculation_settings['fit_metric']}) at the optimal order values: {str(best_OS)}"
-                            if VTNA_auto_calculation.deg==1:
-                                # Determine a sensible number of decimals to include for the slope value. 
-                                rounding=6
-                                slope=VTNA_auto_calculation.best_slope
-                                order_of_magnitude_slope=round(np.log10(slope))
-                                rounding+=(-order_of_magnitude_slope)
-                                # Add the slope to the overlay score string. 
-                                overlay_score_string=overlay_score_string+f'\nSlope of linear fit w/ best orders (w/o data scaling): {round(VTNA_auto_calculation.best_slope,rounding)}'
-                            # Update the interval table using the intervals from the automatic VTNA calculation. 
-                            df_interval=VTNA_auto_calculation.interval.round(decimals=5)
-                            table_values=df_interval.values.tolist()
-                            for i,value in enumerate(table_values):
-                                table_values[i]=tuple(value)
-                            window['interval_table'].update(values=table_values)
-                            window["Overlay Score"].update(overlay_score_string)
-                            window["interval_score"].update(calculation_settings['score_interval']*100)
-                            window['interval_table'].update(num_rows=len(table_values))   
+                        calculation = run_calculation_in_thread(window, data, selected_sheet, selected_columns, selected_result_column, calculation_settings)
+                        if 'None' not in str(type(calculation.results)):
+                            VTNA_auto_calculation = calculation
+                            best_order_dict={}
+                            # Store the best order information from the calculation. 
+                            for i in range(len(VTNA_auto_calculation.best_orders)):
+                                best_order_dict[f"{VTNA_auto_calculation.results.columns[i].replace('order in ','')}"]=VTNA_auto_calculation.best_orders[i]
+                            orders_last_species=VTNA_auto_calculation.results.iloc[:,-2].to_numpy()
+                            resolution_orders=str(format(orders_last_species[-1]-orders_last_species[-2],".12f"))
+                            best_order_dict_rounded={}
+                            # Make a rounded version of the best order dictionary. 
+                            for i in range(len(resolution_orders)):
+                                if resolution_orders[i]!='.' and resolution_orders[i]!='0':
+                                    break
+                            for species,best_order in best_order_dict.items():
+                                best_rounded=f'{round(best_order, i-1):.{int(i-1)}f}'
+                                best_order_dict_rounded[species]=best_rounded
+                            # Update the auto_vtna_result dictionary.
+                            auto_vtna_results["best_order_dict"]=best_order_dict
+                            auto_vtna_results["order_vs_overlay_table"]=VTNA_auto_calculation.results
+                            auto_vtna_results["interval_table"]=VTNA_auto_calculation.interval
+                            if VTNA_auto_calculation:
+                                # Inform the user that the automatic VTNA calculation is complete. 
+                                sg.popup("Calculation complete.",auto_close=True, auto_close_duration=2)
+                                window['-TABLE-'].update(values=[[key, value] for key, value in best_order_dict_rounded.items()])
+                                enable_plot_button = True  # Enable the "Plot Results" button
+                                # Enable buttons for plottin the results of the automatic VTNA calculation. 
+                                window["Plot results"].update(disabled=not enable_plot_button)
+                                window["Save Results"].update(disabled=not enable_plot_button)
+                                window["Plot settings"].update(disabled=not enable_plot_button)
+                                window["extra_info"].update(disabled=False)
+                                # Identify the best overlay score.
+                                if calculation_settings['fit_metric']=='R2':
+                                    best_OS=round(max(VTNA_auto_calculation.results[f"{VTNA_auto_calculation.fit_metric} overlay score"]),5)
+                                else:
+                                    best_OS=round(min(VTNA_auto_calculation.results[f"{VTNA_auto_calculation.fit_metric} overlay score"]),6)  
+                                overlay_score_string=f"Overlay score ({calculation_settings['fit_metric']}) at the optimal order values: {str(best_OS)}"
+                                if VTNA_auto_calculation.deg==1:
+                                    # Determine a sensible number of decimals to include for the slope value. 
+                                    rounding=6
+                                    slope=VTNA_auto_calculation.best_slope
+                                    order_of_magnitude_slope=round(np.log10(slope))
+                                    rounding+=(-order_of_magnitude_slope)
+                                    # Add the slope to the overlay score string. 
+                                    overlay_score_string=overlay_score_string+f'\nSlope of linear fit w/ best orders (w/o data scaling): {round(VTNA_auto_calculation.best_slope,rounding)}'
+                                # Update the interval table using the intervals from the automatic VTNA calculation. 
+                                df_interval=VTNA_auto_calculation.interval.round(decimals=5)
+                                table_values=df_interval.values.tolist()
+                                for i,value in enumerate(table_values):
+                                    table_values[i]=tuple(value)
+                                window['interval_table'].update(values=table_values)
+                                window["Overlay Score"].update(overlay_score_string)
+                                window["interval_score"].update(calculation_settings['score_interval']*100)
+                                window['interval_table'].update(num_rows=len(table_values))   
                 else:
                     sg.popup_error("The number of fixed order species can't be the same as or higher than the number of normalised reaction species.")
             else:
                 sg.popup_error("Please select experiments, reaction species, and output reaction species to run automatic VTNA.")
         elif event == "refresh_interval_table":
-            print(values['interval_score'])
             try:
                 interval_score=values['interval_score']
                 if not is_float(interval_score):
                     raise ValueError("Invalid score interval. Must be numerical")
                 if not float(interval_score)>0:
                     raise ValueError("Invalid score interval. Must be above 0.")
             except ValueError as e:
@@ -742,87 +1515,88 @@
             window['refresh_interval_table'].update(visible=visible)
             # Update the extra info button according to the visibility status. 
             if visible:
                 window['extra_info'].update('Hide + Info')
             else:
                 window['extra_info'].update('Show +Info')
 
-        elif event == "Plot Settings":
+        elif event == "Plot settings":
             # Define the layout of the plot settings menu, consisting of 3 different frames for general settings, 
             # contour plot settings and pop-up overlay plot settings (for the VTNA overlay plots generated by clicking 
             # on the main plot.)
             layout_settings_OvsO_plot = [
-                [sg.Text("Overlay Score vs. Order Plot Settings", font=("helvetica", 12, "bold"))],
+                [sg.Text("Overlay Score vs. Order Plot Settings", font=("helvetica", 11, "bold"))],
                 [sg.Frame("General settings",layout=[
-                    [sg.Text("Show legend in main plot:"),
-                    sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['show_legend_main']),key='show_legend_main', enable_events=True, readonly=True,size=(6,1))],
-                    [sg.Text("Show error interval datapoints:"),
-                    sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['interval']),key="interval", enable_events=True, readonly=True,size=(6,1))],
-                    [sg.Text("Score interval:"),
-                    sg.InputText(key="plot_score_interval", size=(6, 1),default_text=calculation_settings['score_interval'] if order_vs_overlay_plot_settings["plot_score_interval"] in [None,''] else order_vs_overlay_plot_settings["plot_score_interval"])],
+                    [sg.Column([[sg.Text("Show main plot legend:")],[sg.Text("Show error interval:")],[sg.Text("Overlay score interval: ")],[sg.Text("Main figure size scaler:")]]),
+                    sg.Column([[sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['show_legend_main']),key='show_legend_main', enable_events=True, readonly=True,size=(6,1))],
+                               [sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['interval']),key="interval", enable_events=True, readonly=True,size=(6,1))],
+                               [sg.InputText(key="score_interval", size=(6, 1),default_text=order_vs_overlay_plot_settings["score_interval"])],
+                               [sg.InputText(key="size_scaler1", size=(6, 1),default_text=float(order_vs_overlay_plot_settings["size_scaler1"]))]])],
                     [sg.Text("Overlay score range:"),sg.InputText(key="contour_cbar_min", size=(6, 1),default_text='Default' if order_vs_overlay_plot_settings["contour_cbar_min"] is None else str(order_vs_overlay_plot_settings["contour_cbar_min"])),
-                    sg.Text(" to "),sg.InputText(key="contour_cbar_max", size=(6, 1),default_text='Default' if order_vs_overlay_plot_settings["contour_cbar_max"] is None else str(order_vs_overlay_plot_settings["contour_cbar_max"]))],
+                    sg.Text("to"),sg.InputText(key="contour_cbar_max", size=(6, 1),default_text='Default' if order_vs_overlay_plot_settings["contour_cbar_max"] is None else str(order_vs_overlay_plot_settings["contour_cbar_max"]))],
                     [sg.Text("Custom figure title:"),
-                    sg.InputText(key="custom_title", size=(19, 1),default_text=str(order_vs_overlay_plot_settings["custom_title"]) if order_vs_overlay_plot_settings["custom_title"]!=None else '')],
-                    [sg.Text("Main figure size scaler:    "),
-                    sg.InputText(key="main_size_scaler", size=(5, 1),default_text=float(order_vs_overlay_plot_settings["size_scaler1"]))]])],
+                    sg.InputText(key="custom_title", size=(18, 1),default_text=str(order_vs_overlay_plot_settings["custom_title"]) if order_vs_overlay_plot_settings["custom_title"]!=None else 'Default')],
+                    ])],
                 [sg.Frame("Settings for contour plot",layout=[
-                    [sg.Text("Show datapoints:                      "),
-                     sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['datapoints']),key="datapoints", enable_events=True, readonly=True,size=(6,1))],
-                    [sg.Text("Show optimum annotation:         "),
-                     sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['annotate']),key="annotate", enable_events=True, readonly=True,size=(6,1))],
-                    [sg.Text("Color bar max scaler:                "),
-                    sg.InputText(key="colour_scaler", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["colour_scaler"]))],
-                    [sg.Text("Colour bar resolution:                "),
-                    sg.InputText(key="contour_resolution", size=(6, 1),default_text='Default' if order_vs_overlay_plot_settings["contour_resolution"] is None else str(order_vs_overlay_plot_settings["contour_resolution"]))],
-                    [sg.Text("Domain around optimum (zoom):"),
-                     sg.InputText(key="zoom", size=(5, 1),default_text=str(order_vs_overlay_plot_settings["zoom"]))],
-                    [sg.Text("Number of decimals for cbar:     "),
-                     sg.InputText(key="decimals_cbar", size=(5, 1),default_text=str(order_vs_overlay_plot_settings["decimals_cbar"]))]])],
+                    [sg.Column([[sg.Text("Show datapoints:")],[sg.Text("Show optimum annotation:")],[sg.Text("Color bar max scaler:")],[sg.Text("Colour bar resolution:")],[sg.Text("Zoom around optimum:")],[sg.Text("Number of cbar decimals:")]]),
+                    sg.Column([[sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['datapoints']),key="datapoints", enable_events=True, readonly=True,size=(6,1))],
+                               [sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['annotate']),key="annotate", enable_events=True, readonly=True,size=(6,1))],
+                               [sg.InputText(key="colour_scaler", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["colour_scaler"]), enable_events=True)],
+                               [sg.InputText(key="contour_resolution", size=(6, 1),default_text='Default' if order_vs_overlay_plot_settings["contour_resolution"] is None else str(order_vs_overlay_plot_settings["contour_resolution"]), enable_events=True)],
+                               [sg.InputText(key="zoom", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["zoom"]), enable_events=True)],
+                               [sg.InputText(key="decimals_cbar", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["decimals_cbar"]), enable_events=True)]])]])],
                 [sg.Frame("Settings for pop-up overlay plots",layout=[
-                    [sg.Text("Show legend:                 "),
-                    sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['show_legend_popup']),key="show_legend_popup", enable_events=True, readonly=True,size=(6,1))],
-                    [sg.Text("Pop-up figure size scaler:"),
-                    sg.InputText(key="popup_size_scaler", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["popup_scaler"]),enable_events=True)],
-                    [sg.Text("Concentration unit:          "),
-                    sg.InputText(key="y_unit", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["y_unit"]))]])],
-                [sg.Button("OK"), sg.Button("Cancel")]]
+                    [sg.Column([[sg.Text("Show legend:")],[sg.Text("Pop-up figure size scaler:")],[sg.Text("Concentration unit:")]]),
+                    sg.Column([[sg.Combo(['True','False'], default_value=str(order_vs_overlay_plot_settings['show_legend_popup']),key="show_legend_popup", enable_events=True, readonly=True,size=(6,1))],
+                               [sg.InputText(key="popup_scaler", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["popup_scaler"]),enable_events=True)],
+                               [sg.InputText(key="y_unit", size=(6, 1),default_text=str(order_vs_overlay_plot_settings["y_unit"]), enable_events=True)]])]])],
+                [sg.Button("OK"), sg.Button("Cancel"),sg.Button("Reset settings")]]
             # Create the plot settings window. 
             window_OvsO_plot_settings = sg.Window("Order Versus Overlay Plot Settings", layout_settings_OvsO_plot)
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event_OvsO_plot_settings, values_OvsO_plot_settings = window_OvsO_plot_settings.read()
                 # Break the while loop to close the window if cancel is pressed or the window is closed. 
                 if event_OvsO_plot_settings == sg.WIN_CLOSED or event_OvsO_plot_settings == "Cancel":
                     break
+                # If the reset button is pressed, reset all the settings.
+                if event_OvsO_plot_settings=="Reset settings":
+                    for i,j in default_order_vs_overlay_plot_settings.items():
+                        if j==None:
+                            j='Default'
+                        elif 'scaler' in str(i):
+                            j=float(j)
+                        else:
+                            j=str(j)
+                        window_OvsO_plot_settings[i].update(value=j)
                 # if the user clicks OK, save the settings selected. 
                 elif event_OvsO_plot_settings == "OK":
                     try:
                         order_vs_overlay_plot_settings["y_unit"] = str(values_OvsO_plot_settings["y_unit"])
-                        main_size_scaler = float(values_OvsO_plot_settings["main_size_scaler"])
-                        popup_scaler = float(values_OvsO_plot_settings["popup_size_scaler"])
+                        main_size_scaler = float(values_OvsO_plot_settings["size_scaler1"])
+                        popup_scaler = float(values_OvsO_plot_settings["popup_scaler"])
                         colour_scaler = float(values_OvsO_plot_settings["colour_scaler"])
                         if values_OvsO_plot_settings["contour_resolution"] not in [None,'Default']:
                             order_vs_overlay_plot_settings["contour_resolution"]=float(values_OvsO_plot_settings["contour_resolution"])
                         else:
                             order_vs_overlay_plot_settings["contour_resolution"]=None 
                         datapoints = values_OvsO_plot_settings["datapoints"]
                         annotate = values_OvsO_plot_settings["annotate"]
                         interval = values_OvsO_plot_settings["interval"]
-                        plot_score_interval=values_OvsO_plot_settings["plot_score_interval"]
+                        plot_score_interval=values_OvsO_plot_settings["score_interval"]
                         show_legend_popup = values_OvsO_plot_settings["show_legend_popup"]
                         show_legend_main = values_OvsO_plot_settings["show_legend_main"]
                         zoom_range = str(values_OvsO_plot_settings["zoom"])
                         decimals_cbar = values_OvsO_plot_settings["decimals_cbar"]
                         order_vs_overlay_plot_settings["decimals_cbar"]=decimals_cbar
-                        if values_OvsO_plot_settings["contour_cbar_max"] not in [None,'Default']:
+                        if values_OvsO_plot_settings["contour_cbar_max"] not in [None,'Default','']:
                             order_vs_overlay_plot_settings["contour_cbar_max"] = float(values_OvsO_plot_settings["contour_cbar_max"])
                         else:
                             order_vs_overlay_plot_settings["contour_cbar_max"] = None
-                        if values_OvsO_plot_settings["contour_cbar_min"] not in [None,'Default']:
+                        if values_OvsO_plot_settings["contour_cbar_min"] not in [None,'Default','']:
                             order_vs_overlay_plot_settings["contour_cbar_min"] = float(values_OvsO_plot_settings["contour_cbar_min"])
                         else:
                             order_vs_overlay_plot_settings["contour_cbar_min"]=None
                         # Define the datapoint and interval settings by bolean values.
                         if datapoints=='True':
                             order_vs_overlay_plot_settings["datapoints"] = True
                         else:
@@ -848,24 +1622,25 @@
                             raise ValueError("Invalid score interval for plot. Must be above 0.")
                         if not (0.1 < main_size_scaler <= 3):
                             raise ValueError("Invalid figure size scaler. Must be between 0.1 and 3.")
                         if not (0.1 < popup_scaler <= 3):
                             raise ValueError("Invalid popup figure size scaler. Must be between 0.1 and 3.")
                         if not (0 < colour_scaler <= 2):
                             raise ValueError("Invalid contour plot colour bar scaler. Must be between 0 and 2")
+                        if float(plot_score_interval)<=0:
+                            raise ValueError("Invalid overlay score interval. Must be above 0.")
                         if zoom_range!='None':
                             if not (0 < float(zoom_range) <= float(calculation_settings["order_range"][-1]-calculation_settings["order_range"][0])+2):
                                 raise ValueError("The zoom range defines the breadth of order values shown in the\
  order versus overlay plot, and can't be below 0 and should't be much higher than the order range of the calculation")
                         # Save the relevant settings if no error was produced. 
                         order_vs_overlay_plot_settings["size_scaler1"] = main_size_scaler
                         order_vs_overlay_plot_settings["popup_scaler"] = popup_scaler
                         order_vs_overlay_plot_settings["colour_scaler"] = colour_scaler
-                        order_vs_overlay_plot_settings["custom_title"]= str(values_OvsO_plot_settings["custom_title"])
-                        order_vs_overlay_plot_settings["plot_score_interval"]=float(plot_score_interval)
+                        order_vs_overlay_plot_settings["score_interval"]=float(plot_score_interval)
                         if zoom_range=='None' or len(zoom_range)==0:
                             order_vs_overlay_plot_settings["zoom"]='None'
                         else:
                             order_vs_overlay_plot_settings["zoom"]= float(zoom_range)
                     except ValueError as e:
                         sg.popup_error(f"Invalid input: {e}")
                         continue
@@ -874,58 +1649,91 @@
 
         elif event == "Overlay Plot Settings":
             # Create the layout for the plot settings menu. 
             # The pinned settings are for when the user selects to show the fitted curve and or overlay score value. 
             # This opens up extra settings like which polynomial degree and which constraint to apply. 
             layout_settings = [
                 [sg.Text("Overlay Plot Settings", font=("helvetica", 12, "bold"))],
-                [sg.Text("Concentration unit:       "),
-                sg.InputText(key="y_unit", size=(5, 1), default_text=str(overlay_plot_settings["y_unit"]))],
-                [sg.Text("tT axis label scaler:      "),
-                sg.InputText(key="tt_scaler", size=(5, 1), default_text=str(overlay_plot_settings["tt_scaler"]))],
-                [sg.Text("tT axis number notation:"),
-                sg.Combo(['Automatic','Normal', 'Scientific'],size=(7, 1), default_value=str(overlay_plot_settings['tT_notation']), key="tT_notation", enable_events=True, readonly=True)],
-                [sg.Text("Datapoint size scaler:   "),
-                sg.InputText(key="DP_scaler", size=(5, 1), default_text=str(overlay_plot_settings["DP_scaler"]))],
-                [sg.Text("Line width scaler:         "),
-                sg.InputText(key="line_scaler", size=(5, 1), default_text=str(overlay_plot_settings["line_scaler"]))],
-                [sg.Text("x-axis tick label rotation:"),
-                sg.InputText(key="xtick_rotation", size=(5, 1), default_text=str(overlay_plot_settings["xtick_rotation"]))],
-                [sg.Text("Figure size scaler:        "),
-                sg.InputText(key="size_scaler", size=(5, 1), default_text=str(overlay_plot_settings["size_scaler"]))],
-                [sg.Text("Show gridlines:            "),
+                [sg.Frame("Axis Settings", layout=[
+                [sg.Text("Conc. unit:"),
+                sg.InputText(key="y_unit", size=(4, 1), default_text=str(overlay_plot_settings["y_unit"])),
+                sg.Text("x-tick label rotation:"),
+                sg.InputText(key="xtick_rotation", size=(4, 1), default_text=float(overlay_plot_settings["xtick_rotation"]))
+                ],
+                [sg.Text("x-axis number type:"),
+                sg.Combo(['Automatic','Normal', 'Scientific'],size=(9, 1), default_value=str(overlay_plot_settings['tT_notation']), key="tT_notation", enable_events=True, readonly=True)]
+                ])],
+                [sg.Frame("Size Scalers", layout=[
+                [sg.Text("Linewidth scaler:"),
+                sg.InputText(key="line_scaler", size=(4, 1), default_text=float(overlay_plot_settings["line_scaler"])),
+                sg.Text("Figure scaler:"),
+                sg.InputText(key="size_scaler", size=(4, 1), default_text=float(overlay_plot_settings["size_scaler"]))],
+                [sg.Text("Datapoint scaler:"),
+                sg.InputText(key="DP_scaler", size=(4, 1), default_text=float(overlay_plot_settings["DP_scaler"])),
+                sg.Text("x-label scaler:"),
+                sg.InputText(key="tt_scaler", size=(4, 1), default_text=float(overlay_plot_settings["tt_scaler"]))]
+                ])],
+
+                [sg.Frame("Other Settings", layout=[
+                [sg.Text("Show legend: "),
+                sg.Combo(['True', 'False'],size=(5, 1), default_value=str(overlay_plot_settings['legend']), key="legend", enable_events=True, readonly=True),
+                sg.Text("Gridlines:"),
                 sg.Combo(['True', 'False'],size=(5, 1), default_value=str(overlay_plot_settings['grid']), key="grid", enable_events=True, readonly=True)],
-                [sg.Text("Show legend:              "),
-                sg.Combo(['True', 'False'],size=(5, 1), default_value=str(overlay_plot_settings['legend']), key="legend", enable_events=True, readonly=True)],
-                [sg.Text("Legend position:          "),
+                [sg.Text("Legend position:"),
                 sg.Combo(['Inside','Outside'],size=(5, 1), default_value=str(overlay_plot_settings['legend_position']), key="legend_position", enable_events=True, readonly=True)],
                 [sg.Text("Custom title:"),
-                sg.InputText(key="custom_title", size=(22, 1),default_text=str(overlay_plot_settings["custom_title"]) if overlay_plot_settings["custom_title"]!=None else 'Default')],
+                sg.InputText(key="custom_title", size=(24, 1),default_text=str(overlay_plot_settings["custom_title"]) if overlay_plot_settings["custom_title"]!=None else 'Default')]
+                ])],
                 [sg.Checkbox("Calculate overlay score", key='check_score',default=overlay_plot_settings["check_score"],enable_events=True),
                     sg.Checkbox("Show fit function", key='check_fit',default=overlay_plot_settings["check_fit"],enable_events=True)],
-                [sg.pin(sg.Text("Constraint:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key="constraint_text")),sg.pin(sg.Combo(['monotonic', 'None', 'through origin'],
-                        default_value=overlay_plot_settings["constraint"],
-                        key="constraint", enable_events=True, readonly=True,visible=overlay_plot_settings['score_settings_visibility']))],
-                [sg.pin(sg.Text("Degree:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='deg_text')),sg.pin(sg.Combo([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], default_value=overlay_plot_settings["deg"],
+                [sg.pin(sg.Text("Constraint:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key="constraint_text")),sg.pin(sg.Combo(['Monotonic', 'None', 'Via origin'],
+                        default_value=overlay_plot_settings["constraint"],size=(9, 1),
+                        key="constraint", enable_events=True, readonly=True,visible=overlay_plot_settings['score_settings_visibility'])),
+                sg.pin(sg.Text("Degree:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='deg_text')),sg.pin(sg.Combo([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], default_value=overlay_plot_settings["deg"],
                         key="deg",enable_events=True, readonly=True,visible=overlay_plot_settings['score_settings_visibility']))],
-                [sg.pin(sg.Text("Goodness-of-Fit Measurement:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='GOF_text')),sg.pin(sg.Combo(['SE', 'RMSE', 'R2', 'Variance'],
-                        default_value=overlay_plot_settings["fit_metric"],
+                [sg.pin(sg.Text("Goodness-of-fit measurement:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='GOF_text')),sg.pin(sg.Combo(['SE', 'RMSE', 'R2', 'Variance'],
+                        default_value=overlay_plot_settings["fit_metric"],size=(8, 1),
                         key="fit_metric", enable_events=True, readonly=True,visible=overlay_plot_settings['score_settings_visibility']))],
-                [sg.pin(sg.Text("Show Extra Legend:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='extra_legend_text')),sg.pin(sg.Combo(['True','False'], default_value=overlay_plot_settings["extra_legend"],
+                [sg.pin(sg.Text("Show fit function legend:",enable_events=True,visible=overlay_plot_settings['score_settings_visibility'],key='extra_legend_text')),sg.pin(sg.Combo(['True','False'], default_value=overlay_plot_settings["extra_legend"],
                         key="extra_legend",enable_events=True, readonly=True,visible=overlay_plot_settings['score_settings_visibility']))],
-                [sg.Button("OK"), sg.Button("Cancel")]
+                [sg.Button("OK"), sg.Button("Cancel"), sg.Button("Reset settings")]
             ]
             # Create the overlay plot settings window. 
             window_overlay_settings = sg.Window("Overlay Plot Settings", layout_settings,resizable=True)
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event_overlay_settings, values_overlay_settings = window_overlay_settings.read()
                 if event_overlay_settings == sg.WIN_CLOSED or event_overlay_settings == "Cancel":
                     break
-                elif event_overlay_settings in ['check_score','check_fit']:
+                # Update to the default settings if the user presses the reset settings button. 
+                elif event_overlay_settings=='Reset settings':
+                    # Loop through the elements of the default overlay plot settings and apply these
+                    # to the overlay settings window.
+                    for i,j in default_overlay_plot_settings.items():
+                        if 'scaler' in i:
+                            j=float(j)
+                        elif i=='custom_title':
+                            j='Default'
+                        else:
+                            j=str(j)
+                        if i not in ['score_settings_visibility','save','saved_values']:
+                            window_overlay_settings[i].update(value=j)
+                    window_overlay_settings['check_fit'].update(value=False)
+                    window_overlay_settings['check_score'].update(value=False)
+                    # Set all the extra settings to be invisible
+                    overlay_plot_settings['score_settings_visibility']=False
+                    window_overlay_settings["constraint_text"].update(visible=False)
+                    window_overlay_settings["constraint"].update(visible=False)
+                    window_overlay_settings["deg_text"].update(visible=False)
+                    window_overlay_settings["deg"].update(visible=False)
+                    window_overlay_settings["GOF_text"].update(visible=False)
+                    window_overlay_settings["fit_metric"].update(visible=False)
+                    window_overlay_settings["extra_legend"].update(visible=False)
+                    window_overlay_settings["extra_legend_text"].update(visible=False)
+                if event_overlay_settings in ['check_score','check_fit']:
                     # If one of the check boxes for overlay score or show the fit curve have been modified, check whether the
                     # boxes are ticked (values True). If one or both of these are True, define the visibility variable as True and 
                     # use this to make the extra settings visible. 
                     if values_overlay_settings['check_score']==True or values_overlay_settings['check_fit']==True:
                         visibility=True
                     else:
                         visibility=False
@@ -970,17 +1778,17 @@
                         if legend_bol=='True':
                             overlay_plot_settings["legend"]=True
                         else:
                             overlay_plot_settings["legend"]=False
                         # Check if the selected values are valid. Raise errors if not. 
                         if deg not in [1, 2, 3, 4, 5, 6, 7,8,9,10,11,12,13]:
                             raise ValueError("Invalid degree. Must be an integer between 1 and 13.")
-                        if constraint=='through origin':
+                        if constraint=='Via origin':
                             if int(deg)!=1:
-                                raise ValueError("Set fitting degree to 1 for linear line through origin.")
+                                raise ValueError("Set fitting degree to 1 for linear line via origin.")
                         if not (0.1 < size_scaler <= 3):
                             raise ValueError("Invalid figure size scaler. Must be between 0.1 and 3.")
                         if not (0.1 < tt_scaler <= 3):
                             raise ValueError("Invalid figure transformed time axis label scaler. Must be between 0.1 and 3.")
                         if not (0.00 <= DP_scaler <= 5):
                             raise ValueError("Invalid datapoint size scaler. Must be between 0 and 5.")
                         if not (0.00 <= xtick_rotation <= 180):
@@ -992,15 +1800,15 @@
                         overlay_plot_settings["xtick_rotation"]=xtick_rotation
                     except ValueError as e:
                             sg.popup_error(f"Invalid input: {e}")
                             continue
                     window_overlay_settings.close()
             window_overlay_settings.close()
 
-        elif event == "Plot Results":
+        elif event == "Plot results":
             # Plot the results from the automatic VTNA calculation using settings from the over_vs_overlay_plot_settings dictionary. 
             try:
                 # Check the dimensionality of the overlay score versus order matrix to see if a graph (one dimension) or contour plot 
                 # (two dimensions) can be produced.
                 no_dimensions=-len(fixed_orders.values())+len(selected_columns)
                 if no_dimensions>2:
                     raise ValueError("Can't plot results for more than two normalised reaction species to investigate.")
@@ -1017,27 +1825,27 @@
                 # Create the figure and save it as a variable img.
                 img=VTNA_auto_calculation.plot_orders_vs_overlay(y_unit=order_vs_overlay_plot_settings["y_unit"],size_scaler=order_vs_overlay_plot_settings["size_scaler1"],
                 size_scaler2=order_vs_overlay_plot_settings["popup_scaler"],color_scaler=order_vs_overlay_plot_settings["colour_scaler"],
                 fixed_cbar_resolution=order_vs_overlay_plot_settings["contour_resolution"],points=order_vs_overlay_plot_settings["datapoints"],
                 interval=order_vs_overlay_plot_settings["interval"],zoom=zoom_range,overlay_score_range_max=order_vs_overlay_plot_settings["contour_cbar_max"],
                 overlay_score_range_min=order_vs_overlay_plot_settings["contour_cbar_min"],title=custom_title,show_legend_popup=order_vs_overlay_plot_settings["show_legend_popup"],
                 show_legend_main=order_vs_overlay_plot_settings["show_legend_main"],decimals_in_colorbar=order_vs_overlay_plot_settings["decimals_cbar"],
-                annotate_optimum=order_vs_overlay_plot_settings["annotate"],specified_score_interval=order_vs_overlay_plot_settings['plot_score_interval'])
+                annotate_optimum=order_vs_overlay_plot_settings["annotate"],specified_score_interval=order_vs_overlay_plot_settings['score_interval'])
             except ValueError as e:
                 sg.popup_error(f"Invalid input: {e}")
                 continue
         
         elif event == "Generate Overlay Plot":
             # Ensure that all exisiting plots are closed to avoid bugs.
             plt.close('all')
             # Define the selected experiments, selected columns and selected output species
             # for generating the correct VTNA overlay plot. 
             selected_sheet = values["experiments"]
             selected_columns = values["columns"]
-            selected_result_columns = values["result_columns"]
+            selected_result_column = values["result_column"]
             # Define keyword arguments from the overlay_plot_settings dictionary. 
             tt_scaler=overlay_plot_settings['tt_scaler']
             DP_scaler=float(overlay_plot_settings["DP_scaler"])
             line_scaler=float(overlay_plot_settings["line_scaler"])
             xtick_rotation=float(overlay_plot_settings["xtick_rotation"])
             y_unit=overlay_plot_settings['y_unit']
             size_scaler=overlay_plot_settings['size_scaler']
@@ -1053,27 +1861,30 @@
             legend_bol=overlay_plot_settings['legend']
             if overlay_plot_settings['legend_position']=='Inside':
                 legend_outside=False
             else:
                 legend_outside=True
             if overlay_plot_settings['custom_title'] in ['','None']:
                 title=None
-            if selected_sheet and selected_columns and selected_result_columns:
+            if selected_sheet and selected_columns and selected_result_column:
                 # Open a pop-up window to input order values for selected fixed order species
                 if selected_columns:
                     layout_order_values = [
                         [sg.Text(f"Enter order values for selected species:")],
                     ]
                     # Add a text and input text element for each normalised species to allow the user to input order values. 
+                    species_column=[]
+                    orders_column=[]
                     for species in selected_columns:
+                        species_column.append([sg.Text(f"{species}:")])
                         if overlay_plot_settings['save'] and species in list(overlay_plot_settings['saved_values'].keys()):
-                            species_input=[sg.Text(f"{species}"), sg.InputText(key=f"order_value_{species}", size=(5, 1),enable_events=True,default_text=overlay_plot_settings['saved_values'][species])]
+                            orders_column.append([sg.InputText(key=f"order_value_{species}", size=(5, 1),enable_events=True,default_text=overlay_plot_settings['saved_values'][species])])
                         else:
-                            species_input=[sg.Text(f"{species}"), sg.InputText(key=f"order_value_{species}", size=(5, 1),enable_events=True)]
-                        layout_order_values.append(species_input)
+                            orders_column.append([sg.InputText(key=f"order_value_{species}", size=(5, 1),enable_events=True)])
+                    layout_order_values.append([sg.Column(species_column,element_justification='left'),sg.Column(orders_column,element_justification='left')])
                     # Define the OK and cancel buttons for the pop-up menu.
                     buttons=[sg.Button("OK"), sg.Button("Cancel")]
                     # If optimal order values have been calculated by automatic VTNA, and some of these reaction species have 
                     # been selected for the overlay plot, create a button for auto-filling these calculated order values. 
                     if len(best_order_dict)!=0:
                         if [i in selected_columns for i in list(best_order_dict.keys())]:
                             buttons.append(sg.Button("Auto-fill calculated values.",key='auto'))
@@ -1135,15 +1946,15 @@
                                 order_values[species] = str(values_order_values[f"order_value_{species}"])
                             # If input is valid, break out of the loop
                             if input_valid:
                                 # Save the final order values to the overlay_plot_settings dictionary. 
                                 if overlay_plot_settings['save']:
                                     overlay_plot_settings['saved_values']=order_values
                                 # Generate the overlay plot using the overlay_plot function. 
-                                overlay_plot(data,selected_sheet,order_values,selected_result_columns[0],tt_scaler=tt_scaler,\
+                                overlay_plot(data,selected_sheet,order_values,selected_result_column[0],tt_scaler=tt_scaler,\
                                          grid=grid,y_unit=y_unit,size_scaler=size_scaler,title=title, fit_metric=fit_metric,
                                          deg=deg,constraint=constraint,show_overlay_score=show_overlay_score,\
                                          show_fit_function=show_fit_function,DP_scaler=DP_scaler,xtick_rotation=xtick_rotation,\
                                          show_legend=legend_bol,legend_outside=legend_outside,extra_legend=extra_legend,\
                                          line_scaler=line_scaler,tT_notation=tT_notation)
             else:
                 sg.popup_error("Please select experiments, reaction species, and output reaction species before generating overlay plot.")
@@ -1167,72 +1978,85 @@
                             sg.Checkbox("", key=f"Check_{compound}", enable_events=True,default=True),
                             sg.InputText(key=f"Value_{compound}", visible=True,size=(5,1),
                             default_text=str(fixed_orders_start[compound]))])
                 else:
                     layout_fixed_order.append([
                         sg.Text(compound, size=(label_width, 1)),
                         sg.Checkbox("", key=f"Check_{compound}", enable_events=True),
-                        sg.InputText(key=f"Value_{compound}", visible=False,size=(5,1),
+                        sg.InputText(key=f"Value_{compound}", visible=False,size=(5,1),enable_events=True,
                         )])
             # Define the main layout of the calculation settings window. 
             layout_settings = [
             [sg.Text("Calculation Settings", font=("helvetica", 12, "bold"))],
             [sg.Frame("Fit Settings", layout=[
                 [sg.Text("Constraint:"),
-                sg.Combo(['monotonic', 'None', 'through origin'],
+                sg.Combo(['Monotonic', 'None', 'Via origin'],
                         default_value=calculation_settings["constraint"],
-                        key="constraint", enable_events=True, readonly=True,size=(11,1)),
+                        key="constraint", enable_events=True, readonly=True,size=(8,1)),
                 sg.Text("Degree:"),
-                sg.Combo([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], default_value=calculation_settings["deg"], key="deg")],
+                sg.Combo([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], default_value=calculation_settings["deg"], key="deg",size=(3,1))],
                 [sg.Text("Goodness-of-fit metric:"),
                 sg.Combo(['SE', 'RMSE', 'R2', 'Variance'], default_value=calculation_settings["fit_metric"],
                         key="fit_metric", enable_events=True, readonly=True,size=(8,1))],
             ])],
-            [sg.Frame("Order exploration settings", layout=[
+            [sg.Frame("Order Exploration Settings", layout=[
                 [sg.Text("Iterations:"),
                 sg.Combo([1, 2, 3, 4, 5, 6, 7,8,9,10,11,12], default_value=calculation_settings["iterations"], key="iterations"),
                 sg.Text("Order grid density:"),
                 sg.InputText(key="resolution", size=(3, 1),
                             default_text=str(calculation_settings["resolution"]))],
                 [sg.Text("Higher initial order mesh density:"),
                 sg.Combo(['True','False'], default_value=str(calculation_settings["initial_mesh_denser"]),
                             key='initial_mesh_denser', enable_events=True, readonly=True,size=(6,1))]
             ])],
             [sg.Button("Standard settings",key='standard'),sg.Button("Quick settings",key='quick')],
-            [sg.Frame("Order range to explore", layout=[
+            [sg.Frame("Order Range to Explore", layout=[
                 [sg.Text("From"),
                 sg.InputText(key="order_range_low", size=(4, 1),
                             default_text=str(calculation_settings["order_range"][0])),
                 sg.Text("to"),
                 sg.InputText(key="order_range_high", size=(4, 1),
                             default_text=str(calculation_settings["order_range"][1]))]
             ]),
             sg.Frame("Score Interval", layout=[
                 [sg.Text("Interval:"),
                 sg.InputText(key="score_interval", size=(4, 1),
                             default_text=str(calculation_settings["score_interval"]))]
             ])],
             [sg.Frame("Fixed Order Species", layout=layout_fixed_order)],
-            [sg.Button("OK"), sg.Button("Cancel")]]
+            [sg.Button("OK"), sg.Button("Cancel"),sg.Button("Reset settings")]]
 
             window_settings = sg.Window("Calculation Settings", layout_settings)
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event_settings, values_settings = window_settings.read()
                 if event_settings == sg.WIN_CLOSED or event_settings == "Cancel":
                     break
+                # Reset the calculation settings if the reset button is pressed. 
+                elif event_settings=='Reset settings':
+                    # Loop through the elements of the default overlay plot settings and apply these
+                    # to the overlay settings window.
+                    for i,j in default_calculation_settings.items():
+                        if i not in ['order_range','fixed_order_species']:
+                            window_settings[i].update(value=str(j))
+                    window_settings["order_range_low"].update(value=default_calculation_settings['order_range'][0])
+                    window_settings["order_range_high"].update(value=default_calculation_settings['order_range'][1])
+                    for compound in columns:
+                        window_settings[f"Check_{compound}"].update(value=False)
+                        window_settings[f"Value_{compound}"].update(value='')
+                        window_settings[f"Value_{compound}"].update(visible=False)
                 # Apply the quick settings if the Quick button is pressed. 
                 elif event_settings=='quick':
                     window_settings['constraint'].update(value='None')
                     window_settings['resolution'].update(value=4)
                     window_settings['iterations'].update(value=10)
                     window_settings["initial_mesh_denser"].update(value='False')
                 # Apply the standard calculation settings if the Standard settings button is pressed.
                 elif event_settings=='standard':
-                    window_settings['constraint'].update(value='monotonic')
+                    window_settings['constraint'].update(value='Monotonic')
                     window_settings['resolution'].update(value=7)
                     window_settings['iterations'].update(value=7)
                     window_settings["initial_mesh_denser"].update(value='True')
                 # Update the fixed order species frame if the user has ticked or unticked one of the boxes.
                 elif event_settings.startswith("Check_"):
                     window_settings[event_settings.replace('Check_','Value_')].update(visible=values_settings[event_settings])
                     if values_settings[event_settings]==False:
@@ -1256,29 +2080,29 @@
                         if not (-3 <= order_range_low < order_range_high <= 3.5):
                             raise ValueError("Invalid order range. Must be between -3 and 3.5 with the first value lower than the second.")
                         # Check if the selected fit metric is valid
                         if fit_metric not in ['SE', 'RMSE', 'R2', 'Variance']:
                             raise ValueError("Invalid fit metric. Must be one of: 'SE', 'RMSE', 'R2', 'Variance'.")
                         # Check constraint
                         constraint = values_settings["constraint"]
-                        if constraint not in ['monotonic', 'None', 'through origin']:
-                            raise ValueError("Invalid constraint. Must be 'monotonic', 'None', or 'through origin'.")
+                        if constraint not in ['Monotonic', 'None', 'Via origin']:
+                            raise ValueError("Invalid constraint. Must be 'Monotonic', 'None', or 'Via origin'.")
 
                         # Check score interval
                         if not (0 <= score_interval <= 100):
                             raise ValueError("Invalid score interval. Must be between 0 and 100.")
                         # Check resolution
                         if not (4 <= resolution <= 30):
                             raise ValueError("Invalid score interval. Must be between 4 and 30.")
                         # Check degree
                         if deg not in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10,11, 12, 13]:
                             raise ValueError("Invalid degree. Must be an integer between 1 and 13.")
-                        if constraint=='through origin':
+                        if constraint=='Via origin':
                             if int(deg)!=1:
-                                raise ValueError("Set fitting degree to 1 for linear line through origin.")
+                                raise ValueError("Set fitting degree to 1 for linear line via origin.")
                     except ValueError as e:
                         sg.popup_error(f"Invalid input: {e}")
                         continue
                     # Save the calculation settings
                     calculation_settings["constraint"] = constraint
                     calculation_settings["order_range"] = [order_range_low, order_range_high]
                     calculation_settings["iterations"] = round(iterations)
@@ -1293,15 +2117,15 @@
                         calculation_settings["fixed_order_species"]=None
                     break
             window_settings.close()
 
         elif event == "Select CSVs":
             # Define counter to know which browse and input text elements to make visible. 
             count=1
-            sg.theme("DefaultNoMoreNagging")
+            #sg.theme("DefaultNoMoreNagging")
             # Define layout with one set of visible InputText and FilesBrowse elements and several hidden ones. 
             layout = [
                 [sg.Text("NB: If >1 file in same browse, alternative names can't be given.\nIf a file is uploaded more than once, the duplicate(s) will be removed.")],
                 [sg.InputText(key="file_name_1", enable_events=True, size=(18, 1)),sg.FilesBrowse(key="browse_1"),sg.Text("Data name (optional):",key="text_1"),sg.InputText(key="nickname_1", size=(10, 1))],
                 [sg.InputText(key="file_name_2", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_2",visible=False),sg.Text("Data name (optional):",visible=False,key="text_2"),sg.InputText(key="nickname_2", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_3", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_3",visible=False),sg.Text("Data name (optional):",visible=False,key="text_3"),sg.InputText(key="nickname_3", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_4", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_4",visible=False),sg.Text("Data name (optional):",visible=False,key="text_4"),sg.InputText(key="nickname_4", size=(10, 1),visible=False)],
@@ -1310,103 +2134,123 @@
                 [sg.InputText(key="file_name_7", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_7",visible=False),sg.Text("Data name (optional):",visible=False,key="text_7"),sg.InputText(key="nickname_7", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_8", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_8",visible=False),sg.Text("Data name (optional):",visible=False,key="text_8"),sg.InputText(key="nickname_8", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_9", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_9",visible=False),sg.Text("Data name (optional):",visible=False,key="text_9"),sg.InputText(key="nickname_9", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_10", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_10",visible=False),sg.Text("Data name (optional):",visible=False,key="text_10"),sg.InputText(key="nickname_10", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_11", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_11",visible=False),sg.Text("Data name (optional):",visible=False,key="text_11"),sg.InputText(key="nickname_11", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_12", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_12",visible=False),sg.Text("Data name (optional):",visible=False,key="text_12"),sg.InputText(key="nickname_12", size=(10, 1),visible=False)],
                 [sg.InputText(key="file_name_13", enable_events=True, size=(18, 1),visible=False), sg.FilesBrowse(key="browse_13",visible=False),sg.Text("Data name (optional):",visible=False,key="text_13"),sg.InputText(key="nickname_13", size=(10, 1),visible=False)],
-                [sg.Button("Add File", key="add_file"), sg.Button("OK")]
+                [sg.Button("OK")]
             ]
             # Create the window.
             window_csv = sg.Window("CSV Loader", layout)
             pattern = re.compile(r'/([^/]+)\.csv$')
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event, values = window_csv.read()
+                if event == sg.WIN_CLOSED:
+                    break
+                elif event == "OK":
+                    try:
+                        values_not_nickname=[i[1] for i in list(values.items()) if 'nickname' not in i[0] and i[1]!='']
+                        if len(values_not_nickname)==0:
+                            break
+                        file_names=[]
+                        file_paths_full=[]
+                        for key,value in values.items():
+                            # Loop through all the keys and values in the values of the window_csv.
+                            if value==None:
+                                break
+                            elif "file_name" in key and len(value)!=0:
+                                file_paths = value.split(';')
+                                file_paths_full=file_paths_full+file_paths
+                                # Obtain the index number of the file_name text.
+                                index=''.join(char for char in key if char.isdigit())
+                                # Obtain the corresponding nickname from the values dictionary. 
+                                name=values[f"nickname_{int(index)}"]
+                                for i in file_paths:
+                                    # Identify the file name from the file path if no nickname has been specified.
+                                    if len(name)==0 or len(file_paths)!=1:
+                                        name_search = pattern.search(i)
+                                        name=name_search.group(1)
+                                        file_names.append(name)
+                                    else:
+                                        file_names.append(name)
+                        # Check the file paths and file names lists for duplicates. 
+                        # Makes new lists that are guaranteed not to have duplicates. 
+                        file_paths_no_duplicates,file_names_no_duplicates=[],[]
+                        for count,(i,j) in enumerate(zip(file_paths_full,file_names)):
+                            if i not in file_paths_full[:count]:
+                                file_paths_no_duplicates.append(i)
+                                file_names_no_duplicates.append(j)
+                        # Loop through the file paths and create the kinetic data dictionary. 
+                        kinetic_data={}
+                        for (i,j) in zip(file_paths_no_duplicates,file_names_no_duplicates):
+                            dataset=pd.read_csv(f"{i}")
+                            # Convert column titles to strings. 
+                            dataset.columns = dataset.columns.astype(str)
+                            kinetic_data[j]=dataset
+                        # Define data as a copy of the kinetic data which is not altered later in the code. 
+                        # This allows the original data to be accessed even if the copy is altered. 
+                        data = kinetic_data.copy()
+                        omission_range_dictionary={}
+                        omission_range_dictionary["range_type"]='Percentage'
+                        # Figure out if default data cropping mode should be datapoints or range.
+                        df_nrows=[]
+                        for i in kinetic_data.keys():
+                            df_nrows.append(kinetic_data[i].shape[0])
+                        if max(df_nrows)>25:
+                            omission_mode='Range mode'
+                        else:
+                            omission_mode='Datapoint mode'
+                        # Update the time label and the experiments, column and fixed order species. 
+                        time_label=list(data.values())[0].columns[0]
+                        experiments = list(data.keys())
+                        columns = data[experiments[0]].columns[1:].tolist()  # Exclude the first column
+                        # Create a list of reaction species that have concentration profiles that change over time. 
+                        reaction_species_not_constant=data[experiments[0]].columns[1:].tolist()
+                        for exp in data.keys():
+                            for species in columns:
+                                # Avoid trying to remove a constant species twice. 
+                                if species in reaction_species_not_constant:
+                                    # Define the list of concentration values for the relevant species in the relevant experiment. 
+                                    values=list(data[exp][species].to_numpy())
+                                    # If all values are the same, remove this species from the not constant list
+                                    if all([species==values[0] for species in values]):
+                                        reaction_species_not_constant.remove(species)
+                        fixed_order_species = data[experiments[0]].columns[1:].tolist()  # All reaction species
+                        # Update the sheet, columns and result column listboxes with the relevant data
+                        # (Sheet names, reactant names and reactant names respectively)
+                        window["experiments"].update(values=experiments)
+                        window["columns"].update(values=columns)
+                        window["result_column"].update(values=reaction_species_not_constant)
+                        # Enable various buttons now that the kinetic data has been loaded. 
+                        window["Run Auto VTNA"].update(disabled=False)  
+                        window["calculation_settings"].update(disabled=False)  
+                        window["Check Kinetic Data"].update(disabled=False) 
+                        window["Inspect Kinetic Data"].update(disabled=False)
+                        window["Generate Overlay Plot"].update(disabled=False)
+                        window["Overlay Plot Settings"].update(disabled=False)
+                        window["Crop Kinetic Data"].update(disabled=False)
+                        files_calculation=file_paths_no_duplicates
+                        break
+                    except ValueError as e:
+                        sg.popup_error(f"Error: {e}")
+                        continue
                 # If a file is browsed, make the next InputText and FilesBrowser visible. 
                 if 'file_name' in event and event[-1]==str(count):
                     file_paths = values[event].split(';')
                     if len(file_paths)>1:
                         window_csv[f"nickname_{count}"].update(visible=False)
                         window_csv[f"text_{count}"].update(visible=False)
                     count+=1
                     window_csv[f"file_name_{count}"].update(visible=True)
                     window_csv[f"browse_{count}"].update(visible=True)
                     window_csv[f"text_{count}"].update(visible=True)
                     window_csv[f"nickname_{count}"].update(visible=True)
                 # If the window is closed, collect the filenames selected as a list.
-                elif event == sg.WIN_CLOSED or event == "OK":
-                    file_paths_full=[]
-                    file_names=[]
-                    for key,value in values.items():
-                        # Loop through all the keys and values in the values of the window_csv.
-                        if value==None:
-                            break
-                        elif "file_name" in key and len(value)!=0:
-                            file_paths = value.split(';')
-                            file_paths_full=file_paths_full+file_paths
-                            # Obtain the index number of the file_name text.
-                            index=''.join(char for char in key if char.isdigit())
-                            # Obtain the corresponding nickname from the values dictionary. 
-                            name=values[f"nickname_{int(index)}"]
-                            for i in file_paths:
-                                # Identify the file name from the file path if no nickname has been specified.
-                                if len(name)==0 or len(file_paths)!=1:
-                                    name_search = pattern.search(i)
-                                    name=name_search.group(1)
-                                    file_names.append(name)
-                                else:
-                                    file_names.append(name)
-                    # Check the file paths and file names lists for duplicates. 
-                    # Makes new lists that are guaranteed not to have duplicates. 
-                    file_paths_no_duplicates,file_names_no_duplicates=[],[]
-                    for count,(i,j) in enumerate(zip(file_paths_full,file_names)):
-                        if i not in file_paths_full[:count]:
-                            file_paths_no_duplicates.append(i)
-                            file_names_no_duplicates.append(j)
-                    # Loop through the file paths and create the kinetic data dictionary. 
-                    kinetic_data={}
-                    for (i,j) in zip(file_paths_no_duplicates,file_names_no_duplicates):
-                        dataset=pd.read_csv(f"{i}")
-                        # Convert column titles to strings. 
-                        dataset.columns = dataset.columns.astype(str)
-                        kinetic_data[j]=dataset
-                    # Define data as a copy of the kinetic data which is not altered later in the code. 
-                    # This allows the original data to be accessed even if the copy is altered. 
-                    data = kinetic_data.copy()
-                    omission_range_dictionary={}
-                    omission_range_dictionary["range_type"]='Percentage'
-                    # Figure out if default data cropping mode should be datapoints or range.
-                    df_nrows=[]
-                    for i in kinetic_data.keys():
-                        df_nrows.append(kinetic_data[i].shape[0])
-                    if max(df_nrows)>25:
-                        omission_mode='Range mode'
-                    else:
-                        omission_mode='Datapoint mode'
-                    # Update the time label and the experiments, column and fixed order species. 
-                    time_label=list(data.values())[0].columns[0]
-                    experiments = list(data.keys())
-                    columns = data[experiments[0]].columns[1:].tolist()  # Exclude the first column
-                    fixed_order_species = data[experiments[0]].columns[1:].tolist()  # All reaction species
-                    # Update the sheet, columns and result column listboxes with the relevant data
-                    # (Sheet names, reactant names and reactant names respectively)
-                    window["experiments"].update(values=experiments)
-                    window["columns"].update(values=columns)
-                    window["result_columns"].update(values=columns)
-                    # Enable various buttons now that the kinetic data has been loaded. 
-                    window["Run Auto VTNA"].update(disabled=False)  
-                    window["calculation_settings"].update(disabled=False)  
-                    window["Check Kinetic Data"].update(disabled=False) 
-                    window["Inspect Kinetic Data"].update(disabled=False)
-                    window["Generate Overlay Plot"].update(disabled=False)
-                    window["Overlay Plot Settings"].update(disabled=False)
-                    window["Crop Kinetic Data"].update(disabled=False)
-                    files_calculation=file_paths_no_duplicates
-                    break
             window_csv.close()
 
         elif event == "Check Kinetic Data":
             # Apply the check_kinetic_data to investigate whether it has been uploaded correctly 
             # and is ready for analysis. 
             check_kinetic_data(data)
 
@@ -1501,15 +2345,15 @@
                             ]],visible=True,key='total_frame')]
                 # Complete the layout by combining the experiment specific and total layout lists. 
                 rows_range=[remove_data_selective]+[remove_data_total]
                 # Add the final elements to the range cropping layout.
                 rows_range.append([sg.Text("Relative or absolute times"),
                                     sg.Combo(['Absolute','Percentage'], default_value=omission_range_dictionary["range_type"],
                                             key="range_type", enable_events=True, readonly=True)])
-                layout_range = rows_range + [[[sg.Button('OK')],sg.Button("Reset")]]
+                layout_range = rows_range + [[sg.Button('OK'),sg.Button("Reset")]]
                 # Create the range crop window.
                 window_range = sg.Window('Crop Data Range', layout_range)
                 # Maintain an infinite loop to process events until the window is shut down.
                 while True:
                     event_range, values_range = window_range.read()
                     if event_range=="Reset":
                         data_cropping=kinetic_data.copy()
@@ -1626,15 +2470,15 @@
                         rows.append(row_title + checkboxes)
                 else:
                 # Create the layout for the datapoint cropping window if no information has already been saved.
                     for key, df in kinetic_data.items():
                         row_title = [sg.Text(f'Row {key}')]
                         checkboxes = [sg.Checkbox(str(i), key=f'CHECK_{key}__{i}') for i in range(1, len(df[time_label]) + 1)]
                         rows.append(row_title + checkboxes)
-                layout = rows + [[sg.Button("Reset")],[sg.Button('OK')]]
+                layout = rows + [[sg.Button('OK'),sg.Button("Reset")]]
                 window_omissions = sg.Window('Select rows to reversibly remove from kinetic data.', layout)
                 # Maintain an infinite loop to process events until the window is shut down.
                 while True:
                     event_omissions, values_omissions = window_omissions.read()
                     # Remove all box ticks if the reset button is pressed by the user. 
                     if event_omissions=="Reset":
                         for key, df in kinetic_data.items():
@@ -1661,58 +2505,66 @@
         elif event == "Inspect Kinetic Data":
             # Open a new window for inspecting kinetic data
             # Ensure that all exisiting plots are closed to avoid bugs.
             plt.close('all')
             # Define the layout of the window including both buttons for different plots and 
             # the plot settings. 
             layout_inspect_kinetic_data = [
-                [sg.Button("Generate Initial Concentration Table")],
-                [sg.Button("Plot Kinetic Data")],
-                [sg.Button("Plot Kinetic Data for Selected Experiments and Species")],
-                [sg.Button("Plot Concentration Profiles")],
-                [sg.Frame("Settings", layout=[
+                [sg.Button("Generate initial concentration table")],
+                [sg.Button("Plot kinetic data")],
+                [sg.Button("Plot data for selected experiments & species")],
+                [sg.Button("Plot concentration profiles")],
+                [sg.Button('Export the kinetic dataset to .xlsx or .csv')],
+                [sg.Frame("Data Visualisation Settings", layout=[
                     [sg.Text("Concentration unit:"),
-                     sg.InputText(key="y_unit", size=(5, 1),default_text=str(data_plotting_settings["y_unit"])),
-                     sg.Text("Time unit:"),
-                     sg.InputText(key="t_unit", size=(5, 1),default_text=str(data_plotting_settings["t_unit"]))],
-                    [sg.Text("Figure size scaler:"),
-                     sg.InputText(key="size_scaler", size=(5, 1),default_text=float(data_plotting_settings["size_scaler"])),
-                     sg.Text("Max y:"),
-                     sg.InputText(key="ylim", size=(5, 1),default_text=str(data_plotting_settings["ylim"]))],
-                    [sg.Text("Datapoint size scaler:"),
-                     sg.InputText(key="DP_scaler", size=(4, 1),default_text=float(data_plotting_settings["DP_scaler"])),
+                     sg.InputText(key="y_unit", size=(5, 1),default_text=str(data_plotting_settings["y_unit"]),enable_events=True),
+                     sg.Text("Time unit: "),
+                     sg.InputText(key="t_unit", size=(5, 1),default_text=str(data_plotting_settings["t_unit"]),enable_events=True)],
+                    [sg.Text("Figure size scaler: "),
+                     sg.InputText(key="size_scaler", size=(5, 1),default_text=float(data_plotting_settings["size_scaler"]),enable_events=True),
+                     sg.Text("Max y:     "),
+                     sg.InputText(key="ylim", size=(5, 1),default_text=str(data_plotting_settings["ylim"]),enable_events=True)],
+                    [sg.Text("Datapoint scaler:   "),
+                     sg.InputText(key="DP_scaler", size=(5, 1),default_text=float(data_plotting_settings["DP_scaler"]),enable_events=True),
                      sg.Text("Linewidth:"),
-                     sg.InputText(key="linewidth", size=(4, 1),default_text=float(data_plotting_settings["linewidth"]))],
-                    [sg.Text("Legend position:"),
-                     sg.Combo(['Inside','outside'], default_value=data_plotting_settings["legend_position"],key="legend_position", enable_events=True, readonly=True)],
+                     sg.InputText(key="linewidth", size=(5, 1),default_text=float(data_plotting_settings["linewidth"]),enable_events=True)],
+                    [sg.Text("Legend position:    "),
+                     sg.Combo(['Inside','Outside'], size=(7, 1),default_value=data_plotting_settings["legend_position"],key="legend_position", enable_events=True, readonly=True)],
                     [sg.Text("Significant figures for initial conc. table:"),
-                     sg.InputText(key="SF", size=(5, 1),default_text=float(data_plotting_settings["significant_figs"]))],
+                     sg.InputText(key="SF", size=(5, 1),default_text=float(data_plotting_settings["SF"]),enable_events=True)],
                     [sg.Text("Mode for visualising kinetic data:"),sg.Combo(['Scroll', 'Together', 'Separate'], default_value=data_plotting_settings["mode"],
                             key="mode", enable_events=True, readonly=True)],
                 ])],
-                [sg.Button("Back")]
+                [sg.Button("Back"),sg.Button('Reset settings')]
             ]
             # Create the window. 
             window_inspect_kinetic_data = sg.Window("Inspect Kinetic Data", layout_inspect_kinetic_data)
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event_inspect_kinetic_data, values_inspect_kinetic_data = window_inspect_kinetic_data.read()
                 if event_inspect_kinetic_data == sg.WIN_CLOSED or event_inspect_kinetic_data == "Back":
                     break
+                # Reset the settings to the default values if the user presses reset settings. 
+                elif event_inspect_kinetic_data=='Reset settings':
+                    # Loop through the elements of the default data plotting settings and apply these
+                    # to the inspect kinetic data window.
+                    for i,j in default_data_plotting_settings.items():
+                        if 'scaler' in i or i in ['linewidth','SF']:
+                            j=float(j)
+                        else:
+                            j=str(j)
+                        window_inspect_kinetic_data[i].update(value=j)
                 # Check that the inputed settings are valid before creating any plots or table. 
-                if event_inspect_kinetic_data in ["Generate Initial Concentration Table","Plot Kinetic Data",
-                        "Plot Kinetic Data for Selected Experiments and Species","Plot Concentration Profiles"]:
+                if event_inspect_kinetic_data in ["Generate initial concentration table","Plot kinetic data",
+                        "Plot data for selected experiments & species","Plot concentration profiles"]:
                     try:
                         if not is_float(values_inspect_kinetic_data["ylim"]):
                             ylim = None
                         else: 
                             ylim = float(values_inspect_kinetic_data["ylim"])
-                        if event_inspect_kinetic_data=="Plot Kinetic Data for Selected Experiments and Species":
-                            print(values['columns'])
-                            print(values["experiments"])
                         y_unit = values_inspect_kinetic_data["y_unit"]
                         t_unit = values_inspect_kinetic_data["t_unit"]
                         if not is_float(values_inspect_kinetic_data["SF"]):
                             raise ValueError("Significant figures for initial concentration table must be a numerical value.")
                         significant_figures=int(abs(float(values_inspect_kinetic_data["SF"])))
                         data_plotting_settings["legend_position"]=values_inspect_kinetic_data["legend_position"]
                         DP_scaler = float(values_inspect_kinetic_data["DP_scaler"])
@@ -1736,39 +2588,43 @@
                             if ylim!='None' and ylim!='':
                                 raise ValueError("Concentration axis limit must be a numerical value.")
                         if significant_figures==0 or significant_figures>9:
                             raise ValueError("Significant figures for initial concentration must be between 1 and 9.")
                         if type(ylim)==str:
                             if ylim!='None' and ylim!='':
                                 raise ValueError("Concentration axis limit must be a numerical value.")
-                        data_plotting_settings["significant_figs"]=int(significant_figures)
+                        data_plotting_settings["SF"]=int(significant_figures)
                         data_plotting_settings["size_scaler"]=size_scaler
-                        data_plotting_settings["ylim"]=ylim
+                        # Ensure that the ylim setting is set to None rather than '' or 'None' if this is selected. 
+                        if ylim not in ['None','']:
+                            data_plotting_settings["ylim"]=ylim
+                        else:
+                            data_plotting_settings["ylim"]=None
                         data_plotting_settings["y_unit"]=y_unit
                         data_plotting_settings["t_unit"]=t_unit
                         data_plotting_settings["mode"]=mode
                         data_plotting_settings["DP_scaler"]=DP_scaler
                         data_plotting_settings["linewidth"]=linewidth
                     except ValueError as e:
                             sg.popup_error(f"Invalid input: {e}")
                             continue
                 # React to the specifics of the users button click. 
-                if event_inspect_kinetic_data == "Generate Initial Concentration Table":
-                    generate_initial_concentration_table(data,size_scaler,y_unit,significant_figures=data_plotting_settings["significant_figs"])
-                elif event_inspect_kinetic_data == "Plot Kinetic Data":
+                if event_inspect_kinetic_data == "Generate initial concentration table":
+                    generate_initial_concentration_table(data,size_scaler,y_unit,significant_figures=data_plotting_settings["SF"])
+                elif event_inspect_kinetic_data == "Plot kinetic data":
                     # Ask the user whether to visualise mass balance using a custom popup window.
                     layout_visualise_mass_balance = [
                         [sg.Text("Do you want to visualise mass balance for the kinetic data?")],
                         [sg.Button("Yes"), sg.Button("No")]
                     ]
                     window_visualise_mass_balance = sg.Window("Visualise Mass Balance", layout_visualise_mass_balance)
                     event_visualise_mass_balance, values_visualise_mass_balance = window_visualise_mass_balance.read()
                     window_visualise_mass_balance.close()
                     if event_visualise_mass_balance==sg.WIN_CLOSED:
-                        break
+                        continue
                     if event_visualise_mass_balance == "Yes":
                         # Use Listbox to create a multi-selection list
                         selected_species = sg.Listbox(
                             values=columns,
                             select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE,
                             size=(20, min(12, len(fixed_order_species))),
                             key="selected_species_listbox"
@@ -1782,51 +2638,60 @@
                         ]
                         window_select_species = sg.Window("Select Reaction Species", layout_select_species)
                         # Maintain an infinite loop to process events until the window is shut down.
                         while True:
                             event_select_species, values_select_species = window_select_species.read()
                             # Close the window if the user closes it or clicks cancel. 
                             if event_select_species == sg.WIN_CLOSED or event_select_species == "Cancel":
+                                window_select_species.close()
                                 break
                             elif event_select_species == "OK":
                                 selected_species_values = values_select_species["selected_species_listbox"]
                                 if not selected_species_values:
                                     sg.popup_error("Please select one or more reaction species.")
                                 else:
                                     # Query user for stoichiometry numbers.
                                     layout_stoichiometry_values = [
                                         [sg.Text(f"Enter stoichiometry values for selected reaction species:")],
                                     ]
+                                    # Define columns with reaction species and with input boxes for order values:
+                                    species_column=[]
+                                    orders_column=[]
                                     for species in selected_species_values:
-                                        layout_stoichiometry_values.append(
-                                            [sg.Text(f"{species}"), sg.InputText(key=f"stoichiometry_value_{species}", size=(5, 1))])
+                                        species_column.append([sg.Text(f"{species}")])
+                                        orders_column.append([sg.InputText(key=f"stoichiometry_value_{species}", size=(5, 1))])
+                                    # Add the columns to the layout. 
+                                    layout_stoichiometry_values.append([sg.Column(species_column,element_justification='left'),sg.Column(orders_column,element_justification='left')])
                                     layout_stoichiometry_values.append([sg.Button("OK"), sg.Button("Cancel")])
                                     # Create the popup window for inputing stochiometry values. 
                                     window_stoichiometry_values = sg.Window("Enter Stoichiometry Values", layout_stoichiometry_values)
                                     # Maintain an infinite loop to process events until the window is shut down.
                                     while True:
                                         event_stoichiometry_values, values_stoichiometry_values = window_stoichiometry_values.read()
                                         if event_stoichiometry_values == sg.WIN_CLOSED or event_stoichiometry_values == "Cancel":
                                             break
                                         elif event_stoichiometry_values == "OK":
-                                            # Save the stochiometry values inputted by the user as a dictionary. 
-                                            stoichiometry_values = {}
-                                            for species in selected_species_values:
-                                                stoichiometry_value = values_stoichiometry_values.get(f"stoichiometry_value_{species}", "")
-                                                stoichiometry_values[species] = stoichiometry_value
-                                            # Call the plot kinetic data functio using the stochiometry values dictionary. 
-                                            plot_kinetic_data(data, stoichiometry_values,data_plotting_settings)
-                                            break
+                                            try:
+                                                # Save the stochiometry values inputted by the user as a dictionary. 
+                                                stoichiometry_values = {}
+                                                for species in selected_species_values:
+                                                    stoichiometry_value = values_stoichiometry_values.get(f"stoichiometry_value_{species}", "")
+                                                    stoichiometry_values[species] = float(stoichiometry_value)
+                                                # Call the plot kinetic data functio using the stochiometry values dictionary. 
+                                                plot_kinetic_data(data, stoichiometry_values,data_plotting_settings)
+                                                break
+                                            except ValueError as e:
+                                                sg.popup_error(f"Invalid input: {e}")
                                     window_stoichiometry_values.close()
                                 break
                         window_select_species.close()
                     else:
                         # If the user chooses not to visualise mass balance, call the plot_kinetic_data function without 
                         plot_kinetic_data(data,None,data_plotting_settings)
-                elif event_inspect_kinetic_data == "Plot Kinetic Data for Selected Experiments and Species":  
+                elif event_inspect_kinetic_data == "Plot data for selected experiments & species":  
                     # Selected the experiments and reaction species selected by the user. 
                     selected_experiments = values["experiments"]
                     selected_species = values["columns"]
                     # Create an error message is no selected experiments or species have been selected. 
                     if not selected_experiments and not selected_species:
                         sg.popup_error("No experiments nor reaction species have been selected.")
                     elif not selected_experiments:
@@ -1849,15 +2714,15 @@
                             [sg.Text("Do you want to visualise mass balance for the kinetic data?")],
                             [sg.Button("Yes"), sg.Button("No")]]
                         # Create the visualise mass balance window. 
                         window_visualise_mass_balance = sg.Window("Visualise Mass Balance", layout_visualise_mass_balance)
                         event_visualise_mass_balance, values_visualise_mass_balance = window_visualise_mass_balance.read()
                         window_visualise_mass_balance.close()
                         if event_visualise_mass_balance == sg.WIN_CLOSED:
-                            break
+                            continue
                         if event_visualise_mass_balance == "Yes":
                             # Use Listbox to create a multi-selection list
                             selected_species_list = sg.Listbox(
                                 values=columns,
                                 select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE,
                                 size=(20, min(12, len(selected_species))),
                                 key="selected_species_listbox"
@@ -1868,27 +2733,31 @@
                                 [sg.Button("OK"), sg.Button("Cancel")]
                             ]
                             window_select_species = sg.Window("Select Reaction Species", layout_select_species)
                             # Maintain an infinite loop to process events until the window is shut down.
                             while True:
                                 event_select_species, values_select_species = window_select_species.read()
                                 if event_select_species == sg.WIN_CLOSED or event_select_species == "Cancel":
+                                    window_select_species.close()
                                     break
                                 elif event_select_species == "OK":
                                     selected_species_values = values_select_species["selected_species_listbox"]
                                     if not selected_species_values:
                                         sg.popup_error("Please select one or more reaction species.")
                                     else:
-                                        # Query for stoichiometry numbers
-                                        layout_stoichiometry_values = [
-                                            [sg.Text(f"Enter stoichiometry values for selected reaction species:")],
-                                        ]
+                                        # Query user for stoichiometry numbers.
+                                        layout_stoichiometry_values = [[sg.Text(f"Enter stoichiometry values for selected reaction species:")]]
+                                       # Define columns with reaction species and with input boxes for order values:
+                                        species_column=[]
+                                        orders_column=[]
                                         for species in selected_species_values:
-                                            layout_stoichiometry_values.append(
-                                                [sg.Text(f"{species}"), sg.InputText(key=f"stoichiometry_value_{species}", size=(5, 1))])
+                                            species_column.append([sg.Text(f"{species}")])
+                                            orders_column.append([sg.InputText(key=f"stoichiometry_value_{species}", size=(5, 1))])
+                                        # Add the columns to the layout. 
+                                        layout_stoichiometry_values.append([sg.Column(species_column,element_justification='left'),sg.Column(orders_column,element_justification='left')])
                                         layout_stoichiometry_values.append([sg.Button("OK"), sg.Button("Cancel")])
                                         # Create the window for the user to input stochiometry values for mass balance.
                                         window_stoichiometry_values = sg.Window("Enter Stoichiometry Values", layout_stoichiometry_values)
                                         # Maintain an infinite loop to process events until the window is shut down.
                                         while True:
                                             event_stoichiometry_values, values_stoichiometry_values = window_stoichiometry_values.read()
                                             if event_stoichiometry_values == sg.WIN_CLOSED or event_stoichiometry_values == "Cancel":
@@ -1898,59 +2767,82 @@
                                                 # Save the selected stochiometry values. 
                                                 for species in selected_species_values:
                                                     stoichiometry_value = values_stoichiometry_values.get(f"stoichiometry_value_{species}", "")
                                                     stoichiometry_values[species] = stoichiometry_value
                                                 # Plot the modified kinetic data with the inputted stochiometry values and the data plotting settings. 
                                                 plot_kinetic_data(data_modified, stoichiometry_values,data_plotting_settings)
                                                 break
-                                        window_stoichiometry_values.close()
-                                    break                
+                                        window_stoichiometry_values.close()             
                             window_select_species.close()
                         else:
                             # If the user chooses not to visualise mass balance, return None for mass balance and stoichiometry list
                             plot_kinetic_data(data_modified,None,data_plotting_settings)
 
-                elif event_inspect_kinetic_data == "Plot Concentration Profiles":
+                elif event_inspect_kinetic_data == "Plot concentration profiles":
                     # Create a list of reaction species 
                     reaction_species_list = fixed_order_species
+                    # Create a list of selected experiments:
+                    selected_experiments = values["experiments"]
                     # Use Combo to create a dropdown menu for the user to select reaction species. 
                     selected_species = sg.Combo(
                         values=reaction_species_list,
                         default_value=reaction_species_list[0] if reaction_species_list else "",
                         size=(20, 1),
                         key="selected_species_dropdown",)
                     # Create the select species layout. 
                     layout_select_species = [
-                        [sg.Text("Select one reaction species for concentration profiles:")],
+                        [sg.Text("Select one reaction species to plot concentration profiles:")],
                         [selected_species],
-                        [sg.Checkbox("Only include selected experiments",key='experiments',default=Plot_concentration_profiles_selected_experiments,enable_events=True)],
                         [sg.Button("OK"), sg.Button("Cancel")]]
+                    if len(selected_experiments)>0:
+                        layout_select_species.insert(2,[sg.Checkbox("Only include selected experiments",key='experiments',default=Plot_concentration_profiles_selected_experiments,enable_events=True)])
+                    else:
+                        layout_select_species.insert(2,[sg.Text('NB: Select experiments in main window for subset of experiments.', font=('Arial', 9))])
                     # Create a window for selecting reaction species. 
                     window_select_species = sg.Window("Select Reaction Species", layout_select_species)
                     # Maintain an infinite loop to process events until the window is shut down.
                     while True:
                         event_select_species, values_select_species = window_select_species.read()
                         if event_select_species == sg.WIN_CLOSED or event_select_species == "Cancel":
                             break
                         elif event_select_species == "OK":
-                            # Define the experiments selected by the user. 
-                            Plot_concentration_profiles_selected_experiments=values_select_species['experiments']
-                            selected_experiments = values["experiments"]
-                            # Modify the dataset to only include the concentration profiles of the selected species. 
-                            if Plot_concentration_profiles_selected_experiments and len(selected_experiments)>0:
-                                data_2=copy.deepcopy(data)
-                                data_modified={}
-                                for exp in selected_experiments:
-                                    data_modified[exp]=data_2[exp]
                             selected_species_value = values_select_species["selected_species_dropdown"]
-                            # Plot the modified kinetic data. 
-                            if selected_species_value:
-                                if Plot_concentration_profiles_selected_experiments and len(selected_experiments)>0:
+                            if len(selected_experiments)==0:
+                                plot_concentration_profiles(data, selected_species_value,data_plotting_settings)
+                            else:
+                                if values_select_species['experiments']:
+                                    # Make a copy of the data and make a modified version of it with only the selected experiments. 
+                                    data_2=copy.deepcopy(data)
+                                    data_modified={}
+                                    for exp in selected_experiments:
+                                        data_modified[exp]=data_2[exp]
+                                    selected_species_value = values_select_species["selected_species_dropdown"]
+                                    # Plot the modified kinetic data. 
                                     plot_concentration_profiles(data_modified, selected_species_value,data_plotting_settings)
                                 else:
                                     plot_concentration_profiles(data, selected_species_value,data_plotting_settings)
-                            break
+                                break
                     window_select_species.close()
+                elif event_inspect_kinetic_data=='Export the kinetic dataset to .xlsx or .csv':
+                        # Open a browse window where the user can save the active kinetic data ("data").
+                        file_path_save_data = sg.popup_get_file('Save As', save_as=True, no_window=True,file_types=(("Excel File", "*.xlsx"), ("CSV File", "*.csv")))
+                        # Identify the selected extension (xlsx or csv)
+                        file_extension = os.path.splitext(file_path_save_data)[1]
+                        if file_extension=='.xlsx':
+                            # Save an .xlsx file with one experiment per sheet. 
+                            with pd.ExcelWriter(file_path_save_data) as writer:
+                                for name, df in data.items():
+                                    df.to_excel(writer, sheet_name=name,index=False)
+                        elif file_extension=='.csv':
+                            # Add a confirmation box to inform the user that saving as csv will generate one file per experiment. 
+                            proceed = sg.popup_ok_cancel('NB: Saving as CSV will generate one file per experiment in the selected folder.\nDo you want to proceed?', title='Confirmation')
+                            # Save each of the experiments as CSVs if the user has clicked OK. 
+                            if proceed == 'OK':
+                                for name, df in data.items():
+                                    df.to_csv(os.path.join(os.path.dirname(file_path_save_data), f"{name}.csv"), index=False)
+                            else:
+                                continue
             window_inspect_kinetic_data.close()
     window.close()
 if __name__ == "__main__":
-    main()
+    main()
+
```

### Comparing `auto_vtna-1.0.2/auto_vtna/Automatic_VTNA.py` & `auto_vtna-1.0.3/auto_vtna/Automatic_VTNA.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,7 +343,8 @@
             plt.grid()
         image_stream = BytesIO()
         plt.savefig(image_stream, format='png', bbox_inches='tight', pad_inches=0)
         image_stream.seek(0)
         img = Image(image_stream)
         plt.show()
         return img
+
```

### Comparing `auto_vtna-1.0.2/auto_vtna/Normal_VTNA.py` & `auto_vtna-1.0.3/auto_vtna/Normal_VTNA.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.2/auto_vtna/VTNA_functions.py` & `auto_vtna-1.0.3/auto_vtna/VTNA_functions.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.2/auto_vtna/__init__.py` & `auto_vtna-1.0.3/auto_vtna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,27 +319,33 @@
         graphs will pop-up one after the other. 
         legend_outside (bol): Set to False by default to show legend inside the axis of the plot. \
         Can be set to True to show the legend outside the axis (top right). 
         DP_scaler (float, int): Factor by which the datapoints of the plots is scaled from a standard \
         value of 6. 
         linewidth (float, int): The linewidth parameter used to generate plots. Is by default set to 1. 
     """
+    # Make the plot mode 'separate' if there is only one experiment in the dataset. 
+    if len(list(data.keys()))==1:
+        plot_mode='separate'
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     if plot_mode=='together':
         addition=0
         if legend_outside:
             addition=1
         # Check how many rows and columns there should be based on the number of dataframes in data.
         n,m = len(list(data.keys()))+addition,3
         if n>6:
             m=4
         num_cols = min(m, n)
         num_rows = (n + num_cols - 1) // num_cols
+        # Add an exception if there are 9 plot objects:
+        if len(list(data.keys()))+addition==9:
+            num_cols,num_rows=3,3
         # Create a single figure and subplots with specified number of rows and columns.
         fig, axs = plt.subplots(nrows=num_rows, ncols=num_cols, figsize=(7 * 0.45*fig_size_scaler * num_cols, 5 * 0.6*num_rows * fig_size_scaler),constrained_layout=True)
         for i, (rm_name, rm_data) in enumerate(data.items()):
             # Check if there's only one row
             if num_rows == 1:  
                 ax = axs[i % num_cols]  # Use modulo to handle indexing in a 1D array
             else:
@@ -377,15 +383,15 @@
             ax.spines['bottom'].set_visible(False)
             ax.set_xticklabels([])
             ax.set_yticklabels([])
             ax.set_xticks([])
             ax.set_yticks([])
             ax.legend(handles, labels, loc='center')
         # Remove empty subplots if there are any
-        for i in range(len(data)+1, num_cols * num_rows):
+        for i in range(len(data)+addition, num_cols * num_rows):
             fig.delaxes(axs.flatten()[i])
         plt.show()
     elif plot_mode=='scrollable':
         # Define a class for creating scrollable plots
         class ScrollablePlot:
             def __init__(self, data_dict, ylim=None, y_unit='M', t_unit=None, 
                          fig_size_scaler=1,legend_outside=legend_outside,DP_scaler=1,linewidth=1):
@@ -480,15 +486,16 @@
                 # Move to the next plot and update the display
                 self.current_plot_index = (self.current_plot_index + 1) % len(self.data)
                 self.plot_current_data()
             def previous_plot(self):
                 # Move to the previous plot and update the display
                 self.current_plot_index = (self.current_plot_index - 1) % len(self.data)
                 self.plot_current_data()
-        scrollable_plot = ScrollablePlot(data, ylim=ylim, y_unit=y_unit, t_unit=t_unit, fig_size_scaler=fig_size_scaler,legend_outside=legend_outside)
+        scrollable_plot = ScrollablePlot(data, ylim=ylim, y_unit=y_unit, t_unit=t_unit, 
+        fig_size_scaler=fig_size_scaler,legend_outside=legend_outside,DP_scaler=DP_scaler,linewidth=linewidth)
         plt.show()
     else:
             # Identify the first key in the data dictionary
         RM1=list(data.keys())[0]
         # Identify the time column unit for the first reaction mixture data set
         t=data[RM1].columns[0]
         for i in data.keys():
@@ -525,14 +532,15 @@
                 fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                 plt.gcf().set_size_inches(fig_size)
             else:
                 plt.legend()
             if ylim!=None:
                 plt.ylim(0,ylim)
             #Use plt.show to complete plot and move to the next reaction mixture data set
+            plt.tight_layout()
             plt.show()
 
 def plot_data_together(data,species,ylim=None,y_unit='mM',fig_size_scaler=1,t_unit=None,
     legend_outside=False,DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using Pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
@@ -567,15 +575,15 @@
     fig, ax = plt.subplots(figsize=(7*0.9*fig_size_scaler, 5*0.9*fig_size_scaler))
     for i in data.keys():
         time=data[i][t]
         # plot kinetic profiles for the chosen species for each reaction mixture data set
         for j in data[i].keys():
             if j==t or j not in species:
                 continue
-            ax.plot(time,data[i][j],label=f'{i},{species}',linestyle='-',marker='o',
+            ax.plot(time,data[i][j],label=f'{i}, {species}',linestyle='-',marker='o',
                     markersize=6*DP_scaler,linewidth=linewidth)
             ax.set_title(f'concentration profiles for {species}')
             ax.set_xlabel(t_label)
             ax.set_ylabel(f'concentration / {y_unit}')
         # Define y-axis range up to ylim if defined.
         if ylim!=None:
             ax.set_ylim(0,ylim)
@@ -628,94 +636,109 @@
         graphs will pop-up one after the other. 
         legend_outside (bol): Set to False by default to show legend inside the axis of the plot. \
         Can be set to True to show the legend outside the axis (top right). 
         DP_scaler (float, int): Factor by which the datapoints of the plots is scaled from a standard \
         value of 6. 
         linewidth (float, int): The linewidth parameter used to generate plots. Is by default set to 1. 
     """
+    # Make the plot mode 'separate' if there is only one experiment in the dataset. 
+    if len(list(data.keys()))==1:
+        plot_mode='separate'
     # Find the title of the time column of the experiment datasets
     RM1 = list(data.keys())[0]
     t = data[RM1].columns[0]
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     MB_title_string = ''
     # Define the title of the mass balance axis
     for mol in range(len(species)):
         if mol != 0 and species[mol] == species[-1]:
             MB_title_string = MB_title_string + 'and '
         MB_title_string = MB_title_string + f'{species[mol]}, '
     if len(species) == 1:
         MB_title_string = f'{species[0]}. '
-    if plot_mode == 'together':
-        # define the number of columns and rows for the subplot. 
-        n,m = len(list(data.keys()))+1,3
+    if plot_mode=='together':
+        addition=0
+        if legend_outside:
+            addition=1
+        # Check how many rows and columns there should be based on the number of dataframes in data.
+        n,m = len(list(data.keys()))+addition,3
         if n>6:
             m=4
         num_cols = min(m, n)
-        num_rows = (n + num_cols - 1) // num_cols  # Equivalent to ceil(n / num_cols)
-        # Create subplots
-        fig, axes = plt.subplots(num_rows, num_cols, figsize=(7 * 0.8*fig_size_scaler * num_cols, 5 *0.8* num_rows * fig_size_scaler))
+        num_rows = (n + num_cols - 1) // num_cols
+        # Add an exception if there are 9 plot objects:
+        if len(list(data.keys()))+addition==9:
+            num_cols,num_rows=3,3
+        # Create a single figure and subplots with specified number of rows and columns.
+        fig, axes = plt.subplots(nrows=num_rows, ncols=num_cols, figsize=(7.5 * 0.45*fig_size_scaler * num_cols, 4.5 * 0.6*num_rows * fig_size_scaler),constrained_layout=True)
         axes = axes.flatten() 
         for idx, (i, ax) in enumerate(zip(data.keys(), axes)):
             Concs = []
             largest_conc = []
             time = data[i][t]
             # Create a curve for each reaction species
             for j in data[i].keys():
                 if j == t:
                     continue
                 ax.plot(time, data[i][j], label=j, linestyle='-', marker='o', markersize=6*DP_scaler,linewidth=linewidth)
                 ax.set_title(i)
                 ax.set_xlabel(t)
                 ax.set_ylabel(f'concentration / {y_unit}')
-                if ylim is not None:
-                    ax.set_ylim(0, ylim)
                 largest_conc.append(max(data[i][j].to_numpy()))
                 if t_unit is not None:
                     ax.set_xlabel(f'{t} / {t_unit}')
                 if j == t or j not in species:
                     continue
                 # Add concentration*stochiometry array for calculation of mass balance over time
                 Concs.append(data[i][j].to_numpy() * stochiometry[species.index(j)])
             # Use Concs to create mass balance sum for each time point
             sums = np.zeros(len(Concs[0]))
             for i in Concs:
                 sums = sums + i
             # Use sums to find the % mass balance at each time relative to the initial value.
-            MB = sums / sums[0] * 100 * scaler
+            # If the first sum is 0, use the final sum instead. (could occur if only product(s) are chosen)
+            if sums[0]>0:
+                MB = sums / sums[0] * 100 * scaler
+            else:
+                MB = sums / sums[-1] * 100 * scaler
             ax2 = ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}', color="purple")
-            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",
-                     markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",markersize=6*DP_scaler)
             ax2.plot([0, max(time)], [100, 100], linestyle='--', marker='', color='purple')
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends.
             ax2.set_ylim(0, max(MB) + 28)
-            ax.set_ylim(0, max(largest_conc) + max(largest_conc) * 0.15)
+            if ylim is not None and type(ylim) in [float,int]:
+                ax.set_ylim(0, ylim)
+            else:
+                ax.set_ylim(0, max(largest_conc) + max(largest_conc) * 0.15)
+            if not legend_outside:
+                ax.legend()
         ax = axes[idx+1]
         handles, labels = axes[0].get_legend_handles_labels()
         ax.spines['top'].set_visible(False)
         ax.spines['right'].set_visible(False)
         ax.spines['left'].set_visible(False)
         ax.spines['bottom'].set_visible(False)
         ax.set_xticklabels([])
         ax.set_yticklabels([])
         ax.set_xticks([])
         ax.set_yticks([])
         ax.legend(handles, labels, loc='center left')
-        for i in range(len(data)+1, num_cols * num_rows):
+        for i in range(len(data)+addition, num_cols * num_rows):
           fig.delaxes(axes.flatten()[i])
         # Adjust layout to prevent overlap
-        plt.subplots_adjust(wspace=1.45, hspace=1.45)
         plt.tight_layout()
         plt.show()
     elif plot_mode=='scrollable':
         class ScrollablePlot:
-            def __init__(self, data_dict,species, stochiometry,y_unit='M',t_unit=None,fig_size_scaler=1,ylim=None,scaler=1,legend_outside=False):
+            def __init__(self, data_dict,species, stochiometry,y_unit='M',t_unit=None,fig_size_scaler=1,
+                         ylim=None,scaler=1,legend_outside=False,DP_scaler=1,linewidth=1):
                 data_1=[]
                 for i,j in data_dict.items():
                     data_1.append(data_dict[i])
                 data_labels=list(data_dict.keys())
                 self.data = data_1
                 self.labels = data_labels
                 self.current_plot_index = 0
@@ -752,16 +775,14 @@
                         continue
                     self.ax.plot(time_column,current_data[j],label=j,linestyle='-',marker='o',
                                  markersize=6*self.DP_scaler,linewidth=linewidth)
                     self.ax.set_title(f'Concentration profiles in {current_label}')
                     self.fig.set_size_inches(7*0.8*self.fig_size_scaler, 5*0.8*self.fig_size_scaler)
                     self.ax.set_xlabel(t)
                     self.ax.set_ylabel(f'concentration / {self.y_unit}')
-                    if self.ylim!=None:
-                        self.ax.set_ylim(0,self.ylim)
                     largest_conc.append(max(current_data[j].to_numpy()))
                     if self.t_unit!=None:
                         self.ax.set_xlabel(f'Time / {self.t_unit}')
                     if j==t or j not in self.species:
                         continue
                     # Add concentration*stochiometry array for calculation of mass balance over time
                     Concs.append(current_data[j].to_numpy()*self.stochiometry[self.species.index(j)])
@@ -769,36 +790,39 @@
                 sums=np.zeros(len(Concs[0]))
                 for i in Concs:
                     sums=sums+i
                 # Use sums to find the % mass balance at each time relative to the intial value.
                 MB=sums/sums[0]*100* scaler
                 self.ax2.set_ylabel(f'Mass balance for:\n {self.MB_title_string[:-2]}',color="purple")
                 self.ax2.yaxis.set_label_position('right')
-                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",
-                              markersize=6*self.DP_scaler,linewidth=linewidth)
+                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*self.DP_scaler)
                 self.ax2.plot([0,max(time_column)],[100,100],linestyle='--',marker='',color='purple')
                 self.ax2.legend(loc='upper center')
                 # Ensure appropriate y limits with space for legends. 
                 self.ax2.set_ylim(0,max(MB)+28)
-                self.ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
+                if self.ylim!=None and type(self.ylim) in [float,int]:
+                    self.ax.set_ylim(0,self.ylim)
+                else:
+                    self.ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
                 if self.legend_outside:
                     # Calculate the width of the legend dynamically based on the longest text element
                     legend = self.ax.legend()
                     # Obtain the legend width in display units. 
                     legend_bbox = legend.get_window_extent()
                     legend_width = legend_bbox.width
                     # Obtain the figure width in display units.
                     fig_box = plt.gcf().get_window_extent()
                     fig_width_display = fig_box.width
                     # See by what fraction the figure width needs to be extended for outside legend.
                     legend_width_scaled=legend_width/fig_width_display
                     # Scale the right argument according to the legend width
-                    self.fig.subplots_adjust(right=1 - legend_width_scaled-0.06)
+                    self.fig.subplots_adjust(right=1 - legend_width_scaled-0.07)
                     # Place the legend outside the axis
-                    self.ax.legend(loc='center left',bbox_to_anchor=(1.16, 0.8))
+                    legend_position_scaler=fig_size_scaler**0.3 if fig_size_scaler<1 else 1
+                    self.ax.legend(loc='center left',bbox_to_anchor=(1.14/legend_position_scaler, 0.8))
                     # Adjust figure size to increase width according to the outside legend width
                     fig_size = plt.gcf().get_size_inches()
                     fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                     plt.gcf().set_size_inches(fig_size)
                 else:
                     self.ax.legend()
                 plt.tight_layout()
@@ -813,15 +837,16 @@
             def next_plot(self):
                 self.current_plot_index = (self.current_plot_index + 1) % len(self.data)
                 self.plot_current_data()
 
             def previous_plot(self):
                 self.current_plot_index = (self.current_plot_index - 1) % len(self.data)
                 self.plot_current_data()
-        scrollable_plot = ScrollablePlot(data,species,stochiometry,fig_size_scaler=fig_size_scaler,t_unit=t_unit,y_unit=y_unit,scaler=scaler,ylim=ylim,legend_outside=legend_outside)
+        scrollable_plot = ScrollablePlot(data,species,stochiometry,fig_size_scaler=fig_size_scaler,
+        t_unit=t_unit,y_unit=y_unit,scaler=scaler,ylim=ylim,legend_outside=legend_outside,linewidth=linewidth, DP_scaler=DP_scaler)
         plt.show()
     else: 
         # Create a twin plot for each experiment dataset
         for i in data.keys():
             Concs=[]
             largest_conc=[]
             fig,ax = plt.subplots(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
@@ -839,48 +864,49 @@
                 largest_conc.append(max(data[i][j].to_numpy()))
                 if t_unit!=None:
                     plt.xlabel(f'{t} / {t_unit}')
                 if j==t or j not in species:
                     continue
                 # Add concentration*stochiometry array for calculation of mass balance over time
                 Concs.append(data[i][j].to_numpy()*stochiometry[species.index(j)])
-            if ylim!=None:
-                ax.set_ylim(0,ylim)
             if legend_outside:
                 # Calculate the width of the legend dynamically based on the longest text element
                 legend = ax.legend()
                 # Obtain the legend width in display units. 
                 legend_bbox = legend.get_window_extent()
                 legend_width = legend_bbox.width
                 # Obtain the figure width in display units.
                 fig_box = plt.gcf().get_window_extent()
                 fig_width_display = fig_box.width
                 # See by what fraction the figure width needs to be extended for outside legend.
                 legend_width_scaled=legend_width/fig_width_display
                 # Scale the right argument according to the legend width
-                fig.subplots_adjust(right=1 - legend_width_scaled-0.06)
+                fig.subplots_adjust(right=1 - legend_width_scaled-0.07)
                 # Place the legend outside the axis
-                ax.legend(loc='center left', bbox_to_anchor=(1.16, 0.8))
+                legend_position_scaler=fig_size_scaler**0.3 if fig_size_scaler<1 else 1
+                ax.legend(loc='center left',bbox_to_anchor=(1.14/legend_position_scaler, 0.8))
                 # Adjust figure size to increase width according to the outside legend width
                 fig_size = plt.gcf().get_size_inches()
                 fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                 plt.gcf().set_size_inches(fig_size)
             else:
                 ax.legend()
             # Use Concs to create mass balance sum for each time point
             sums=np.zeros(len(Concs[0]))
             for i in Concs:
                 sums=sums+i
             # Use sums to find the % mass balance at each time relative to the intial value.
             MB=sums/sums[0]*100*scaler
             ax2=ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}',color="purple")
-            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",
-                     markersize=6*DP_scaler,linewidth=linewidth)
-            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple',
-                     markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*DP_scaler)
+            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple')
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends. 
             ax2.set_ylim(0,max(MB)+28)
-            ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
+            if ylim!=None and type(ylim) in [float,int]:
+                ax.set_ylim(0,ylim)
+            else:
+                ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
+            fig.subplots_adjust(right=0.85)
             plt.show()
```

### Comparing `auto_vtna-1.0.2/auto_vtna.egg-info/PKG-INFO` & `auto_vtna-1.0.3/auto_vtna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-vtna
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.2/setup.py` & `auto_vtna-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 
 # Meta-data of the package.
 NAME = 'auto_vtna'
 DESCRIPTION = 'A Python package for efficient and automatic VTNA analysis'
 EMAIL = 'dd4518@ic.ac.uk'
 AUTHOR = 'Daniel Dalland'
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 REQUIRED=[
     'pandas',
     'numpy',
     'matplotlib',
     'num2words',
     'mplcursors',
     'scipy',
```

