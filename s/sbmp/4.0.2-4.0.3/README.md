# Comparing `tmp/sbmp-4.0.2.tar.gz` & `tmp/sbmp-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmp-4.0.2.tar", last modified: Tue Apr 23 17:25:31 2024, max compression
+gzip compressed data, was "sbmp-4.0.3.tar", last modified: Tue Apr 23 18:35:23 2024, max compression
```

## Comparing `sbmp-4.0.2.tar` & `sbmp-4.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.057424 sbmp-4.0.2/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-4.0.2/LICENSE
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 17:25:31.057021 sbmp-4.0.2/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-4.0.2/README.txt
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.055794 sbmp-4.0.2/sbmp/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       37 2024-04-23 10:25:06.000000 sbmp-4.0.2/sbmp/__init__.py
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)    21244 2024-04-23 17:25:15.000000 sbmp-4.0.2/sbmp/awt.py
--rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-4.0.2/sbmp/iss.py
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.056724 sbmp-4.0.2/sbmp.egg-info/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      180 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/SOURCES.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/dependency_links.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/top_level.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-23 17:25:31.057487 sbmp-4.0.2/setup.cfg
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-23 17:25:23.000000 sbmp-4.0.2/setup.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 18:35:23.451880 sbmp-4.0.3/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-4.0.3/LICENSE
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 18:35:23.451485 sbmp-4.0.3/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-4.0.3/README.txt
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 18:35:23.450440 sbmp-4.0.3/sbmp/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       37 2024-04-23 10:25:06.000000 sbmp-4.0.3/sbmp/__init__.py
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)    25205 2024-04-23 18:34:36.000000 sbmp-4.0.3/sbmp/awt.py
+-rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-4.0.3/sbmp/iss.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 18:35:23.451250 sbmp-4.0.3/sbmp.egg-info/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 18:35:23.000000 sbmp-4.0.3/sbmp.egg-info/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      180 2024-04-23 18:35:23.000000 sbmp-4.0.3/sbmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-23 18:35:23.000000 sbmp-4.0.3/sbmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-23 18:35:23.000000 sbmp-4.0.3/sbmp.egg-info/top_level.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-23 18:35:23.451925 sbmp-4.0.3/setup.cfg
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-23 18:35:16.000000 sbmp-4.0.3/setup.py
```

### Comparing `sbmp-4.0.2/LICENSE` & `sbmp-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmp-4.0.2/PKG-INFO` & `sbmp-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 4.0.2
+Version: 4.0.3
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-4.0.2/sbmp/awt.py` & `sbmp-4.0.3/sbmp/awt.py`

 * *Files 12% similar despite different names*

```diff
@@ -592,26 +592,203 @@
             {
                 return;
             }
             args.IsValid = true;
         } //end of UserCustomValidate method
 '''
 
+access_modifiers_public = '''
+using System;
+using System.Collections.Generic;
+using System.Linq;
+using System.Text;
+using System.Threading.Tasks;
+
+namespace access_modifier
+{
+    internal class Program
+    {
+        class Student
+        {
+            // Declaring members rollNo
+            // and name as public
+            public int rollNo;
+            public string name;
+            // Constructor
+            public Student(int r, string n)
+            {
+                rollNo = r;
+                name = n;
+            }
+            // methods getRollNo and getName
+            // also declared as public
+            public int getRollNo()
+            {
+                return rollNo;
+            }
+            public string getName()
+            {
+                return name;
+            }
+        }
+        static void Main(string[] args)
+        {
+            // Creating object of the class Student
+            Student S = new Student(2, "John");
+            // Displaying details directly
+            // using the class members
+            Console.WriteLine("Roll number: {0}", S.rollNo);
+            Console.WriteLine("Name: {0}", S.name);
+            Console.WriteLine();
+            // Displaying details using member method 
+            Console.WriteLine("Roll number: {0}", S.getRollNo());
+            Console.WriteLine("Name: {0}", S.getName());
+            Console.ReadKey();
+        }
+    }
+}
+
+'''
+
+sessions = '''
+ // Login.aspx
+
+<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="Login.aspx.cs" Inherits="Session1.WebForm2" %>
+
+<!DOCTYPE html>
+
+<html xmlns="http://www.w3.org/1999/xhtml">
+<head runat="server">
+    <title></title>
+</head>
+<body>
+<form id="form1" runat="server">
+<div>
+User Name :-<asp:TextBox ID="tbUserName" runat="server"></asp:TextBox>
+<br />
+<br />
+Password :-<asp:TextBox ID="tbpmd" runat="server"></asp:TextBox>
+<br />
+<asp:Button ID="Buttonl" runat="server" OnClick="Buttonl_Click" Text="Submit" />
+</div>
+</form>
+</body>
+</html>
+
+// login.aspx.cs
+
+using System;
+using System.Collections.Generic;
+using System.Linq;
+using System.Web;
+using System.Web.UI;
+using System.Web.UI.WebControls;
+
+namespace Session1
+{
+    public partial class WebForm2 : System.Web.UI.Page
+    {
+        protected void Page_Load(object sender, EventArgs e)
+        {
+
+        }
+
+        protected void Buttonl_Click(object sender, EventArgs e)
+        {
+            if (tbUserName.Text == "stu" && tbpmd.Text == "123")
+            {
+
+                Session["uname"] = tbUserName.Text;
+                Response.Redirect("WebForm1.aspx");
+            }
+
+            else
+            {
+
+               // Response.Redirect("Default.aspx");
+
+            }
+        }
+    }
+}
+
+<%@ Page Language="C#" AutoEventWireup="true" CodeBehind="WebForm1.aspx.cs" Inherits="Session1.WebForm1" %>
+
+<!DOCTYPE html>
+
+<html xmlns="http://www.w3.org/1999/xhtml">
+<head runat="server">
+    <title></title>
+</head>
+<body>
+    <form id="form2" runat="server">
+<div>
+<asp:Label ID="Label1" runat="server" Text="Label"></asp:Label>
+<br />
+<asp:Button ID="Button2" runat="server" OnClick="Button2_Click" Text="Logout"/>
+    </div>
+    </form>
+</body>
+</html>
+
+using System;
+using System.Collections.Generic;
+using System.Linq;
+using System.Reflection.Emit;
+using System.Web;
+using System.Web.UI;
+using System.Web.UI.WebControls;
+
+namespace Session1
+{
+    public partial class WebForm1 : System.Web.UI.Page
+    {
+        protected void Page_Load(object sender, EventArgs e)
+        {
+            if (Session["uname"] == null)
+            {
+
+                Response.Redirect("Login.aspx");
+            }
+
+            else
+            {
+
+                Label1.Text = "Welcome " + Session["uname"].ToString();
+            }
+
+        }
+
+        protected void Button2_Click(object sender, EventArgs e)
+        {
+            Session["uname"] = null;
+            Response.Redirect("Login.aspx");
+
+        }
+
+        }
+    }
+
+
+'''
+
 awt_codes = {
     "string_functions.txt": string_functions,
     "empregfrom_db_connectivity_insert.txt": empregfrom_db_connectivity_insert,
     "data_grid1.txt": data_grid1,
     "data_grid2.txt": data_grid2,
     "without_data_grid.txt": without_data_grid,
     "file_handling1.txt": file_handling1,
     "validators.txt": validators,
     "validators2.txt": validators2,
     "validators3.txt": validators3,
     "validators4.txt": validators4,
-    "email.txt": email
+    "email.txt": email,
+    "sessions.txt": sessions,
+
 }
 
 def awtcodes_():
     for file,code in awt_codes.items():
         print(file)
     filename = input("Enter filename: ")
     with open(filename, 'w') as f:
```

### Comparing `sbmp-4.0.2/sbmp/iss.py` & `sbmp-4.0.3/sbmp/iss.py`

 * *Files identical despite different names*

### Comparing `sbmp-4.0.2/sbmp.egg-info/PKG-INFO` & `sbmp-4.0.3/sbmp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 4.0.2
+Version: 4.0.3
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-4.0.2/setup.py` & `sbmp-4.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with open('CHANGELOG.txt', 'r') as changelog_file:
         changelog_content = changelog_file.read()
 except FileNotFoundError:
     changelog_content = 'No changelog available.'
 
 setup(
   name='sbmp',
-  version='4.0.2',
+  version='4.0.3',
   description='SBMP',
   long_description=readme_content + '\n\n' + changelog_content,
   url='',  
   author='Jainam Barbhaya',
   author_email='jainambarbhaya1509@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

