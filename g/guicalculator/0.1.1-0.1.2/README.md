# Comparing `tmp/guicalculator-0.1.1.tar.gz` & `tmp/guicalculator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guicalculator-0.1.1.tar", max compression
+gzip compressed data, was "guicalculator-0.1.2.tar", max compression
```

## Comparing `guicalculator-0.1.1.tar` & `guicalculator-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1093 2024-04-17 17:58:02.039277 guicalculator-0.1.1/LICENSE
--rw-r--r--   0        0        0      695 2024-04-18 18:36:07.745298 guicalculator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      619 2024-04-18 13:49:29.244697 guicalculator-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 18:49:53.515810 guicalculator-0.1.1/src/guicalculator/__init__.py
--rw-r--r--   0        0        0      158 2024-04-17 17:45:29.508932 guicalculator-0.1.1/src/guicalculator/__main__.py
--rw-r--r--   0        0        0    11406 2024-04-17 00:17:19.880626 guicalculator-0.1.1/src/guicalculator/buttoncfg.py
--rw-r--r--   0        0        0    37678 2024-04-18 15:29:32.226805 guicalculator-0.1.1/src/guicalculator/guicalculator.py
--rw-r--r--   0        0        0     2499 2024-04-17 18:20:19.755644 guicalculator-0.1.1/src/guicalculator/supportfuncs.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 guicalculator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-17 17:58:02.039277 guicalculator-0.1.2/LICENSE
+-rw-r--r--   0        0        0      695 2024-04-23 12:08:32.555663 guicalculator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      619 2024-04-18 13:49:29.244697 guicalculator-0.1.2/README.md
+-rw-r--r--   0        0        0     1229 2024-04-23 11:23:56.017110 guicalculator-0.1.2/src/guicalculator/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-23 11:24:19.849845 guicalculator-0.1.2/src/guicalculator/__main__.py
+-rw-r--r--   0        0        0     7854 2024-04-23 11:21:52.638136 guicalculator-0.1.2/src/guicalculator/buttoncfg.py
+-rw-r--r--   0        0        0     1797 2024-04-23 11:23:58.373463 guicalculator-0.1.2/src/guicalculator/globals.py
+-rw-r--r--   0        0        0    44051 2024-04-23 11:32:23.420997 guicalculator-0.1.2/src/guicalculator/guicalculator.py
+-rw-r--r--   0        0        0     8983 2024-04-23 11:23:25.196817 guicalculator-0.1.2/src/guicalculator/supportfuncs.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 guicalculator-0.1.2/PKG-INFO
```

### Comparing `guicalculator-0.1.1/LICENSE` & `guicalculator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guicalculator-0.1.1/pyproject.toml` & `guicalculator-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "guicalculator"
-version = "0.1.1"
+version = "0.1.2"
 license = "MIT"
 description = "A calculator written with python and tkinter"
 authors = ["Thomas Brotherton <tombroth@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/tombroth/guicalculator"
 classifiers = [
     "Programming Language :: Python :: 3.12",
```

### Comparing `guicalculator-0.1.1/README.md` & `guicalculator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `guicalculator-0.1.1/src/guicalculator/guicalculator.py` & `guicalculator-0.1.2/src/guicalculator/guicalculator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,41 @@
-import ast
+"""
+guicalculator.py - This is the gui calculator. For an example of how to run it, 
+see __main__.py.
+
+Copyright (c) 2024 Thomas Brotherton
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+"""
+
 import keyword
 import tkinter as tk
 from decimal import Decimal
 from tkinter import scrolledtext, ttk
 from typing import Any, Dict, Tuple
-from unicodedata import normalize
 
-from . import buttoncfg as bc  # type: ignore
-from .supportfuncs import numtostr, strtodecimal, wrap_button_invoke
+from .buttoncfg import ButtonInfo, ButtonLocation, buttons
+from .globals import DEFAULT_VARIABLES, VariablesType
+from .supportfuncs import evaluate_calculation, numtostr, strtodecimal
 
 FONT = ("TkDefaultFont", "12", "bold")
 
 
 class GuiCalculator(tk.Tk):
     """
     GuiCalculator - The root calculator window
@@ -62,50 +86,37 @@
         self.configure("red.TButton", background="orangered2")
         self.configure("memory.TButton", background="lightcyan3")
         self.configure("mathop.TButton", background="cornsilk3")
 
 
 class CalcFrm(ttk.Frame):
     """
-    CalcFrm - The main frame of the calculator root window. Everything is in this frame.
+    CalcFrm - The main frame of the calculator root window. Everything is
+    in this frame.
     """
 
     # data used by the calculator
     current_display_calc: str = ""  # the current caolculation to be displayed
     current_eval_calc: str = ""  # the current calculation to be evalueated
     current_input: str = ""  # the current number input
 
-    pi = "\u03c0"  # Greek letter pi, 3.14....
-
-    # variables stores default variables pi and e and user defined variables
-    # including first 30 digits because default precision is 28 in Decimal
-    # hard coding instead of using math.pi due to float to Decimal rounding issues
-    variables: dict[str, dict[str, Decimal]] = {
-        "default": {
-            normalize("NFKC", pi): Decimal("3.141592653589793238462643383279"),
-            "e": Decimal("2.718281828459045235360287471352"),
-        },
-        "user variables": {},
-    }
+    user_variables: VariablesType = VariablesType({})  # user defined variables
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-        self.buttons = bc.get_buttons(self)  # the list of calculator buttons
-
-        # the map of ast operators to math operators for the parser, gathered from the buttons
-        self.operator_map = {
-            k: v
-            for button in self.buttons
-            if "operators" in button
-            for k, v in button["operators"].items()
-        }
+        # self.buttons = bc.get_buttons(self)  # the list of calculator buttons
 
         # scrolled text display
-        self.display = scrolledtext.ScrolledText(self, height=10, width=20, font=FONT)
+        self.display = scrolledtext.ScrolledText(
+            self,
+            height=10,
+            width=20,
+            font=FONT,
+        )
         # display is only enabled when we write to it
         self.display.configure(state="disabled")
         self.display.grid(row=0, column=0, sticky="news")
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=1)
 
         # frame to hold the memory display
@@ -114,18 +125,21 @@
         self.rowconfigure(1, weight=0)
 
         # frame to hold the buttons
         self.btnfrm = BtnDispFrm(self)
         self.btnfrm.grid(column=0, row=2, sticky="news")
         self.rowconfigure(2, weight=1)
 
-        invk = wrap_button_invoke(self.winfo_toplevel().destroy)
-        self.winfo_toplevel().bind("<Escape>", invk)
+        self.winfo_toplevel().bind(
+            "<Escape>", lambda _: self.winfo_toplevel().destroy()
+        )
 
-    def get_current_display_calc(self, symbol: str = "") -> str:
+    def get_current_display_calc(
+        self, symbol: str = "", func: Tuple[str, str] = None  # type: ignore
+    ) -> str:
         """
         get_current_display_calc - Get the current displayed calculation.
 
         Get the current displayed calculation, including current number input
         and optional mathematical operator.
 
         Parameters
@@ -135,330 +149,485 @@
             will be blank or a mathematical operator, by default "".
 
         Returns
         -------
         str
             The current displayed calculation.
         """
+
         if self.current_input:
-            inpt = numtostr(self.get_current_input(), commas=True, removeZeroes=False)
+            inpt = numtostr(
+                self.get_current_input(),
+                commas=True,
+                removeZeroes=False,
+            )
             if self.current_input[-1] == ".":
                 inpt += "."
         else:
             inpt = ""
-        rv = " ".join(filter(None, [self.current_display_calc, inpt, symbol])).strip()
-        return rv
 
-    def get_current_eval_calc(self, symbol: str = "") -> str:
+        if func and inpt:
+            if func[0] == "1/":
+                inpt = f"({func[0]}{inpt})"
+            else:
+                inpt = f"{func[0]}({inpt})"
+
+        return_value = " ".join(
+            filter(None, [self.current_display_calc, inpt, symbol])
+        ).strip()
+        return return_value
+
+    def get_current_eval_calc(
+        self, symbol: str = "", func: Tuple[str, str] = None  # type: ignore
+    ) -> str:
         """
         get_current_eval_calc - Get the current calculation to be evaluated.
 
-        Get the current calculation to be evaluated, including current number input
-        and optional mathematical operator. The primary difference from
-        get_current_display_calc is that the number inputs are surrounded by calls to
-        Decimal to convert int and float inputs into Decimal to avoid
-        decimal to binary and back to decimal conversion errors.
+        Get the current calculation to be evaluated, including current number
+        input and optional mathematical operator. The primary difference from
+        get_current_display_calc is that the number inputs are surrounded by
+        calls to Decimal to convert int and float inputs into Decimal to avoid
+        decimal to binary and back to decimal rounding errors. In other words
+        0.3 - 0.2 should be 0.1, not 0.09999999999999998.
 
         Parameters
         ----------
         symbol : str, optional
             Optional string to be added to the end of the calculation. Normally
             will be blank or a mathematical operator, by default "".
 
         Returns
         -------
         str
-            _description_
+            The calculation to be evaluated.
         """
+
         if self.current_input:
-            i = +Decimal(self.current_input)
+            i = +self.get_current_input()
             inpt = f"Decimal({str(i)!r})"
         else:
             inpt = ""
-        rv = " ".join([self.current_eval_calc, inpt, symbol]).strip()
-        return rv
+
+        if func and inpt:
+            if func[0] == "1/":
+                inpt = f"({func[1]}{inpt})"
+            else:
+                inpt = f"{func[1]}({inpt})"
+
+        return_value = " ".join([self.current_eval_calc, inpt, symbol]).strip()
+        return return_value
 
     def get_current_input(self) -> Decimal:
         """
         get_current_input - Get current number input as a Decimal.
 
         Returns
         -------
         Decimal
             Decimal version of the number currently being input. 0 if no
             number is currently being input.
         """
+
         if self.current_input:
             return Decimal(self.current_input)
         else:
             return Decimal(0)
 
     def update_display(self) -> None:
         """
         update_display - Update the calculator display.
 
-        This works be erasing the last line that displays the formula
-        being input and replacing it with the most recent changes as
-        returned by get_current_display_calc.
+        This works be erasing the last line that displays the formula being
+        input and replacing it with the most recent changes as returned by
+        get_current_display_calc.
         """
+
         self.display.configure(state="normal")
         # replace last line
         self.display.delete("end-1l", "end")
-        self.display.insert("end", "\n{}".format(self.get_current_display_calc()))
+        self.display.insert("end", f"\n{self.get_current_display_calc()}")
         # move to end
         self.display.see(tk.END)
         self.display.configure(state="disabled")
 
-    def update_current_calc(self, symbol: str = "") -> None:
+    def update_current_calc(
+        self, symbol: str = "", func: Tuple[str, str] = None  # type: ignore
+    ) -> None:
         """
         update_current_calc - Update the current calculation being input.
 
         Uses get_current_display_calc and get_current_eval_calc to generate
         the most recent versions of the calculation being input (including
         the current number being input and the operator being input passed
         in by symbol) and stores them in globals.current_display_calc and
         globals.current_eval_calc. Then calls update_display.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
 
         Parameters
         ----------
         symbol : str, optional
             Optional string to be added to the end of the calculation. Normally
             will be blank or a mathematical operator, by default "".
         """
+
         if self.current_input:  # if we have a value, round it
             self.current_input = numtostr(self.get_current_input())
-        self.current_display_calc = self.get_current_display_calc(symbol)
-        self.current_eval_calc = self.get_current_eval_calc(symbol)
+
+        self.current_display_calc = self.get_current_display_calc(symbol, func)
+        self.current_eval_calc = self.get_current_eval_calc(symbol, func)
         self.current_input = ""
+
         self.update_display()
 
-    def buttonPress(self, symbol: str | int) -> None:
+    def process_button(self, buttoncmd: str, buttontxt: str | int = "") -> None:
+        """
+        process_button - Process a calculator button press.
+
+        Parameters
+        ----------
+        buttoncmd : str
+            The command string from the ButtonInfo dictionary in
+            buttoncfg.py buttons.
+        buttontxt : str | int, optional
+            For buttons in buttoncfg.py that don't have a command
+            (number and basic math symbols) this is the button label,
+            by default ""
         """
-        buttonPress - Handles simple button presses.
+
+        match buttoncmd:
+            case "button":
+                self.button_press(buttontxt)
+
+            case "backspace":
+                self.backspace()
+
+            case "calculate":
+                self.calculate()
+
+            case "clearAll":
+                self.clear_all()
+
+            case "clearValue":
+                self.clear_value()
+
+            case "inverseNumber":
+                self.inverse_number()
+
+            case "invertSign":
+                self.invert_sign()
+
+            case "memAdd":
+                self.memory_add()
+
+            case "memClear":
+                self.memory_clear()
+
+            case "memRecall":
+                self.memory_recall()
+
+            case "memStore":
+                self.memory_store()
+
+            case "memSubtract":
+                self.memory_add(False)
+
+            case "memSwap":
+                self.memory_swap()
+
+            case "rootNumber":
+                self.root_number()
+
+            case "squareNumber":
+                self.square_number()
+
+            case "varsPopup":
+                self.vars_popup()
+
+            case "xToTheY":
+                self.button_press("**")
+            case _:
+                self.bell()
+                print(f"Unknown command: {buttoncmd!r}")
+
+    def button_press(self, symbol: str | int) -> None:
+        """
+        button_press - Handles simple button presses.
 
         Handles simple button presses that just add to the current formula. For
         example, a digit (passed as int, not str), ".", "+", "-", etc. Does not
         handle complex things like computing the square root of the current
         number being input.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context if symbol is not a digit or decimal point.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context if symbol is not a digit or decimal
+        point.
 
         Parameters
         ----------
         symbol : str | int
             The digit or mathematical operator being processed.
         """
+
         if isinstance(symbol, int):
             self.current_input += str(symbol)
             self.update_display()
+
         elif symbol == ".":
-            if not (symbol in self.current_input):
-                if self.current_input:
-                    self.current_input += symbol
-                else:
-                    self.current_input = f"0{symbol}"
-                self.update_display()
+            if symbol in self.current_input:
+                self.bell()
+                return
+
+            self.current_input = (self.current_input or "0") + symbol
+            self.update_display()
+
         else:
             self.update_current_calc(symbol)
 
     def backspace(self) -> None:
         """
         backspace - Erase last character from number being input.
         """
+
         if self.current_input:
             self.current_input = self.current_input[:-1]
         self.update_display()
 
     def clear_value(self) -> None:
         """
         clear_value - Clear the current number input, or if that is empty
         then clear the current calculation.
         """
+
         if self.current_input:
             self.current_input = ""
         else:
             self.current_display_calc = ""
             self.current_eval_calc = ""
+
         self.update_display()
 
-    def clear_everything(self) -> None:
+    def clear_all(self) -> None:
         """
-        clear_everything - Clear the current number being input, the current
+        clear_all - Clear the current number being input, the current
         calculation, and the display. Does not clear the value in memory.
         """
+
         self.display.configure(state="normal")
         self.display.delete(1.0, "end")
         self.display.configure(state="disabled")
+
         self.current_display_calc = ""
         self.current_eval_calc = ""
         self.current_input = ""
+
         self.update_display()
 
     def get_current_memory(self) -> Decimal:
         """
-        get_current_memory - Get the current value stored in memory as a Decimal.
+        get_current_memory - Get the current value stored in memory as a
+        Decimal.
 
         Returns
         -------
         Decimal
             Decimal version of the value stored in memory. 0 if no value is
             currently stored in memory.
         """
+
         mem = self.memfrm.memval.get().replace(",", "")
         if mem:
             return Decimal(mem)
         else:
             return Decimal(0)
 
-    def memClear(self) -> None:
+    def memory_clear(self) -> None:
         """
-        memClear - Clear the value stored in memory
+        memory_clear - Clear the value stored in memory
         """
+
         self.memfrm.memval.set("")
 
-    def memRecall(self) -> None:
+    def memory_recall(self) -> None:
         """
-        memRecall - Replace the current number being input with the value stored
-        in memory.
+        memory_recall - Replace the current number being input with the value
+        stored in memory.
         """
+
         self.current_input = self.memfrm.memval.get().replace(",", "")
         self.update_display()
 
-    def memStore(self) -> None:
+    def memory_store(self) -> None:
         """
-        memStore - Change the value stored in memory to be the same as the current
-        number being input.
+        memory_store - Change the value stored in memory to be the same as the
+        current number being input.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        Cannot do a simple set because we round and format the display.
+
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
+
+        # get and reformat current value
         cur_val = +self.get_current_input()
         self.current_input = numtostr(cur_val)
         self.update_display()
+
+        # store it
         self.memfrm.memval.set(numtostr(cur_val, commas=True))
 
-    def memSwap(self) -> None:
+    def memory_swap(self) -> None:
         """
-        memSwap - Swap the value stored in memory with the current number being input.
+        memory_swap - Swap the value stored in memory with the current number
+        being input.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        Cannot do a simple swap like (a,b) = (b,a) because we need to cal .set
+        on the tk.StringVar that stores the memory value, and we round and
+        format the display.
+
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
+
+        # get current value (formatted with commas)
         cur_num = numtostr(self.get_current_input(), commas=True)
+
+        # store memory in current value
         self.current_input = self.memfrm.memval.get().replace(",", "")
+
+        # store retrieved current value in memory
         self.memfrm.memval.set(cur_num)
+
         self.update_display()
 
-    def memAdd(self, addto: bool = True) -> None:
+    def memory_add(self, addto: bool = True) -> None:
         """
-        memAdd - Add or subtract the current number being input to or from the
-        value stored in memory.
+        memory_add - Add or subtract the current number being input to or from
+        the value stored in memory.
 
         Notes
         -----
-        If addto is passed in as false, will subtract the value being input from
-        memory by multiplying the value by -1 before adding.
+        If addto is passed in as false, will subtract the value being input
+        from memory by multiplying the value by -1 before adding.
 
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
 
         Parameters
         ----------
         addto : bool, optional
-            If true, performs addition. If false, performs subtraction. By default True.
+            If true, performs addition. If false, performs subtraction.
+            By default True.
         """
+
+        # adding or subtracting
         if addto:
             sign = Decimal(1)
         else:
             sign = Decimal(-1)
 
+        # get the current input number (and reformat it)
         cur_val = +self.get_current_input()
         self.current_input = numtostr(cur_val)
         self.update_display()
+
+        # get current memory
         cur_mem = self.get_current_memory()
 
+        # add (or subtract)
         mv = cur_mem + (cur_val * sign)
         self.memfrm.memval.set(numtostr(mv, commas=True))
 
-    def invertSign(self) -> None:
+    def invert_sign(self) -> None:
         """
-        invertSign - Convert the current number being input from
-        positive to negative or negative to positive: x * -1.
+        invert_sign - Convert the current number being input from positive to
+        negative or negative to positive: -x.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
+
         if self.current_input:
-            self.current_input = numtostr(self.get_current_input() * -1)
+            self.current_input = numtostr(-self.get_current_input())
         self.update_display()
 
-    def inverseNumber(self) -> None:
+    def inverse_number(self) -> None:
         """
-        inverseNumber - Convert the current number being input to
-        it's mathematical inverse: 1/x.
+        inverse_number - Convert the current number being input to it's
+        mathematical inverse: 1/x.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
         if self.current_input:
-            self.current_input = numtostr(1 / self.get_current_input())
+            # inpt = self.get_current_input()
+            # if inpt == Decimal(0):
+            #     self.bell()
+            #     return
+
+            # self.current_input = numtostr(1 / inpt)
+            self.update_current_calc(func=("1/", "1/"))
         self.update_display()
 
-    def squareNumber(self) -> None:
+    def square_number(self) -> None:
         """
-        squareNumber - Convert the current number being input to
-        it's square: x**2.
+        square_number - Convert the current number being input to its
+        square: x**2.
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
+
         if self.current_input:
-            self.current_input = numtostr(self.get_current_input() ** 2)
+            # self.current_input = numtostr(self.get_current_input() ** 2)
+            self.update_current_calc("** 2")
         self.update_display()
 
-    def rootNumber(self) -> None:
+    def root_number(self) -> None:
         """
-        rootNumber - Convert the current number being input to
-        it's square root: Decimal.sqrt(x).
+        root_number - Convert the current number being input to its
+        square root: Decimal.sqrt(x).
 
         Notes
         -----
-        As a side effect, will round the number currently being input to precision
-        in Decimal context.
+        As a side effect, will round the number currently being input to the
+        precision in the Decimal context.
         """
+
         if self.current_input:
-            self.current_input = numtostr(Decimal.sqrt(self.get_current_input()))
+            self.update_current_calc(func=("sqrt", "Decimal.sqrt"))
+            # self.current_input = numtostr(Decimal.sqrt(self.get_current_input()))
         self.update_display()
 
     def vars_popup(self) -> None:
         """
-        vars_popup - Display a popup window with currently defined variables.
+        varsPopup - Display a popup window with currently defined variables.
         """
+
+        # get x and y location for popup
         x = self.winfo_toplevel().winfo_x() + 10
         x = max(x, 10)
         y = self.winfo_toplevel().winfo_y() + 175
         y = max(y, 10)
+
         self.varspopup = VarsPopup(calcfrm=self)
         self.varspopup.geometry("+%d+%d" % (x, y))
 
     def calculate(self) -> None:
         """
         calculate - Performs the current calculation and updates the display
         with the results.
@@ -467,16 +636,18 @@
         # update current calc and display
         self.update_current_calc()
 
         # if we have a calculation to perform
         if self.current_eval_calc:
             try:
                 # run the current calculation
-                root_node = ast.parse(self.current_eval_calc, mode="eval")
-                val = self._eval(root_node)
+                val = evaluate_calculation(
+                    self.current_eval_calc,
+                    self.user_variables,
+                )
 
                 # clear current calc and set current input to result
                 self.current_display_calc = ""
                 self.current_eval_calc = ""
                 self.current_input = numtostr(val)
 
                 # show the result
@@ -485,111 +656,28 @@
                     "end", f" =\n{numtostr(val, commas=True)}\n{'=' * 30}\n\n"
                 )
                 self.display.configure(state="disabled")
 
             except Exception as error:
                 # should probably use a logger
                 print(f"ERROR: {error}\n")
+
                 # clear the current calculation and print the error message
                 self.current_display_calc = ""
                 self.current_eval_calc = ""
                 self.current_input = ""
+
+                # show user error message
                 self.display.configure(state="normal")
                 self.display.insert("end", f"\n= ERROR\n\n")
                 self.display.configure(state="disabled")
 
-            # update the display with either the calculated value or the empty string
+            # update the display
             self.update_display()
 
-    def _eval(self, node: ast.AST) -> Decimal:
-        """
-        _eval - Attempt to safely perform the input calculation.
-
-        Works in combination with calculate, uses the ast package to restrict
-        what people can do.
-
-        Parameters
-        ----------
-        node : ast.AST
-            Current node being evaluated
-
-        Returns
-        -------
-        Decimal
-            The result of the current node evaluation. For the root node
-            this is the final answer.
-
-        Raises
-        ------
-        TypeError
-            Used for custom errors, message indicates what the specific error was.
-        """
-        match node:
-            case ast.Expression():
-                return self._eval(node.body)
-            # replaced with Decimal numbers, left in just in case something falls through
-            case ast.Constant():
-                if isinstance(node.value, (int, float)):  # probably overkill
-                    return Decimal(node.value)
-                else:
-                    raise TypeError(f"Unknown constant: ast.{ast.dump(node, indent=2)}")
-            case ast.BinOp():
-                left, right, op = node.left, node.right, node.op
-                method = self.operator_map[type(op)]
-                return method(
-                    self._eval(left),
-                    self._eval(right),
-                )
-            case ast.UnaryOp():
-                operand, uop = node.operand, node.op
-                method = self.operator_map[type(uop)]
-                return method(self._eval(operand))
-            case ast.Name():
-                # unary plus forces rounding to precision in Decimal context
-                if normalize("NFKC", node.id) in self.variables["default"]:
-                    return +self.variables["default"][normalize("NFKC", node.id)]
-
-                elif normalize("NFKC", node.id) in self.variables["user variables"]:
-                    return +self.variables["user variables"][normalize("NFKC", node.id)]
-
-                else:
-                    raise TypeError(
-                        f"Unknown variable: {node.id.encode('unicode_escape')!r}"
-                    )
-            case ast.Call():
-                # if I ever allow more function calls, will have to make another dict
-                if isinstance(node.func, ast.Attribute):  # package.procedure
-                    if isinstance(node.func.value, ast.Name):
-                        pkg = node.func.value.id
-                        func = node.func.attr
-                elif isinstance(node.func, ast.Name):  # procedure (without package.)
-                    pkg = ""
-                    func = node.func.id
-                else:
-                    raise TypeError(
-                        f"Unknown type of ast.Call: \nast.{ast.dump(node, indent=2)}"
-                    )
-
-                if isinstance(node.args[0], ast.Constant):
-                    parm = node.args[0].value
-                else:
-                    parm = ""
-
-                if (pkg == "decimal" and func == "Decimal") or (
-                    pkg == "" and func == "Decimal"
-                ):
-                    # unary plus forces rounding to precision in Decimal context
-                    return +Decimal(parm)
-                else:
-                    raise TypeError(
-                        f"Unknown function call: \nast.{ast.dump(node, indent=2)}"
-                    )
-            case _:
-                raise TypeError(f"Unknown ast node: \nast.{ast.dump(node, indent=2)}")
-
 
 class MemDispFrm(ttk.Frame):
     """
     MemDispFrm - The memory display frame.
     """
 
     def __init__(self, *args, **kwargs) -> None:
@@ -612,47 +700,104 @@
     BtnDispFrm - The calculator button display frame.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # each row with a different number of buttons is a different frame
-        # this dict keeps track of them all
-        self.btnfrms: Dict[int, ttk.Frame] = {}
+        # this dict keeps track of all the frames
+        self.button_frames: Dict[int, ttk.Frame] = {}
 
         # this frame contains only frames, so has only one column
         self.columnconfigure(0, weight=1)
 
-        for btn in self.master.buttons:  # type: ignore
+        # the keys in buttons are tuples of frame, row, column
+        # sorting them ensures we process in the correct order
+        for btn_loc, btn_info in sorted(buttons.items()):
+            self.add_button(btn_loc, btn_info)
 
-            # if we have a new frame to add
-            if btn["btnfrm"] not in self.btnfrms:
+    def add_button(self, btn_loc: ButtonLocation, btn_info: ButtonInfo) -> None:
+        """
+        add_button - add a button to BtnDispFrm
 
-                self.btnfrms[btn["btnfrm"]] = ttk.Frame(self)
-                self.btnfrms[btn["btnfrm"]].grid(
-                    column=0, row=btn["btnfrm"], sticky="news"
-                )
-                self.rowconfigure(btn["btnfrm"], weight=1)
+        Parameters
+        ----------
+        button_loc : ButtonLocation
+            Button location information
+        button_info : ButtonInfo
+            Button creation information
+        """
+
+        """
+        at the paranoid level should proably validate that
+        everything in button_loc and button_info is what it
+        should be and not an injection attack
+        """
+
+        # if we have a new frame to add
+        if btn_loc.btn_frame not in self.button_frames:
+
+            self.button_frames[btn_loc.btn_frame] = ttk.Frame(self)
 
-            # add this button to this frame
-            b = ttk.Button(self.btnfrms[btn["btnfrm"]], **btn["btnopts"])
-            b.grid(**btn["gridopts"])
-
-            # if this button is binding any events ...
-            if "bindevents" in btn:
-                invk = wrap_button_invoke(b.invoke)
-                for be in btn["bindevents"]:
-                    self.winfo_toplevel().bind(be, invk)
-
-            # configure the weigts for the buttons
-            self.btnfrms[btn["btnfrm"]].rowconfigure(btn["gridopts"]["row"], weight=1)
-            self.btnfrms[btn["btnfrm"]].columnconfigure(
-                btn["gridopts"]["column"], weight=1
+            self.button_frames[btn_loc.btn_frame].grid(
+                column=0,
+                row=btn_loc.btn_frame,
+                sticky="news",
             )
-            self.rowconfigure(btn["btnfrm"], weight=btn["gridopts"]["row"] + 1)
+
+        # create the button
+        cf: CalcFrm = self.master  # type: ignore
+        if "command" in btn_info:
+            cmd = lambda x=btn_info["command"]: cf.process_button(x)
+        else:
+            cmd = lambda x=btn_info["label"]: cf.process_button("button", x)
+
+        btnopts: dict = {"text": btn_info["label"], "command": cmd}
+        if "style" in btn_info:
+            btnopts["style"] = btn_info["style"]
+
+        cur_btn = ttk.Button(self.button_frames[btn_loc.btn_frame], **btnopts)
+
+        # add the button to the frame
+        gridopts: dict = {
+            "row": btn_loc.btn_row,
+            "column": btn_loc.btn_column,
+            "sticky": "news",
+        }
+
+        if "rowspan" in btn_info:
+            gridopts["rowspan"] = btn_info["rowspan"]
+
+        if "columnspan" in btn_info:
+            gridopts["columnspan"] = btn_info["columnspan"]
+
+        cur_btn.grid(**gridopts)
+
+        # if this button is binding any events ...
+
+        if "events" in btn_info:
+            for be in btn_info["events"]:
+                topwin = self.winfo_toplevel()
+                topwin.bind(be, lambda _, c=cur_btn: c.invoke())  # type: ignore
+
+        # configure the weigts for the buttons
+        self.button_frames[btn_loc.btn_frame].rowconfigure(
+            btn_loc.btn_row,
+            weight=1,
+        )
+        self.button_frames[btn_loc.btn_frame].columnconfigure(
+            btn_loc.btn_column,
+            weight=1,
+        )
+        # the weight of the subframe should be proportional to the
+        # number of rows in the subframe
+        self.rowconfigure(
+            btn_loc.btn_frame,
+            weight=btn_loc.btn_row + 1,
+        )
 
 
 class VarsPopup(tk.Toplevel):
     """
     VarsPopup - The popup window to display variables.
     """
 
@@ -663,19 +808,18 @@
         self.wm_title("Variables")
 
         self.treefrm = VarsPopupTreeFrm(self, calcfrm=calcfrm)
         self.treefrm.grid(row=0, column=0, sticky="news")
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
 
-        if self.treefrm.vars_tree.get_children():
-            self.treefrm.vars_tree.focus(self.treefrm.vars_tree.get_children()[0])
-            self.treefrm.vars_tree.selection_set(
-                self.treefrm.vars_tree.get_children()[0]
-            )
+        vars_tree = self.treefrm.vars_tree
+        if vars_tree.get_children():
+            vars_tree.focus(vars_tree.get_children()[0])
+            vars_tree.selection_set(vars_tree.get_children()[0])
 
 
 class VarsPopupTreeFrm(ttk.Frame):
     """
     VarsPopupTreeFrm - The frame with the variables displayed.
     """
 
@@ -693,96 +837,136 @@
             columns=("value"),
             height=7,
             selectmode="browse",
         )
         self.scrollbar.configure(command=self.vars_tree.yview)
         self.vars_tree.focus_set()
 
-        # our columns in the tree view
-        self.vars_tree.heading("#0", text="Variable")
-        self.vars_tree.column("#0", width=150, anchor="w")
-
-        self.vars_tree.heading("value", text="Value")
-        self.vars_tree.column("value", width=325, anchor="w")
-
         self.vars_tree.grid(row=0, column=0, sticky="news")
         self.scrollbar.grid(row=0, column=1, sticky="ns")
 
         self.columnconfigure(0, weight=1)
         self.columnconfigure(1, weight=0)
         self.rowconfigure(0, weight=1)
 
-        # this loop iterates over the variables and adds them to the treeview
-        for section, vars in self.calcfrm.variables.items():
-            section_id = self.vars_tree.insert("", "end", text=section, values=([""]))
-            for v_key, v_value in vars.items():
-                self.vars_tree.insert(
-                    section_id,
-                    "end",
-                    text=v_key,
-                    values=([numtostr(v_value, commas=True)]),
-                )
-            self.vars_tree.item(section_id, open=True)
+        # our columns in the tree view
+        self.vars_tree.heading("#0", text="Variable")
+        self.vars_tree.column("#0", width=150, anchor="w")
+
+        self.vars_tree.heading("value", text="Value")
+        self.vars_tree.column("value", width=325, anchor="w")
+
+        # this loop iterates over the default variables and adds
+        # them to the treeview
+        self.add_variable_section("default", DEFAULT_VARIABLES)
+
+        # this loop iterates over the user variables and adds
+        # them to the treeview
+        self.add_variable_section("user variables", self.calcfrm.user_variables)
 
         # add buttons to select or edit user variables
         self.buttonfrm = VarsPopupTreeFrmButtons(self, vptf=self)
         self.buttonfrm.grid(row=1, column=0, sticky="news")
         self.rowconfigure(1, weight=0)
 
+        # double click to select
+        self.vars_tree.bind(
+            "<Double-Button-1>", lambda _: self.buttonfrm.select_button.invoke()
+        )
+
+    def add_variable_section(
+        self, section_name: str, section_vars: VariablesType
+    ) -> None:
+        """
+        add_variable_section - Add a variable dictionary to the tree frame
+
+        Parameters
+        ----------
+        section_name : str
+            Section Name
+        section_vars : VariablesType : dict[str, Decimal]
+            Variables
+        """
+
+        section_id = self.vars_tree.insert(
+            "",
+            "end",
+            text=section_name,
+            values=([""]),
+        )
+        for v_key, v_value in section_vars.items():
+            self.vars_tree.insert(
+                section_id,
+                "end",
+                text=v_key,
+                values=([numtostr(v_value, commas=True)]),
+            )
+        self.vars_tree.item(section_id, open=True)
+
 
 class VarsPopupTreeFrmButtons(ttk.Frame):
     """
-    VarsPopupTreeFrmButtons - The frame with the buttons in the variables popup window.
+    VarsPopupTreeFrmButtons - The frame with the buttons in the variables
+    popup window.
 
     """
 
     def __init__(self, *args, vptf: VarsPopupTreeFrm, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.vptf = vptf
 
-        self.select_button = ttk.Button(
+        self.edit_button = ttk.Button(
             self,
-            text="Select",
-            command=self.user_vars_select,
+            text="Edit User Variables",
+            command=self.user_vars_edit,
         )
-        self.select_button.grid(row=0, column=0)
+        self.edit_button.grid(row=0, column=0, columnspan=2)
         self.columnconfigure(0, weight=1)
         self.rowconfigure(0, weight=0)
 
-        invk = wrap_button_invoke(self.select_button.invoke)
-        self.winfo_toplevel().bind("<Return>", invk)
-
-        invk = wrap_button_invoke(self.winfo_toplevel().destroy)
-        self.winfo_toplevel().bind("<Escape>", invk)
+        self.cancel_button = ttk.Button(
+            self,
+            text="Cancel",
+            command=self.winfo_toplevel().destroy,
+        )
+        self.cancel_button.grid(row=1, column=0)
+        self.rowconfigure(1, weight=0)
 
-        self.edit_button = ttk.Button(
+        self.select_button = ttk.Button(
             self,
-            text="Edit User Variables",
-            command=self.user_vars_edit,
+            text="Select",
+            command=self.user_vars_select,
         )
-        self.edit_button.grid(row=0, column=1)
+        self.select_button.grid(row=1, column=1)
         self.columnconfigure(1, weight=1)
 
-    def user_vars_select(self):
+        top_win = self.winfo_toplevel()
+        top_win.bind("<Return>", lambda _: self.select_button.invoke())
+        top_win.bind("<Escape>", lambda _: self.winfo_toplevel().destroy())
+
+    def user_vars_select(self) -> None:
         """
         user_vars_select - Return selected variable to the calculator.
         """
 
-        # if we have one of the variables selected (not on "default" or "user variables")
+        vars_tree = self.vptf.vars_tree
+
+        # if we have one of the variables selected
+        # not on "default" or "user variables"
         if (
-            self.vptf.vars_tree.selection()
-            and self.vptf.vars_tree.selection()[0]
-            not in self.vptf.vars_tree.get_children()
+            vars_tree.selection()
+            and vars_tree.selection()[0] not in vars_tree.get_children()
         ):
-            self.vptf.calcfrm.buttonPress(
-                self.vptf.vars_tree.item(self.vptf.vars_tree.selection()[0])["text"]
+            self.vptf.calcfrm.button_press(
+                vars_tree.item(vars_tree.selection()[0])["text"]
             )
+
         self.winfo_toplevel().destroy()
 
-    def user_vars_edit(self):
+    def user_vars_edit(self) -> None:
         """
         user_vars_edit - Popup window to edit the user variables.
         """
         editvars_win = UserVarsEditPopup(calcfrm=self.vptf.calcfrm)
 
         x = self.winfo_toplevel().winfo_x()
         y = self.winfo_toplevel().winfo_y()
@@ -804,14 +988,17 @@
         self.treefrm = UserVarsEditFrm(self, calcfrm=calcfrm)
         self.treefrm.grid(row=0, column=0, sticky="news")
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
 
 
 class UserVarsEditFrm(tk.Frame):
+    """
+    UserVarsEditFrm - The frame with the user variables edit widgets
+    """
 
     def __init__(self, *args, calcfrm: CalcFrm, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.calcfrm = calcfrm
 
         # column headers
         self.var_lbl = ttk.Label(self, text="User Variable", width=16)
@@ -822,72 +1009,139 @@
         self.val_lbl.grid(row=lastrow, column=1, sticky="we")
 
         self.rowconfigure(lastrow, weight=0)
         self.columnconfigure(0, weight=1)
         self.columnconfigure(1, weight=1)
 
         # validate functions for name/value
-        self.validvarname = (self.register(self.validate_varname), "%P")
-        self.validvalue = (self.register(self.validate_decimal), "%P")
+        self.validate_var_name = (self.register(self.validate_varname), "%P")
+        self.validate_value = (self.register(self.validate_decimal), "%P")
+
+        """
+        variable name/value entry widgets
 
-        # variable name/value entry widgets
-        # this stores a dictionary of all the Text entry boxes for editing user variables
-        # the Tuple[int, int] index is the row and column of the entry widget
-        # column 0 is variable name
-        # column 1 is variable value
+        This dictionary stores all the Text entry boxes for editing 
+        user variables.
+        
+        The tuple[int, int] index is the row and column of the entry widget
+
+        The frame row 0 is the header, so the first variable is row 1.
+
+        Column 0 is variable name.
+        Column 1 is variable value.
+
+        So the first variable name is the entry widget at uservars[1,0] 
+        not at uservars[0,0].
+        """
         self.uservars: dict[Tuple[int, int], ttk.Entry] = {}
 
-        for k, v in calcfrm.variables["user variables"].items():
+        for k, v in calcfrm.user_variables.items():
             lastrow += 1
             self.addrow(lastrow, k, numtostr(v, commas=True))
 
+        # if we had no rows, add a blank one
         if not self.uservars:
             lastrow += 1
             self.addrow(lastrow)
 
         self.uservars[(1, 0)].focus_set()
 
-        # put these at row 1000 to allow for insertint more rows
+        # put these at row 1000 to allow for inserting more rows
         # add row button
         self.addbtn = ttk.Button(
             self,
             text="Add Row",
             command=self.user_vars_edit_addrow,
         )
-        self.addbtn.grid(row=1000, column=0, columnspan=2)
+        self.addbtn.grid(row=1000, column=0)
         self.rowconfigure(1000, weight=0)
 
-        # cancel button
-        self.cancelbtn = ttk.Button(
-            self, text="Cancel", command=self.winfo_toplevel().destroy
+        # add delete row nutton
+        self.delbtn = ttk.Button(
+            self,
+            text="Delete Row",
+            command=self.user_vars_edit_delrow,
+            takefocus=False,
         )
-        self.cancelbtn.grid(row=1001, column=0)
+        self.delbtn.grid(row=1000, column=1)
+
+        # add current_calculation button
+        self.curcalcbtn = ttk.Button(
+            self,
+            text="Add current result as new variable",
+            command=self.add_current,
+        )
+        self.curcalcbtn.grid(row=1001, column=0, columnspan=2)
         self.rowconfigure(1001, weight=0)
 
-        invk = wrap_button_invoke(self.cancelbtn.invoke)
-        self.winfo_toplevel().bind("<Escape>", invk)
+        topwin = self.winfo_toplevel()
+        # cancel button
+        self.cancelbtn = ttk.Button(self, text="Cancel", command=topwin.destroy)
+        self.cancelbtn.grid(row=1002, column=0)
+        self.rowconfigure(1002, weight=0)
+
+        topwin.bind("<Escape>", lambda _: self.cancelbtn.invoke())
 
         # ok button
         self.okbtn = ttk.Button(
             self,
             text="Ok",
             command=self.user_vars_edit_ok,
         )
-        self.okbtn.grid(row=1001, column=1)
+        self.okbtn.grid(row=1002, column=1)
 
-        invk = wrap_button_invoke(self.okbtn.invoke)
-        self.winfo_toplevel().bind("<Return>", invk)
+        topwin.bind("<Return>", lambda _: self.okbtn.invoke())
 
         # error message display
         self.errmsg = tk.StringVar(self)
         self.errmsg_lbl = ttk.Label(self, anchor="w", textvariable=self.errmsg)
-        self.errmsg_lbl.grid(row=1002, column=0, columnspan=2, sticky="news")
-        self.rowconfigure(1002, weight=0)
+        self.errmsg_lbl.grid(row=1003, column=0, columnspan=2, sticky="news")
+        self.rowconfigure(1003, weight=0)
+
+    def user_vars_edit_delrow(self) -> None:
+        """Delete the current row"""
+
+        # find the current row
+        cur_widget = self.winfo_toplevel().focus_get()
+        if cur_widget in list(self.uservars.values()):
+            widget_num = list(self.uservars.values()).index(cur_widget)  # type: ignore
+            row = list(self.uservars.keys())[widget_num][0]
+
+            # found it, now destroy entry widgets and remove from dictionary
+            self.uservars[(row, 0)].destroy()
+            self.uservars[(row, 1)].destroy()
+            self.uservars.pop((row, 0), None)
+            self.uservars.pop((row, 1), None)
+
+            # if we still have entry widgets, set focus to one of them
+            if self.uservars:
+                remaining_vars = list(self.uservars.keys())
+                if widget_num >= len(remaining_vars):
+                    widget_num = -1
+                self.uservars[remaining_vars[widget_num]].focus_set()
+
+    def add_current(self) -> None:
+        """Add the current calculation result as a variable"""
+
+        currcalc = self.calcfrm.get_current_display_calc()
+        if currcalc:
+            # get the result
+            self.calcfrm.calculate()
+            result = self.calcfrm.get_current_input()
+
+            # add result to a new row
+            row = self.user_vars_edit_addrow()
 
-    def addrow(self, rownum: int, var: str = "", val: str = ""):
+            self.uservars[(row, 0)].delete(0, tk.END)
+            self.uservars[(row, 0)].insert(0, "x")
+
+            self.uservars[(row, 1)].delete(0, tk.END)
+            self.uservars[(row, 1)].insert(0, numtostr(result, commas=True))
+
+    def addrow(self, rownum: int, var: str = "", val: str = "") -> None:
         """
         addrow - Add a row for a new variable
 
         Parameters
         ----------
         rownum : int
             Row number
@@ -896,15 +1150,15 @@
         val : str, optional
             Variable value, by default ""
         """
 
         self.addtextbox(rownum, 0, var)
         self.addtextbox(rownum, 1, val)
 
-    def addtextbox(self, rownum: int, colnum: int, text: str = ""):
+    def addtextbox(self, rownum: int, colnum: int, text: str = "") -> None:
         """
         addtextbox - Add a text entry box for variable name or variable value
 
         Parameters
         ----------
         rownum : int
             Text box row number
@@ -912,43 +1166,48 @@
             Text box column number, 0 for variable name, 1 for variable value
         text : str, optional
             Initial text to put in box, by default ""
         """
 
         entopts: dict[str, Any]  # entry widget validation options
         if colnum == 0:
-            entopts = {"validate": "key", "validatecommand": self.validvarname}
+            entopts = {
+                "validate": "key",
+                "validatecommand": self.validate_var_name,
+            }
         elif colnum == 1:
-            entopts = {"validate": "key", "validatecommand": self.validvalue}
+            entopts = {
+                "validate": "key",
+                "validatecommand": self.validate_value,
+            }
         else:
             entopts = {}
 
         tbox = ttk.Entry(self, width=(16 * (colnum + 1)), font=FONT, **entopts)
         tbox.insert(tk.INSERT, text)
         tbox.grid(row=rownum, column=colnum, sticky="news")
         self.uservars[(rownum, colnum)] = tbox
         self.rowconfigure(rownum, weight=1)
 
         if colnum == 1:
-            tbox.bind("<KeyRelease>", self.formatnumber)
+            tbox.bind("<KeyRelease>", self.format_number)
 
-    def formatnumber(self, event: tk.Event) -> None:
+    def format_number(self, event: tk.Event) -> None:
         """
         formatnumber - Format the number input
 
         Parameters
         ----------
         event : tk.Event
             The event triggering this call
         """
 
         v = event.widget.get()
         if v:
-            # if we have an entry, get it, convert to decimal, then reconvert to string
-            # so that we can format it
+            # if we have an entry, get it and format it
             v_decimal = strtodecimal(v)
             v_str = numtostr(v_decimal, commas=True, removeZeroes=False)
             if v[-1] == ".":
                 v_str += "."
             event.widget.delete(0, tk.END)
             event.widget.insert(0, v_str)
 
@@ -992,86 +1251,109 @@
         -------
         bool
             True if the number is a valid Decimal, False if not.
         """
 
         if newval:
             try:
-                d = strtodecimal(newval)
-                # self.winfo_toplevel().nametowidget(thiswidget).set(numtostr(newval, commas=True))
-                # with self.winfo_toplevel().nametowidget(thiswidget) as w:
-                #     w.delete(0, len(w.get()))
-                #     w.insert(0, numtostr(newval, commas=True))
+                _ = strtodecimal(newval)
             except:
                 self.bell()
                 return False
 
         return True
 
-    def user_vars_edit_addrow(self):
+    def user_vars_edit_addrow(self) -> int:
         """
-        user_vars_edit_addrow - Add a row for a new user variable to the user_vars_edit window
+        user_vars_edit_addrow - Add a row for a new user variable. Returns row number added
         """
 
         if self.uservars.keys():
             nextrow = max(r for (r, _) in self.uservars.keys()) + 1
         else:
             nextrow = 1
 
         self.addrow(nextrow)
         self.uservars[(nextrow, 0)].focus_set()
 
-    def user_vars_edit_ok(self):
+        return nextrow
+
+    def user_vars_edit_ok(self) -> None:
         """
         user_vars_edit_ok - Update the user variables from entered data
         """
 
-        newuservars: dict[str, Decimal] = {}  # type: ignore
-
-        if not self.uservars:
-            lastrow = 0
+        newuservars: VariablesType = VariablesType({})
 
+        if self.uservars:
+            k = self.uservars.keys()
+            rows = set(list(zip(*k))[0])
         else:
-            lastrow = max(r for (r, _) in self.uservars.keys())
+            rows = set()
 
-        for i in range(1, lastrow + 1):
+        for i in rows:
             # user variable name
             nam = self.uservars[(i, 0)].get().strip()
 
+            # common parts of these error messages
+            # extracted for consistency in messaging
+            errmsg = f"ERROR:"
+            varnam = f"variable name {nam!r}"
+
             # if we don't have a valid identifier, print an error
             if not nam.isidentifier():
-                self.errmsg.set(f"ERROR on row {i}: invalid variable name {nam!r}")
+                self.set_errmsg(f"{errmsg} invalid {varnam}")
+                self.uservars[(i, 0)].focus_set()
                 return
 
             # if we have a keyword, print an error
             if keyword.iskeyword(nam):
-                self.errmsg.set(
-                    f"ERROR on row {i}: variable name {nam!r} is a reserved word"
-                )
+                self.set_errmsg(f"{errmsg} {varnam} is a reserved word")
+                self.uservars[(i, 0)].focus_set()
                 return
 
             # if we  have a duplicate variable name, print an error
-            if nam in newuservars.keys():
-                self.errmsg.set(f"ERROR on row {i}, duplicate variable name {nam!r}")
+            if nam in newuservars.keys() or nam in DEFAULT_VARIABLES.keys():
+                self.set_errmsg(f"{errmsg} duplicate {varnam}")
+                self.uservars[(i, 0)].focus_set()
                 return
 
             # new user variable value
             val = self.uservars[(i, 1)].get().strip()
 
+            # if we don't have a value, print an error
+            if not val:
+                self.set_errmsg(f"{errmsg} value not set")
+                self.uservars[(i, 1)].focus_set()
+                return
+
             # if we don't have a valid Decimal value, print an error
             try:
                 val_decimal = +strtodecimal(val)
             except:
-                self.errmsg.set(f"ERROR on row {i}, invalid numeric value {val!r}")
+                self.set_errmsg(f"{errmsg} invalid numeric value {val!r}")
+                self.uservars[(i, 1)].focus_set()
                 return
 
             newuservars[nam] = val_decimal
 
         # save the new variables
-        self.calcfrm.variables["user variables"] = newuservars
+        self.calcfrm.user_variables = newuservars
 
         # close this window
         self.winfo_toplevel().destroy()
 
         # rebuild the varspopup
         self.calcfrm.varspopup.destroy()
         self.calcfrm.vars_popup()
+
+    def set_errmsg(self, error_msg: str) -> None:
+        """
+        set_errmsg - Set the error message and ring a bell
+
+        Parameters
+        ----------
+        error_msg : str
+            Error message to display
+        """
+        self.bell()
+        self.errmsg.set(error_msg)
```

### Comparing `guicalculator-0.1.1/PKG-INFO` & `guicalculator-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guicalculator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A calculator written with python and tkinter
 Home-page: https://github.com/tombroth/guicalculator
 License: MIT
 Author: Thomas Brotherton
 Author-email: tombroth@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

