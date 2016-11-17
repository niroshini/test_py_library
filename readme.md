# test_py_library (Python)
=========================================
This is an example of how to create a python library. Also see https://python-packaging.readthedocs.io/en/latest/minimal.html

## Naming conventions
The Python library/package names should generally follow the following constraints:

- All lowercase
- Unique on pypi, even if you don’t want to make your package publicly available (you might want to specify it privately as a dependency later)
- Underscore-separated or no word separators at all (don’t use hyphens)


## Directory structure 
```
test_py_library
│   readme.md
│   setup.py    
│
└───test_py_library
     __init__.py
     myclass.py
   
   
  

```

## Local installation
- First download the source code of the library to your local drive (eg: test_py_library)
- Open Terminal, & go inside the downloaded library source code (eg: inside test_py_library) & type `pip install .` . This will install the downloaded source.
- If you make changes to the libary code, you can upgrade the installation by 
`pip install . --upgrade`
- You can now use this library in your local modules by calling `import <library_name>`
- Example:

`10-149-75-153:test_py_library Niroshinie$ pip install .`

`10-149-75-153:test_py_library Niroshinie$ python`

`Python 2.7.12 |Anaconda custom (x86_64)| (default, Jul  2 2016, 17:43:17)` 
`[GCC 4.2.1 (Based on Apple Inc. build 5658) (LLVM build 2336.11.00)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
Anaconda is brought to you by Continuum Analytics.
Please check out: http://continuum.io/thanks and https://anaconda.org`


`>>> import test_py_library`

`>>> print test_py_library.joke()`

`Try and try and one day you will die`

`>>> from test_py_library import Myclass`

`>>> xx = Myclass()`

`>>> xx.mymethod()`

`Test Method`

`>>> `
