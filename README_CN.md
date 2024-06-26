# Cpython Internals![image title](http://www.zpoint.xyz:8080/count/tag.svg?url=github%2FCPython-Internals-CN)

* [English](README.md)
* [한국어](README_KR.md)
* 如果你需要接收更新通知, 点击右上角的 **Watch**, 当有文章更新时会在 issue 发布相关标题和链接
* 如果有任何链接无法打开请自行搭梯子 O(∩_∩)O

这个仓库是笔者分析 [cpython](https://github.com/python/cpython) 源码的时候做的记录/博客

笔者将尝试尽可能的讲清楚 cpython 底层实现的细节

```shell script
# 基于 3.8.0a0 版本
cd cpython
git reset --hard ab54b9a130c88f708077c2ef6c4963b632c132b3

```

这里的内容适用于有过 python 编程经验并且对解释器的实现感兴趣的同学, 如果你需要的的是入门到进阶之类的学习资料, 请参考 [awesome-python-books](https://github.com/Junnplus/awesome-python-books/blob/master/README-ZH_CN.md)


# 目录

* [基本对象](#基本对象)
* [模块](#模块)
* [库](#库)
* [解释器相关](#解释器相关)
* [扩展](#扩展)
* [学习资料](#学习资料)
* [参与贡献](#参与贡献)

* [授权](#授权)


# 基本对象
- [x] [dict](BasicObject/dict/dict_cn.md)
- [x] [long/int](BasicObject/long/long_cn.md)
- [x] [unicode/str](BasicObject/str/str_cn.md)
- [x] [set](BasicObject/set/set_cn.md)
- [x] [list(timsort)](BasicObject/list/list_cn.md)
- [x] [tuple](BasicObject/tuple/tuple_cn.md)
- [x] [bytes](BasicObject/bytes/bytes_cn.md)
- [x] [bytearray(buffer protocol)](BasicObject/bytearray/bytearray_cn.md)
- [x] [float](BasicObject/float/float_cn.md)
- [x] [func(user-defined method)](BasicObject/func/func_cn.md)
- [x] [method(builtin method)](BasicObject/method/method_cn.md)
- [x] [iter](BasicObject/iter/iter_cn.md)
- [x] [gen(generator/coroutine/async generator)](BasicObject/gen/gen_cn.md)
- [x] [class(bound method/classmethod/staticmethod)](BasicObject/class/class_cn.md)
- [x] [complex](BasicObject/complex/complex_cn.md)
- [x] [enum](BasicObject/enum/enum_cn.md)
- [x] [type(mro/metaclass/类/实例的创建过程)](BasicObject/type/type_cn.md)

# 模块

 - [ ] io
 	- [x] [fileio](Modules/io/fileio/fileio_cn.md)
 - [x] [pickle](Modules/pickle/pickle_cn.md)

# 库

 - [x] [re(正则)](Modules/re/re_cn.md)
 - [ ] asyncio

# 解释器相关

 - [x] [gil(全局解释器锁)](Interpreter/gil/gil_cn.md)
 - [x] [gc(垃圾回收机制)](Interpreter/gc/gc_cn.md)
 - [x] [memory management(内存管理机制)](Interpreter/memory_management/memory_management_cn.md)
 - [x] [descr(访问(类/实例)属性时发生了什么/`__get__`/`__getattribute__`/`__getattr__`)](Interpreter/descr/descr_cn.md)
 - [x] [exception(异常处理机制)](Interpreter/exception/exception_cn.md)
 - [x] [module(import 实现机制)](Interpreter/module/module_cn.md)
 - [x] [frame](Interpreter/frame/frame_cn.md)
 - [x] [code](Interpreter/code/code_cn.md)
 - [x] [slots/`__slots__`(属性在类/实例创建时是如何初始化的)](Interpreter/slot/slot_cn.md)
 - [x] [thread(线程)](Interpreter/thread/thread_cn.md)
 - [x] [PyObject(基础篇/概述)](Interpreter/pyobject/pyobject_cn.md)

# 扩展

 - [x] [C API(python 性能分析和 C 扩展)](Extension/C/c_cn.md)
 - [ ] Cython(C extension)
 - [x] [Boost C++ libaries (C\+\+ extension)](https://github.com/zpoint/Boost-Python-Examples)
 - [x] [C++ 扩展](Extension/CPP/cpp_cn.md)
 	- [x] 写 NumPy 扩展
 	- [x] 绕过 GIL

# 语法

[编译阶段](Interpreter/compile/compile.md)

* [x] [从语法/元语法到 DFA](Interpreter/compile/compile_cn.md)
* [x] [从 CST 到 AST](Interpreter/compile2/compile_cn.md)
* [x] [从 AST 到 字节码](Interpreter/compile3/compile_cn.md)


# 学习资料

以下的资料笔者遵循先阅读后推荐的原则

* [CPython internals - Interpreter and source code overview(油管视频)](https://www.youtube.com/watch?v=LhadeL7_EIU&list=PLzV58Zm8FuBL6OAv1Yu6AwXZrnsFbbR0S)
* [< < Inside The Python Virtual Machine > >](https://leanpub.com/insidethepythonvirtualmachine)
* [< < Python 源码剖析 > >](https://book.douban.com/subject/3117898/)
* [rushter(blog/eng)](https://rushter.com/)
* [YET ANOTHER PYTHON INTERNALS BLOG(blog/eng)](https://pythoninternal.wordpress.com/)
* [Junnplus(blog/中文)](https://github.com/Junnplus/blog/issues)
* [manjusaka(blog/中文)](https://manjusaka.itscoder.com/)
* [aoik-Python's compiler series(blog/eng)](https://aoik.me/blog/posts/python-compiler-from-grammar-to-dfa)

## 参与贡献

欢迎所有形式的贡献

* 提交一个 pull request
  * 如果你想分享任何你知道的相关知识
  *  发布一篇文章
  * 更正技术性错误
  * 更正语法性错误
  * 翻译
  * 其他情况, 不限于上述
* 提交一个 issue 
  * 任何建议
  * 任何问题
  * 更正错误
  * 其他情况, 不限于上述

# [授权](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)

