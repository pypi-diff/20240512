# Comparing `tmp/reflex_wrapper-0.0.3.tar.gz` & `tmp/reflex_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_wrapper-0.0.3.tar", last modified: Thu May  9 01:11:42 2024, max compression
+gzip compressed data, was "reflex_wrapper-0.0.4.tar", last modified: Sun May 12 15:33:54 2024, max compression
```

## Comparing `reflex_wrapper-0.0.3.tar` & `reflex_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.3/LICENSE
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3914 2024-05-09 01:04:21.000000 reflex_wrapper-0.0.3/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.935625 reflex_wrapper-0.0.3/reflex_wrapper/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       37 2024-05-09 01:11:03.000000 reflex_wrapper-0.0.3/reflex_wrapper/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    13887 2024-05-09 01:10:16.000000 reflex_wrapper-0.0.3/reflex_wrapper/rx_wrapper.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-09 01:11:42.000000 reflex_wrapper-0.0.3/reflex_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-09 01:11:42.939625 reflex_wrapper-0.0.3/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-09 00:52:53.000000 reflex_wrapper-0.0.3/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-12 15:33:54.430205 reflex_wrapper-0.0.4/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-05-01 15:13:57.000000 reflex_wrapper-0.0.4/LICENSE
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-12 15:33:54.426205 reflex_wrapper-0.0.4/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3914 2024-05-09 01:04:21.000000 reflex_wrapper-0.0.4/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-12 15:33:54.426205 reflex_wrapper-0.0.4/reflex_wrapper/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       55 2024-05-12 12:43:50.000000 reflex_wrapper-0.0.4/reflex_wrapper/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    13248 2024-05-12 15:20:43.000000 reflex_wrapper-0.0.4/reflex_wrapper/rx_wrapper.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-05-12 15:33:54.426205 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     4462 2024-05-12 15:33:54.000000 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      271 2024-05-12 15:33:54.000000 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-05-12 15:33:54.000000 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       14 2024-05-12 15:33:54.000000 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       15 2024-05-12 15:33:54.000000 reflex_wrapper-0.0.4/reflex_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-05-12 15:33:54.430205 reflex_wrapper-0.0.4/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      788 2024-05-12 15:33:14.000000 reflex_wrapper-0.0.4/setup.py
```

### Comparing `reflex_wrapper-0.0.3/LICENSE` & `reflex_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_wrapper-0.0.3/PKG-INFO` & `reflex_wrapper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
 Home-page: https://github.com/B4PT0R/reflex_wrapper
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reflex_wrapper-0.0.3/README.md` & `reflex_wrapper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `reflex_wrapper-0.0.3/reflex_wrapper/rx_wrapper.py` & `reflex_wrapper-0.0.4/reflex_wrapper/rx_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """
 Module used as a wrapper around the reflex library to ease custom components creation.
 Defines a generic Component class that automates State init boilerplate and provides a more user-friendly interface to interact with components
 """
 
 import reflex
 from functools import wraps
+from types import FunctionType, CodeType
 from copy import copy
+from textwrap import dedent 
 import uuid
 
+def get_function(code_str, func_name):
+    """ Compiles a function from a code string. Returns the corresponding function object."""
+    code_str = dedent(code_str)
+    compiled_code = compile(code_str, "<string>", "exec")
+    func_code = next(obj for obj in compiled_code.co_consts if isinstance(obj, CodeType))
+    return FunctionType(func_code, globals(), func_name)
+
+
 def get_class_dict(cls,excluded=()):
     """
     Returns a dict representing a given class, excluding chosen attributes
     """
+    excluded_attributes = {'__dict__', '__weakref__', '__module__', '__qualname__','__annotations__',*excluded}
     class_dict = {
         '__name__': cls.__name__,
         '__bases__': tuple(base for base in cls.__bases__ if base != object),
-        '__metaclass__': type(cls),
-        '__annotations__':{k:v for k,v in cls.__annotations__.items() if not k in excluded}
+        '__annotations__':{k:v for k,v in cls.__annotations__.items() if not k in excluded},
+        **{k:v for k,v in cls.__dict__.items() if k not in excluded_attributes}
     }
-
-    excluded_attributes = {'__dict__', '__weakref__', '__module__', '__qualname__','__annotations__',*excluded}
-    class_dict.update({k:v for k,v in cls.__dict__.items() if k not in excluded_attributes})
     return class_dict
 
 def build_class(class_dict):
     """
     Reconstructs a class from a class_dict
     """
     class_dict=copy(class_dict)
     name = class_dict.pop('__name__')
     bases = class_dict.pop('__bases__')
-    metaclass = class_dict.pop('__metaclass__')
-    attributes=dict(**class_dict)
-    return metaclass(name, bases, attributes)
+    return type(name, bases, class_dict)
 
 def auto_render(obj):
     """
     Makes sure obj is or returns a reflex.Component instance
     """
     if callable(obj):
         @wraps(obj)
@@ -69,221 +75,197 @@
     }
     cls_name="State_"+str(uuid.uuid4())
     state=type(cls_name,(reflex.State,),attributes)
     state_var=state.value
     state_setter=state.set_value
     return state_var,state_setter
 
-class StateWrapper:
 
-    """
-    Class acting as a reflex.State proxy, allowing to pass reflex (computed) vars as default values for other state variables.
-    Meant to achieve staightforward state synchronization between components with a priori independent states.
-    """
-
-    def __init__(self,state):
-        self.state=state
-        self.dict=dict()
-
-    def __getattr__(self,attr):
-        if attr in self.dict:
-            return self.dict[attr]
-        else:
-            return getattr(self.state,attr)
-    
-    def __setattr__(self,attr,value):
-        if attr in ['state','dict']:
-            super().__setattr__(attr,value)
-        else:
-            if isinstance(value,reflex.Var):
-                self.dict[attr]=value
-            else:
-                setattr(self.state,attr,value)
+class State:
 
-    def __delattr__(self,attr):
-        if attr in ['state','dict']:
-            super().__delattr__(attr)
-        else:
-            if attr in self.dict:
-                del self.dict[attr]
-            else:
-                delattr(self.state,attr)
-
-
-
-class Component:
-
-    _excluded=(
-        '_excluded',
+    _private=(
+        '_private',
         '_state_model',
         '_state_attrs',
-        '_constructor',
-        '_create',
         '_setup_state_class',
         '_get_instance_state_class',
-        'get_component',
+        '_state',
         '_set_default',
-        '_set_defaults_from_props',
-        '_initialize',
         '__init__',
-        '__getattr__',
+        '__getattribute__',
         '__setattr__',
-        '_render',
         '_is_state_attr',
+        '_is_user_state_attr',
         '_is_state_variable',
         '_is_state_setter',
-        '__doc__'
+        '__doc__',
+        '__class__'
     )
-    
+
     _state_model=None
     _state_attrs=None
-    _constructor=None
     
     @classmethod
     def _setup_state_model(cls):
         """
-        Extract user defined attributes and methods from the Component subclass to construct the Pydantic state model (reflex.Base)
+        Extract user defined attributes and methods from the State subclass to construct the Pydantic state model (reflex.Base)
         """
-        details=get_class_dict(cls,excluded=cls._excluded)
+        details=get_class_dict(cls,excluded=cls._private)
         name=details['__name__']
-        cls._state_attrs=[k for k in details if k not in ('__name__','__bases__','__metaclass__','__annotations__')]
-        details.update(__name__=name+'State',__bases__=(reflex.Base,),_instance_count=0)
+        cls._state_attrs={k:v for k,v in details.items() if not k in ('__name__','__bases__','__annotations__')}
+        details.update(__name__=name+'Model',__bases__=(reflex.Base,),_instance_count=0,_state_name=name)
         cls._state_model=build_class(details)
-        # Remove state attrs from the component object to avoid messing with __getattr__
         for attr in cls._state_attrs:
             delattr(cls,attr)
    
     @classmethod 
     def _get_instance_state_class(cls):
         """
-        Copy the state model into a reflex.State subclass, unique for each component instance.
+        Copy the state model into a reflex.State subclass, unique for each State instance.
         """
         if cls._state_model is None:
             cls._setup_state_model()
         cls._state_model._instance_count += 1
-        instance_state_cls_name = f"{cls._state_model.__name__}_n{cls._state_model._instance_count}"
-        instance_state_class = type(instance_state_cls_name, (cls._state_model, reflex.State), {})
+        instance_state_cls_name = f"{cls._state_model._state_name}_n{cls._state_model._instance_count}"
+        instance_state_class = type(instance_state_cls_name, (cls._state_model, reflex.State),{})
         return instance_state_class
     
-    def _is_state_attr(self,attr):
+    def _is_user_state_attr(self,attr):
         """
         Checks whether an attr is a user-defined state attr
         """
-        if self.state is None:
+        if not hasattr(self,'_state') or self._state is None:
             return False
         else:
             return attr in self.__class__._state_attrs
         
     def _is_state_variable(self,attr):
         """
         Checks whether an attr is a state variable
         """
-        return self._is_state_attr(attr) and attr in self.state.__fields__
+        return self._is_user_state_attr(attr) and attr in self._state.__fields__
     
     def _is_state_setter(self,attr):
         """
-        Checks whether an attr is a state variable setter
+        Checks whether an attr is a state setter
         """
         return attr.startswith('set_') and self._is_state_variable(attr[4:])
     
-    def _is_state(self,attr):
+    def _is_state_attr(self,attr):
         """
-        Check whether an attr is a valid state attr
+        Checks whether an attr is a valid state attribute
         """
-        return self._is_state_attr(attr) or self._is_state_setter(attr)
+        return self._is_user_state_attr(attr) or self._is_state_setter(attr)
     
     def _set_default(self,key,value):
         """
         Sets the default value of a state variable
         """
-        self.state.__fields__[key].default=value
+        if self._is_state_variable(key):
+            self._state.__fields__[key].default=value
+        else:
+            raise AttributeError(f"Could not assign state variable value. Invalid state variable: {key}")
+    
+    def __init__(self):
+        self._state=self.__class__._get_instance_state_class()
 
-    def _set_defaults_from_props(self):
-        """
-        Sets defaults for state variables from props passed to the component
-        Skip if the prop already refers to another state variable (possibly from another component) 
+    def __getattr__(self,key):
         """
-        for key,value in self.props.items():
-            if self._is_state_variable(key):
-                if isinstance(value,(reflex.Var,reflex.vars.ComputedVar)):
-                    setattr(self.state,key,value)
-                else:
-                    self._set_default(key,value)
-                    
-    def _get_reflex_props(self):
+        Delegate attribute access to the reflex.State object
+        """    
+        if self._is_state_attr(key):
+            return getattr(self._state,key)
+        else:
+            raise AttributeError(f"Invalid state attribute: '{key}'")
+        
+    def __setattr__(self,key,value):
         """
-        filters out state variables from props before passing them to the reflex constructor
+        Delegate attribute setting to to the reflex.State object
         """
-        return {k:v for k,v in self.props.items() if not self._is_state(k)}
+        if key in self.__class__._private:
+            object.__setattr__(self,key,value)
+        elif self._is_state_variable(key):
+            self._set_default(key,value)
+        elif self._is_state_attr(key):
+            raise AttributeError(f"Cannot assign to a state attribute which is not a state variable: '{key}'.")
+        else:
+            raise AttributeError(f"Invalid state attribute: '{key}'")
+        
+
+class Component(State):
+
+    _private=State._private+(
+        '_init_constructor',
+        '_constructor',
+        '_attach_state',
+        'props',
+        'get_component',
+        '_render'
+    )
+
+    _constructor=None
     
     def get_component(self,*childen,**props):
         """
         This method should be overriden when defining a custom component class
         """
         raise NotImplementedError("Custom components must implement a get_component method.")
-
-    def _create(self,*children,**props):
+    
+    def _attach_state(self,func):
         """
-        Returns the corresponding reflex.Component instance and attach the state to it
+        Decorator: takes a function returning a reflex.Component instance and attach the state to the returned component
         """
-        component=auto_render(self.get_component)(*children,**props)
-        #component.State=self.state
-        return component
-    
-    def _initialize(self):
+        @wraps(func)
+        def decorated(*args,**kwargs):
+            component=func(*args,**kwargs)
+            component.State=self._state
+            return component
+        return decorated
+
+    def _init_constructor(self):
         """
-        Initializes the reflex.Component constructor:
-        If none is specified at class level, this is a custom component so we initialize its state and constructor accordingly
+        The reflex.Component constructor:
+        If none is specified at class level, this is a custom component so we return the decorated custom get_component method
         If one is already specified at class level, this is a default component, so we use its constructor directly.
         """
         if self.__class__._constructor is None:
-            self.state=StateWrapper(self.__class__._get_instance_state_class())
-            self.constructor=self._create
+            self._constructor=self._attach_state(auto_render(self.get_component))
         else:
-            self.constructor=self.__class__._constructor
+            self._constructor=self.__class__._constructor
 
     def __init__(self,*children,**props):
-        self.parent=None
-        self.state=None
-        self.constructor=None
-        self._initialize()
+        State.__init__(self)
+        self._init_constructor()
         self.props = dict(**props)
         # the 'children' prop, if any, gets precedence over children passed as nested args (similar to React)
         children=self.props.get('children') or children
-        for child in children:
-            if isinstance(child,Component):
-                child.parent=self
         self.props['children']=children
-        self._set_defaults_from_props()
 
     def __getattr__(self,key):
         """
-        Delegate attribute access to state / props
+        Delegate attribute access to the reflex.State object
         """
-        if self._is_state(key):
-            return getattr(self.state,key)
+        if self._is_state_attr(key):
+            return getattr(self._state,key)
         elif key in self.props:
             return self.props[key]
         else:
-            raise AttributeError(f"Invalid attribute key: '{key}'")
+            raise AttributeError(f"Invalid component attribute: '{key}'")
         
     def __setattr__(self,key,value):
         """
-        Delegate attribute setting to state / props
+        Delegate attribute setting to to the reflex.State object or props
         """
-        if key in ['parent','constructor','component','state','props']:
-            super().__setattr__(key,value)
+        if key in self.__class__._private:
+            object.__setattr__(self,key,value)
         elif self._is_state_variable(key):
-            if not isinstance(value,(reflex.Var,reflex.vars.ComputedVar)):
-                self._set_default(key,value)
-            else:
-                setattr(self.state,key,value)
+            self._set_default(key,value)
             self.props[key]=value
-        elif self._is_state_setter(key) or self._is_state_attr(key):
-            raise AttributeError("Cannot override a state method.")
+        elif self._is_state_attr(key):
+            raise AttributeError(f"Cannot assign to a component attribute which is not a prop or state variable: '{key}'.")
         else:
             self.props[key]=value
 
     def _render(self):
         """
         Renders the component
         ie. returns the corresponding reflex.Component instance
@@ -294,23 +276,22 @@
         for child in self.props['children']:
             if isinstance(child,Component):
                 child=child._render()
             rendered_children.append(child)
 
         # Then render the props
         props={}
-        for key,prop in self._get_reflex_props().items():
+        for key,prop in self.props.items():
             if not key=='children':
                 if isinstance(prop,Component):
                     prop=prop._render()
                 props[key]=prop
         
         # Render the component by calling the constructor
-        self.component=self.constructor(*rendered_children,**props)
-        return self.component
+        return self._constructor(*rendered_children,**props)
 
 
 def get_builtin_component(name=None,constructor=None):
     """
     Prepares a component class from a given builtin reflex constructor
     """
     return type(name,(Component,),dict(_constructor=constructor))
@@ -408,15 +389,15 @@
 
 
 class rx(metaclass=rx_meta):
     """
     Class used as a replacement of the reflex module, supporting Components objects
     (its __getattr__ is implemented by the metaclass defined above)
     """
-    _reserved=['page','var','cached_var','Base','State','theme','theme_panel','Var','Config']
+    _reserved=['page','var','cached_var','Base','theme','theme_panel','Var','Config']
     _dict=dict()
```

### Comparing `reflex_wrapper-0.0.3/reflex_wrapper.egg-info/PKG-INFO` & `reflex_wrapper-0.0.4/reflex_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A custom wrapper on top of the reflex library to ease creating and interacting with custom components.
 Home-page: https://github.com/B4PT0R/reflex_wrapper
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

