# Cpython Internals![image title](http://www.zpoint.xyz:8080/count/tag.svg?url=github%2FCPython-Internals)

![cpython logo](https://docs.google.com/drawings/d/e/2PACX-1vQKKPvv9xI22zZcRtElIMx_-G22qYcLUvl-gbngubjf76dr80ZjsYQZCCKVqEvJnmBnwZyDXqG9GPlu/pub?w=300&h=200) 

* [简体中文](README_CN.md)
* [한국어](README_KR.md)
*  **Watch** this repo if you need to be notified when there's update

This repository is my notes/blog for [cpython](https://github.com/python/cpython) source code

Trying to illustrate every detail of cpython implementation

```shell script
# based on version 3.8.0a0
cd cpython
git reset --hard ab54b9a130c88f708077c2ef6c4963b632c132b3
```

The following contents are suitable for those who have python programming experience and interested in internal of python interpreter, for those who needs beginner or advanced material please refer to [awesome-python-books](https://github.com/Junnplus/awesome-python-books)

# Table of Contents

* [Objects](#Objects)
* [Modules](#Modules)
* [Lib](#Lib)
* [Interpreter](#Interpreter)
* [Extension](#Extension)
* [Learning material](#Learning-material)
* [Contribution](#Contribution)
* [License](#License)


# Objects
 - [x] [dict](BasicObject/dict/dict.md)
 - [x] [long/int](BasicObject/long/long.md)
 - [x] [unicode/str](BasicObject/str/str.md)
 - [x] [set](BasicObject/set/set.md)
 - [x] [list(timsort)](BasicObject/list/list.md)
 - [x] [tuple](BasicObject/tuple/tuple.md)
 - [x] [bytes](BasicObject/bytes/bytes.md)
 - [x] [bytearray(buffer protocol)](BasicObject/bytearray/bytearray.md)
 - [x] [float](BasicObject/float/float.md)
 - [x] [func(user-defined method)](BasicObject/func/func.md)
 - [x] [method(builtin method)](BasicObject/method/method.md)
 - [x] [iter](BasicObject/iter/iter.md)
 - [x] [gen(generator/coroutine/async generator)](BasicObject/gen/gen.md)
 - [x] [class(bound method/classmethod/staticmethod)](BasicObject/class/class.md)
 - [x] [complex](BasicObject/complex/complex.md)
 - [x] [enum](BasicObject/enum/enum.md)
 - [x] [type(mro/metaclass/creation of class/instance)](BasicObject/type/type.md)

# Modules

 - [ ] io
 	- [x] [fileio](Modules/io/fileio/fileio.md)
 - [x] [pickle](Modules/pickle/pickle.md)

# Lib

 - [x] [re(regex)](Modules/re/re.md)
 - [ ] asyncio

# Interpreter

 - [x] [gil(Global Interpreter Lock)](Interpreter/gil/gil.md)
 - [x] [gc(Garbage Collection)](Interpreter/gc/gc.md)
 - [x] [memory management](Interpreter/memory_management/memory_management.md)
 - [x] [descr(how does attribute access work/`__get__`/`__getattribute__`/`__getattr__`)](Interpreter/descr/descr.md)
 - [x] [exception(exception handling)](Interpreter/exception/exception.md)
 - [x] [module(how does import work)](Interpreter/module/module.md)
 - [x] [frame](Interpreter/frame/frame.md)
 - [x] [code](Interpreter/code/code.md)
 - [x] [slots/`__slots__`(how does attribute initialized in the creation of class/instance)](Interpreter/slot/slot.md)
 - [x] [thread](Interpreter/thread/thread.md)
 - [x] [PyObject(overview)](Interpreter/pyobject/pyobject.md)

# Extension

 - [x] [C API(profile python code and write pure C extension)](Extension/C/c.md)
 - [ ] Cython(C extension)
 - [x] [Boost C++ libaries (C\+\+ extension)](https://github.com/zpoint/Boost-Python-Examples)
 - [ ] [C++ extension](Extension/CPP/cpp.md)
 	- [x] integrate with NumPy
 	- [x] bypass the GIL

# Grammar

 - [x] [Compile Phase](Interpreter/compile/compile.md)
    - [x] [Grammar/MetaGrammar to DFA](Interpreter/compile/compile.md)
    - [x] [CST to AST](Interpreter/compile2/compile.md)
    - [x] [AST to python byte code](Interpreter/compile3/compile.md)


# Learning material

I will only recommend what I've read

* [CPython internals - Interpreter and source code overview(youtube video)](https://www.youtube.com/watch?v=LhadeL7_EIU&list=PLzV58Zm8FuBL6OAv1Yu6AwXZrnsFbbR0S)
* [< < Inside The Python Virtual Machine > >](https://leanpub.com/insidethepythonvirtualmachine)
* [< < Python 源码剖析 > >](https://book.douban.com/subject/3117898/)
* [rushter(blog/eng)](https://rushter.com/)
* [YET ANOTHER PYTHON INTERNALS BLOG(blog/eng)](https://pythoninternal.wordpress.com/)
* [Junnplus(blog/cn)](https://github.com/Junnplus/blog/issues)
* [manjusaka(blog/cn)](https://manjusaka.itscoder.com/)
* [aoik-Python's compiler series(blog/eng)](https://aoik.me/blog/posts/python-compiler-from-grammar-to-dfa)

# Contribution

All kinds of contributions are welcome

* submit a pull request
  *  if you want to share any knowledge you know
  * post a new article
  * correct any technical mistakes
  * correct english grammar
  * translation
  * anything else
* open an issue 
  * any suggestions
  * any questions
  * correct mistakes
  * anything else

# [License](https://creativecommons.org/licenses/by-nc-sa/4.0/)
