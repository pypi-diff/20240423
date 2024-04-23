# Comparing `tmp/python_optimization-0.0.6.tar.gz` & `tmp/python_optimization-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_optimization-0.0.6.tar", last modified: Sun Apr 21 16:10:37 2024, max compression
+gzip compressed data, was "python_optimization-0.0.7.tar", last modified: Mon Apr 22 11:59:19 2024, max compression
```

## Comparing `python_optimization-0.0.6.tar` & `python_optimization-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 16:10:37.000694 python_optimization-0.0.6/
--rw-rw-rw-   0        0        0      557 2024-04-21 16:10:37.000694 python_optimization-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 16:10:36.972682 python_optimization-0.0.6/python_optimization/
--rw-rw-rw-   0        0        0       33 2024-04-21 16:09:47.000000 python_optimization-0.0.6/python_optimization/__init__.py
--rw-rw-rw-   0        0        0    21539 2024-04-21 15:09:08.000000 python_optimization-0.0.6/python_optimization/python_optimization.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:10:36.996692 python_optimization-0.0.6/python_optimization.egg-info/
--rw-rw-rw-   0        0        0      557 2024-04-21 16:10:36.000000 python_optimization-0.0.6/python_optimization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-21 16:10:36.000000 python_optimization-0.0.6/python_optimization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:10:36.000000 python_optimization-0.0.6/python_optimization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-21 16:10:36.000000 python_optimization-0.0.6/python_optimization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 16:10:37.000694 python_optimization-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-21 16:10:21.000000 python_optimization-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.987967 python_optimization-0.0.7/
+-rw-rw-rw-   0        0        0      551 2024-04-22 11:59:19.986967 python_optimization-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.965961 python_optimization-0.0.7/python_optimization/
+-rw-rw-rw-   0        0        0       53 2024-04-22 11:28:07.000000 python_optimization-0.0.7/python_optimization/__init__.py
+-rw-rw-rw-   0        0        0    23973 2024-04-22 11:59:01.000000 python_optimization-0.0.7/python_optimization/python_optimization.py
+drwxrwxrwx   0        0        0        0 2024-04-22 11:59:19.984964 python_optimization-0.0.7/python_optimization.egg-info/
+-rw-rw-rw-   0        0        0      551 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 11:59:19.000000 python_optimization-0.0.7/python_optimization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 11:59:19.987967 python_optimization-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-04-22 11:47:43.000000 python_optimization-0.0.7/setup.py
```

### Comparing `python_optimization-0.0.6/PKG-INFO` & `python_optimization-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python_optimization
-Version: 0.0.6
+Version: 0.0.7
 Summary: python optimization
-Author: NeuralNine (Florian Dedov)
-Author-email: <mail@neuralnine.com>
+Author: founder synergy
+Author-email: founders.synergy@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `python_optimization-0.0.6/python_optimization/python_optimization.py` & `python_optimization-0.0.7/python_optimization/python_optimization.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     complement(A, B)
     difference(A, B)
     cartprod(A, B)
 
     result = maxmin()
     print("Max-Min Composition is", result)
     '''
-    return 0
+    return "Package not Installed properly"
 
 def milk():
     '''
     import random
     from deap import base, creator, tools, algorithms
     from sklearn.model_selection import train_test_split
     from sklearn.neural_network import MLPClassifier
@@ -149,15 +149,15 @@
         population = toolbox.select(offspring, k=len(population))
 
     best_individual = tools.selBest(population, k=1)[0]
     best_params = best_individual
 
     print("Best Parameters:", best_params)
     '''
-    return 0
+    return "Package not Installed properly"
 
 
 def art():
     '''
     import tensorflow_hub as hub
     import tensorflow as tf
     from matplotlib import pyplot as plt
@@ -179,15 +179,15 @@
 
     stylized_image = model(tf.constant(load_image('car1.jpeg')), tf.constant(load_image('tree.jpg')))[0]
 
     plt.imshow(np.squeeze(stylized_image))
     plt.show()
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def deap():
     '''
     import random
     import numpy as np
     from deap import base, creator, tools, algorithms
     
@@ -219,106 +219,124 @@
         stats.register("max", np.max)
 
         pop, log = algorithms.eaSimple(pop, toolbox, cxpb=0.5, mutpb=0.2, ngen=40,
                                     stats=stats, halloffame=hof, verbose=True)
 
     main()
     '''
-    return 0
+    return "Package not Installed properly"
 
 def ant():
     '''
-    import numpy as np
-    from numpy import inf
+import numpy as np
+from numpy import inf
+
+#given values for the problems
+
+d = np.array([[0,10,12,11,14],[10,0,13,15,8],[12,13,0,9,14],[11,15,9,0,16],[14,8,14,16,0]])
+
+iteration = 100
+n_ants = 5
+n_citys = 5
+
+# intialization part
+m = n_ants
+n = n_citys
+e = .5         #evaporation rate
+alpha = 1     #pheromone factor
+beta = 2       #visibility factor
 
-    d = np.array([[0,10,12,11,14],[10,0,13,15,8],[12,13,0,9,14],[11,15,9,0,16],[14,8,14,16,0]])
+#calculating the visibility of the next city visibility(i,j)=1/d(i,j)
+visibility = 1/d
+visibility[visibility == inf ] = 0
 
-    iteration = 100
-    n_ants = 5
-    n_citys = 5
-    m = n_ants
-    n = n_citys
-    e = .5        
-    alpha = 1    
-    beta = 2      
-    visibility = 1/d
-    visibility[visibility == inf ] = 0
+#intializing pheromne present at the paths to the cities
+pheromne = .1*np.ones((m,n))
 
-    pheromne = .1*np.ones((m,n))
+#intializing the rute of the ants with size rute(n_ants,n_citys+1)
+#note adding 1 because we want to come back to the source city
 
+rute = np.ones((m,n+1))
 
-    rute = np.ones((m,n+1))
+for ite in range(iteration):
 
-    for ite in range(iteration):
+    rute[:,0] = 1          #initial starting and ending positon of every ants '1' i.e city '1'
 
-        rute[:,0] = 1          
+    for i in range(m):
 
-        for i in range(m):
+        temp_visibility = np.array(visibility)         #creating a copy of visibility
 
-            temp_visibility = np.array(visibility)        
-            for j in range(n-1):
-                #print(rute)
+        for j in range(n-1):
+            #print(rute)
 
-                combine_feature = np.zeros(5)     
-                cum_prob = np.zeros(5)            
+            combine_feature = np.zeros(5)     #intializing combine_feature array to zero
+            cum_prob = np.zeros(5)            #intializing cummulative probability array to zeros
 
-                cur_loc = int(rute[i,j]-1)       
+            cur_loc = int(rute[i,j]-1)        #current city of the ant
 
-                temp_visibility[:,cur_loc] = 0     
+            temp_visibility[:,cur_loc] = 0     #making visibility of the current city as zero
 
-                p_feature = np.power(pheromne[cur_loc,:],beta)        
-                v_feature = np.power(temp_visibility[cur_loc,:],alpha)  
+            p_feature = np.power(pheromne[cur_loc,:],beta)         #calculating pheromne feature
+            v_feature = np.power(temp_visibility[cur_loc,:],alpha)  #calculating visibility feature
 
-                p_feature = p_feature[:,np.newaxis]                    
-                v_feature = v_feature[:,np.newaxis]                     
+            p_feature = p_feature[:,np.newaxis]                     #adding axis to make a size[5,1]
+            v_feature = v_feature[:,np.newaxis]                     #adding axis to make a size[5,1]
 
-                combine_feature = np.multiply(p_feature,v_feature)     
+            combine_feature = np.multiply(p_feature,v_feature)     #calculating the combine feature
 
-                total = np.sum(combine_feature)                       
+            total = np.sum(combine_feature)                        #sum of all the feature
 
-                probs = combine_feature/total   
-                cum_prob = np.cumsum(probs)     
-                r = np.random.random_sample()  
-                city = np.nonzero(cum_prob>r)[0][0]+1       
+            probs = combine_feature/total   #finding probability of element probs(i) = comine_feature(i)/total
 
-                rute[i,j+1] = city              
+            cum_prob = np.cumsum(probs)     #calculating cummulative sum
+            #print(cum_prob)
+            r = np.random.random_sample()   #randon no in [0,1)
+            #print(r)
+            city = np.nonzero(cum_prob>r)[0][0]+1       #finding the next city having probability higher then random(r)
+            #print(city)
 
-            left = list(set([i for i in range(1,n+1)])-set(rute[i,:-2]))[0]    
+            rute[i,j+1] = city              #adding city to route
 
-            rute[i,-2] = left                   
-        rute_opt = np.array(rute)              
+        left = list(set([i for i in range(1,n+1)])-set(rute[i,:-2]))[0]     #finding the last untraversed city to route
 
-        dist_cost = np.zeros((m,1))             
+        rute[i,-2] = left                   #adding untraversed city to route
 
-        for i in range(m):
+    rute_opt = np.array(rute)               #intializing optimal route
 
-            s = 0
-            for j in range(n-1):
+    dist_cost = np.zeros((m,1))             #intializing total_distance_of_tour with zero
 
-                s = s + d[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1]  
-            dist_cost[i]=s                      
+    for i in range(m):
 
-        dist_min_loc = np.argmin(dist_cost)             
-        dist_min_cost = dist_cost[dist_min_loc]         
+        s = 0
+        for j in range(n-1):
 
-        best_route = rute[dist_min_loc,:]               
-        pheromne = (1-e)*pheromne                       
+            s = s + d[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1]   #calcualting total tour distance
 
-        for i in range(m):
-            for j in range(n-1):
-                dt = 1/dist_cost[i]
-                pheromne[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1] = pheromne[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1] + dt
+        dist_cost[i]=s                      #storing distance of tour for 'i'th ant at location 'i'
 
-    print('route of all the ants at the end :')
-    print(rute_opt)
-    print()
-    print('best path :',best_route)
-    print('cost of the best path',int(dist_min_cost[0]) + d[int(best_route[-2])-1,0])
+    dist_min_loc = np.argmin(dist_cost)             #finding location of minimum of dist_cost
+    dist_min_cost = dist_cost[dist_min_loc]         #finging min of dist_cost
+
+    best_route = rute[dist_min_loc,:]               #intializing current traversed as best route
+    pheromne = (1-e)*pheromne                       #evaporation of pheromne with (1-e)
+
+    for i in range(m):
+        for j in range(n-1):
+            dt = 1/dist_cost[i]
+            pheromne[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1] = pheromne[int(rute_opt[i,j])-1,int(rute_opt[i,j+1])-1] + dt
+            #updating the pheromne with delta_distance
+            #delta_distance will be more with min_dist i.e adding more weight to that route  peromne
+
+print('route of all the ants at the end :')
+print(rute_opt)
+print()
+print('best path :',best_route)
+print('cost of the best path',int(dist_min_cost[0]) + d[int(best_route[-2])-1,0])
     '''
-    return 0
+    return "Package not Installed properly"
 
 
 def rpcc():
     '''
     import xmlrpc.client
 
     with xmlrpc.client.ServerProxy("http://127.0.0.1:8000/") as proxy:
@@ -337,15 +355,15 @@
         except ValueError as ve:
             print(f"Error: {ve}")
 
         except Exception as e:
             print(f"An unexpected error occurred: {e}")
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def rpcs():
     '''
     from xmlrpc.server import SimpleXMLRPCServer
     import math
 
     def factorial(n: int):
@@ -353,15 +371,15 @@
 
     server = SimpleXMLRPCServer(("localhost", 8000))
     print("Listening on port 8000...")
     server.register_function(factorial, "factorial")
     server.serve_forever()
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def rmic():
     '''
     import Pyro5.api
 
     def main():
         uri = "PYRONAME:string_concatenation_server"
@@ -373,15 +391,15 @@
             print(f"Concatenation result: {result}")
 
 
     if __name__ == "__main__":
         main()
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def rmis():
     '''
     import Pyro5.api
     @Pyro5.api.expose
     class StringConcatenationServer:
         def concatenate_strings(self, str1, str2):
@@ -400,15 +418,15 @@
         daemon.requestLoop()
 
 
     if __name__ == "__main__":
         main()
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def dload():
     '''
     import time
     import random
 
 
@@ -438,15 +456,15 @@
     if __name__ == "__main__":
         server_addresses = ['Server B', 'Server A', 'Server C']
         dynamic_load_balancer = DynamicLoadBalancer(server_addresses)
 
         simulate_dynamic_load_balancing(dynamic_load_balancer, 20)
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 
 def rload():
     '''
     import time
 
     class LoadBalancer:
@@ -473,15 +491,15 @@
     if __name__ == "__main__":
         server_addresses = ['Server A', 'Server B', 'Server C']
         load_balancer = LoadBalancer(server_addresses)
 
         simulate_client_requests(load_balancer, 10)
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 def map():
     '''
     from mrjob.job import MRJob
     from mrjob.step import MRStep
     import csv
     from datetime import datetime
@@ -517,15 +535,15 @@
             yield max_pair_key, max_pair_value
 
 
     if __name__ == "__main__":
         CalculateGrades.run()
 
     '''
-    return 0
+    return "Package not Installed properly"
 
 cjava = '''
         import java.rmi.Naming;
         import java.rmi.RemoteException;
         import java.util.InputMismatchException;
         import java.util.Map;
         import java.util.Scanner;
@@ -602,14 +620,26 @@
                     }
                 }
             }
         }
         '''
 
 sjava = '''
+        import java.rmi.Remote;
+        import java.rmi.RemoteException;
+        import java.util.Map;
+
+        public interface HotelInterface extends Remote {
+        boolean bookRoom(String guestName, int roomNumber) throws RemoteException;
+
+        boolean cancelBooking(String guestName) throws RemoteException;
+
+        Map<String, Integer> getBookings() throws RemoteException;
+        }
+
         import java.rmi.RemoteException;
         import java.rmi.server.UnicastRemoteObject;
         import java.util.HashMap;
         import java.util.Map;
         import java.util.concurrent.locks.Lock;
         import java.util.concurrent.locks.ReentrantLock;
 
@@ -669,8 +699,20 @@
             java.rmi.Naming.rebind("HotelService", server);
             System.out.println("HotelServer is ready.");
             } catch (Exception e) {
             e.printStackTrace();
             }
         }
         }
-        '''
+        '''
+
+def install():
+    """
+    deap==1.4.1
+    sklearn==1.3.2
+    tensorflow_hub==0.16.1
+    tensorflow==2.16.1
+    cv2==4.8.0.76
+    matplotlib==3.8.0
+    pyro5==5.15
+    mrjob==0.7.4"""
+    return "Package not Installed properly"
```

### Comparing `python_optimization-0.0.6/python_optimization.egg-info/PKG-INFO` & `python_optimization-0.0.7/python_optimization.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-optimization
-Version: 0.0.6
+Version: 0.0.7
 Summary: python optimization
-Author: NeuralNine (Florian Dedov)
-Author-email: <mail@neuralnine.com>
+Author: founder synergy
+Author-email: founders.synergy@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `python_optimization-0.0.6/setup.py` & `python_optimization-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'python optimization'
 LONG_DESCRIPTION = 'A package that allows python optimization'
 
 # Setting up
 setup(
     name="python_optimization",
     version=VERSION,
-    author="NeuralNine (Florian Dedov)",
-    author_email="<mail@neuralnine.com>",
+    author="founder synergy",
+    author_email="founders.synergy@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
```

