# Comparing `tmp/cs.taskqueue-20230401.tar.gz` & `tmp/cs.taskqueue-20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.taskqueue-20230401.tar", last modified: Sat Apr  1 08:48:01 2023, max compression
+gzip compressed data, was "cs.taskqueue-20240423.tar", last modified: Tue Apr 23 09:29:29 2024, max compression
```

## Comparing `cs.taskqueue-20230401.tar` & `cs.taskqueue-20240423.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 08:48:01.681223 cs.taskqueue-20230401/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-01 08:47:45.000000 cs.taskqueue-20230401/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     7996 2023-04-01 08:48:01.681349 cs.taskqueue-20230401/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    12887 2023-04-01 08:47:46.000000 cs.taskqueue-20230401/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 08:48:01.676572 cs.taskqueue-20230401/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 08:48:01.676901 cs.taskqueue-20230401/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 08:48:01.678943 cs.taskqueue-20230401/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    30974 2023-04-01 08:47:30.000000 cs.taskqueue-20230401/lib/python/cs/taskqueue.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 08:48:01.680914 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     7996 2023-04-01 08:48:01.000000 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      316 2023-04-01 08:48:01.000000 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-01 08:48:01.000000 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      262 2023-04-01 08:48:01.000000 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-01 08:48:01.000000 cs.taskqueue-20230401/lib/python/cs.taskqueue.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     8530 2023-04-01 08:47:51.000000 cs.taskqueue-20230401/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1120 2023-04-01 08:48:01.681952 cs.taskqueue-20230401/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-01 08:47:46.000000 cs.taskqueue-20230401/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:29:29.630397 cs.taskqueue-20240423/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-23 09:28:51.000000 cs.taskqueue-20240423/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13451 2024-04-23 09:29:29.630038 cs.taskqueue-20240423/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12670 2024-04-23 09:28:53.000000 cs.taskqueue-20240423/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:29:29.625839 cs.taskqueue-20240423/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:29:29.626155 cs.taskqueue-20240423/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:29:29.627650 cs.taskqueue-20240423/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    31016 2024-04-23 09:27:46.000000 cs.taskqueue-20240423/lib/python/cs/taskqueue.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:29:29.629561 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    13451 2024-04-23 09:28:57.000000 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-23 09:29:29.000000 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-23 09:28:57.000000 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      262 2024-04-23 09:28:57.000000 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-23 09:29:29.000000 cs.taskqueue-20240423/lib/python/cs.taskqueue.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14162 2024-04-23 09:28:56.000000 cs.taskqueue-20240423/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-23 09:29:29.630500 cs.taskqueue-20240423/setup.cfg
```

### Comparing `cs.taskqueue-20230401/README.md` & `cs.taskqueue-20240423/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 A general purpose Task and TaskQueue for running tasks with
 dependencies and failure/retry, potentially in parallel.
 
-*Latest release 20230401*:
-Add missing requirement to DISTINFO.
+*Latest release 20240423*:
+Small fixes.
 
-## Class `BaseTask(cs.fsm.FSM, cs.gvutils.DOTNodeMixin, cs.resources.RunStateMixin)`
+## Class `BaseTask(cs.fsm.FSM, cs.resources.RunStateMixin)`
 
 A base class subclassing `cs.fsm.FSM` with a `RunStateMixin`.
 
 Note that this class and the `FSM` base class does not provide
 a `FSM_DEFAULT_STATE` attribute; a default `state` value of
 `None` will leave `.fsm_state` _unset_.
 
@@ -42,15 +42,15 @@
         * `sep`: optional node seprator, default `'
 '`
 
 *Method `BaseTask.tasks_as_svg(tasks, name=None, **kw)`*:
 Return an SVG diagram of the iterable `tasks`.
 This takes the same parameters as `tasks_as_dot`.
 
-## Class `BlockedError(TaskError, cs.fsm.FSMError, builtins.Exception, builtins.BaseException)`
+## Class `BlockedError(TaskError)`
 
 Raised by a blocked `Task` if attempted.
 
 ## Function `main(argv)`
 
 Dummy main programme to exercise something.
 
@@ -101,15 +101,15 @@
 queue the task and its prerequisites for execution.
 
 ## Function `make_now(*tasks, fail_fast=False, queue=None)`
 
 Run the generator `make(*tasks)` to completion and return the
 list of completed tasks.
 
-## Class `Task(BaseTask, cs.fsm.FSM, cs.gvutils.DOTNodeMixin, cs.resources.RunStateMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Task(BaseTask, cs.threads.HasThreadState)`
 
 A task which may require the completion of other tasks.
 
 The model here may not be quite as expected; it is aimed at
 tasks which can be repaired and rerun.
 As such, if `self.run(func,...)` raises an exception from
 `func` then this `Task` will still block dependent `Task`s.
@@ -260,15 +260,15 @@
     >>> t_leaf.make()          # make the leaf, but make t_root first
     True
     >>> t_root.iscompleted()   # implicitly completed by make
     True
     >>> t_leaf.iscompleted()
     True
 
-## Class `TaskError(cs.fsm.FSMError, builtins.Exception, builtins.BaseException)`
+## Class `TaskError(cs.fsm.FSMError)`
 
 Raised by `Task` related errors.
 
 ## Class `TaskQueue`
 
 A task queue for managing and running a set of related tasks.
 
@@ -334,14 +334,17 @@
 but its semantics might mean it is in another state such as `CANCELLED`.
 The consumer of `run` must handle these situations.
 
 # Release Log
 
 
 
+*Release 20240423*:
+Small fixes.
+
 *Release 20230401*:
 Add missing requirement to DISTINFO.
 
 *Release 20230331*:
 * Task: subclass BaseTask instead of (FSM, RunStateMixin).
 * BaseTask.__init__: use @uses_runstate to ensure we've got a RunState.
```

### Comparing `cs.taskqueue-20230401/lib/python/cs/taskqueue.py` & `cs.taskqueue-20240423/lib/python/cs/taskqueue.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from cs.queues import ListQueue
 from cs.resources import RunState, RunStateMixin, uses_runstate
 from cs.result import Result, CancellationError
 from cs.seq import Seq, unrepeated
 from cs.threads import bg as bg_thread, locked, ThreadState, HasThreadState
 from cs.typingutils import subtype
 
-__version__ = '20230401'
+__version__ = '20240423'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
@@ -107,17 +107,17 @@
       `FSM_DEFAULT_STATE` class attribute thus breaks this method.
       Subclasses of this class and `Model` should _not_ provide a
       `FSM_DEFAULT_STATE` attribute, instead relying on the field
       definition to provide this default in the usual way.
   '''
 
   @uses_runstate
-  def __init__(self, *, state=None, runstate=None):
+  def __init__(self, *, state=None, runstate: RunState):
     FSM.__init__(self, state)
-    RunStateMixin.__init__(self, runstate)
+    RunStateMixin.__init__(self, runstate=runstate)
 
   @classmethod
   def tasks_as_dot(
       cls,
       tasks,
       name=None,
       *,
@@ -291,14 +291,16 @@
       cancel_on_result=None,
       track=False,
   ):
     if func is None or isinstance(func, str):
       name = func
       a = list(a)
       func = a.pop(0)
+    else:
+      name = None
     if name is None:
       name = funcname(func)
     self.name = name
     if a:
       raise ValueError(
           "unexpected positional parameters after func:%r: %r" % (func, a)
       )
@@ -401,17 +403,17 @@
           func_args=func_args,
           func_kwargs=func_kwargs,
           **task_kw,
       )
     post_task.require(self)
     return post_task
 
-  @typechecked
   @require(lambda self, otask: otask is not self)
   @require(lambda self: self.is_prepare or self.is_pending)
+  @typechecked
   def require(self, otask: 'TaskSubType'):
     ''' Add a requirement that `otask` be complete before we proceed.
         This is the simple `Task` only version of `.then()`.
     '''
     with self._lock:
       self.required.add(otask)
       otask.blocking.add(self)
```

### Comparing `cs.taskqueue-20230401/pyproject.toml` & `cs.taskqueue-20240423/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 authors = [
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20230331",
-    "cs.fsm>=20221118",
-    "cs.gvutils>=20221207",
+    "cs.deco>=20240412",
+    "cs.fsm>=20240316",
+    "cs.gvutils>=20230816",
     "cs.logutils>=20230212",
-    "cs.pfx>=20230331",
+    "cs.pfx>=20240412",
     "cs.py.func>=20230331",
-    "cs.queues>=20230331",
-    "cs.resources>=20230331",
-    "cs.result>=20230331",
+    "cs.queues>=20240412",
+    "cs.resources>=20240423",
+    "cs.result>=20240412",
     "cs.seq>=20221118",
-    "cs.threads>=20230331",
+    "cs.threads>=20240422",
     "cs.typingutils>=20230331",
     "icontract",
     "typeguard",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230401"
+version = "20240423"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 A general purpose Task and TaskQueue for running tasks with
 dependencies and failure/retry, potentially in parallel.
 
-*Latest release 20230401*:
-Add missing requirement to DISTINFO.
+*Latest release 20240423*:
+Small fixes.
 
-## Class `BaseTask(cs.fsm.FSM, cs.gvutils.DOTNodeMixin, cs.resources.RunStateMixin)`
+## Class `BaseTask(cs.fsm.FSM, cs.resources.RunStateMixin)`
 
 A base class subclassing `cs.fsm.FSM` with a `RunStateMixin`.
 
 Note that this class and the `FSM` base class does not provide
 a `FSM_DEFAULT_STATE` attribute; a default `state` value of
 `None` will leave `.fsm_state` _unset_.
 
@@ -60,15 +60,40 @@
 whose `refresh_from_db` method seems to not refresh fields
 which already exist, and setting `.fsm_state` from a
 `FSM_DEFAULT_STATE` class attribute thus breaks this method.
 Subclasses of this class and `Model` should _not_ provide a
 `FSM_DEFAULT_STATE` attribute, instead relying on the field
 definition to provide this default in the usual way.
 
-## Class `BlockedError(TaskError, cs.fsm.FSMError, builtins.Exception, builtins.BaseException)`
+*Method `BaseTask.as_dot(self, name=None, **kw)`*:
+Return a DOT syntax digraph starting at this `Task`.
+Parameters are as for `Task.tasks_as_dot`.
+
+*Method `BaseTask.dot_node_label(self)`*:
+The default DOT node label.
+
+*Method `BaseTask.tasks_as_dot(tasks, name=None, *, follow_blocking=False, sep=None)`*:
+Return a DOT syntax digraph of the iterable `tasks`.
+        Nodes will be coloured according to `DOT_NODE_FILLCOLOR_PALETTE`
+        based on their state.
+
+        Parameters:
+        * `tasks`: an iterable of `Task`s to populate the graph
+        * `name`: optional graph name
+        * `follow_blocking`: optional flag to follow each `Task`'s
+          `.blocking` attribute recursively and also render those
+          `Task`s
+        * `sep`: optional node seprator, default `'
+'`
+
+*Method `BaseTask.tasks_as_svg(tasks, name=None, **kw)`*:
+Return an SVG diagram of the iterable `tasks`.
+This takes the same parameters as `tasks_as_dot`.
+
+## Class `BlockedError(TaskError)`
 
 Raised by a blocked `Task` if attempted.
 
 ## Function `main(argv)`
 
 Dummy main programme to exercise something.
 
@@ -119,15 +144,15 @@
 queue the task and its prerequisites for execution.
 
 ## Function `make_now(*tasks, fail_fast=False, queue=None)`
 
 Run the generator `make(*tasks)` to completion and return the
 list of completed tasks.
 
-## Class `Task(BaseTask, cs.fsm.FSM, cs.gvutils.DOTNodeMixin, cs.resources.RunStateMixin, cs.threads.HasThreadState, cs.context.ContextManagerMixin)`
+## Class `Task(BaseTask, cs.threads.HasThreadState)`
 
 A task which may require the completion of other tasks.
 
 The model here may not be quite as expected; it is aimed at
 tasks which can be repaired and rerun.
 As such, if `self.run(func,...)` raises an exception from
 `func` then this `Task` will still block dependent `Task`s.
@@ -173,15 +198,120 @@
     t1.bg(time.sleep, 2)
     t2 = Task(name=\"task2\")
     # prevent t2 from running until t1 completes
     t2.require(t1)
     # try to run sleep(5) for t2 immediately after t1 completes
     t1.notify(t2.call, sleep, 5)
 
-## Class `TaskError(cs.fsm.FSMError, builtins.Exception, builtins.BaseException)`
+*Method `Task.__call__(self)`*:
+Block on `self.result` awaiting completion
+by calling `self.result()`.
+
+*Method `Task.bg(self)`*:
+Dispatch a function to complete the `Task` in a separate `Thread`,
+returning the `Thread`.
+This raises `BlockedError` for a blocked task.
+otherwise the thread runs `self.dispatch()`.
+
+*Method `Task.block(self, otask)`*:
+Block another task until we are complete.
+The converse of `.require()`.
+
+*Method `Task.blockers(self)`*:
+A generator yielding tasks from `self.required`
+which should block this task.
+Aborted tasks are not blockers
+but if we encounter one we do abort the current task.
+
+*Method `Task.cancel(self)`*:
+Transition this `Task` to `CANCELLED` state.
+If the task is running, set `.cancelled` on the `RunState`,
+allowing clean task cancellation and subsequent transition
+(mediated by the `.run()` method).
+Otherwise fire the `'cancel'` event directly.
+
+*Method `Task.dispatch(self)`*:
+Dispatch the `Task`:
+If the task is blocked, raise `BlockedError`.
+If a prerequisite is aborted, fire the 'abort' method.
+Otherwise fire the `'dispatch'` event and then run the
+task's function via the `.run()` method.
+
+*Method `Task.isblocked(self)`*:
+A task is blocked if any prerequisite is not complete.
+
+*Method `Task.iscompleted(self)`*:
+This task is completed (even if failed) and does not block contingent tasks.
+
+*Method `Task.join(self)`*:
+Wait for this task to complete.
+
+*Method `Task.make(self, fail_fast=False)`*:
+Complete `self` and its prerequisites.
+This calls the global `make()` function with `self`.
+It returns a Boolean indicating whether this task completed.
+
+*`Task.perthread_state`*
+
+*Method `Task.require(self, otask: 'TaskSubType')`*:
+Add a requirement that `otask` be complete before we proceed.
+This is the simple `Task` only version of `.then()`.
+
+*Method `Task.run(self)`*:
+Run the function associated with this task,
+completing the `self.result` `Result` appropriately when finished.
+
+*WARNING*: this _ignores_ the current state and any blocking `Task`s.
+You should usually use `dispatch` or `make`.
+
+During the run the thread local `Task.default()`
+will be `self` and the `self.runstate` will be running.
+
+Otherwise run `func_result=self.func(*self.func_args,**self.func_kwargs)`
+with the following effects:
+* if the function raises a `CancellationError`, cancel the `Task`
+* if the function raises another exception,
+  if `self.cancel_on_exception` then cancel the task
+  else complete `self.result` with the exception
+  and fire the `'error'` `event
+* if `self.runstate.canceled` or `self.cancel_on_result`
+  was provided and `self.cancel_on_result(func_result)` is
+  true, cancel the task
+* otherwise complete `self.result` with `func_result`
+  and fire the `'done'` event
+
+*Method `Task.then(self, func: Union[str, Callable, ForwardRef('TaskSubType')], *a, func_args=(), func_kwargs=None, **task_kw)`*:
+Prepare a new `Task` or function which may not run before `self` completes.
+This may be called in two ways:
+- `task.then(some_Task): block the `Task` instance `some_Task` behind `self`
+- `task.then([name,]func[,func_args=][,func_kwargs=][,Task_kwargs...]):
+  make a new `Task` to be blocked behind `self`
+Return the new `Task`.
+
+This supports preparing a chain of actions:
+
+    >>> t_root = Task(\"t_root\", lambda: 0)
+    >>> t_leaf = t_root.then(lambda: 1).then(lambda: 2)
+    >>> t_root.iscompleted()   # the root task has not yet run
+    False
+    >>> t_leaf.iscompleted()   # the final task has not yet run
+    False
+    >>> # t_leaf is blocked by t_root
+    >>> t_leaf.dispatch()      # doctest: +ELLIPSIS
+    Traceback (most recent call last):
+      ...
+    cs.taskqueue.BlockedError: ...
+    >>> t_leaf.make()          # make the leaf, but make t_root first
+    True
+    >>> t_root.iscompleted()   # implicitly completed by make
+    True
+    >>> t_leaf.iscompleted()
+    True
+
+## Class `TaskError(cs.fsm.FSMError)`
 
 Raised by `Task` related errors.
 
 ## Class `TaskQueue`
 
 A task queue for managing and running a set of related tasks.
 
@@ -218,18 +348,46 @@
      ...
      t1
      t2
 
 *Method `TaskQueue.__init__(self, *tasks, run_dependent_tasks=False)`*:
 Initialise the queue with the supplied `tasks`.
 
+*Method `TaskQueue.add(self, task)`*:
+Add a task to the tasks managed by this queue.
+
+*Method `TaskQueue.as_dot(self, name=None, **kw)`*:
+Compute a DOT syntax graph description of the tasks in the queue.
+
+*Method `TaskQueue.get(self)`*:
+Pull a completed or an unblocked pending task from the queue.
+Return the task or `None` if nothing is available.
+
+The returned task is no longer tracked by this queue.
+
+*Method `TaskQueue.run(self, runstate=None, once=False)`*:
+Process tasks in the queue until the queue has no completed tasks,
+yielding each task, immediately if `task.iscompleted()`
+otherwise after `taks.dispatch()`.
+
+An optional `RunState` may be provided to allow early termination
+via `runstate.cancel()`.
+
+An incomplete task is `dispatch`ed before `yield`;
+ideally it will be complete when the yield happens,
+but its semantics might mean it is in another state such as `CANCELLED`.
+The consumer of `run` must handle these situations.
+
 # Release Log
 
 
 
+*Release 20240423*:
+Small fixes.
+
 *Release 20230401*:
 Add missing requirement to DISTINFO.
 
 *Release 20230331*:
 * Task: subclass BaseTask instead of (FSM, RunStateMixin).
 * BaseTask.__init__: use @uses_runstate to ensure we've got a RunState.
 
@@ -243,13 +401,21 @@
 * BaseTask: new tasks_as_svg() method like tasks_as_dot() but returning SVG.
 
 *Release 20220805*:
 Initial PyPI release."""
 content-type = "text/markdown"
 
 [build-system]
+build-backend = "setuptools.build_meta"
 requires = [
     "setuptools >= 61.2",
     "trove-classifiers",
     "wheel",
 ]
-build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+py-modules = [
+    "cs.taskqueue",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

