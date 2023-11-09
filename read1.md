### █✔█1584897049575632897(多选)  
**rightAnswer: ['AB']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 目录中存在如下两个文件：
`a/a.py`:
```python
NAME = 'a'


def func():
    return NAME
```
`main.py`:
```python
_______________________  # 需在此填入代码
a.func()
```
在`main.py`中，以下哪些选项中的代码单独填到横线处时可以正确运行（）

**参考文档：**

>`importlib.import_module(name, package=None)`
Import a module. The `name` argument specifies what module to import in absolute or relative terms (e.g. either `pkg.mod` or `..mod`).

>The `import_module()` function acts as a simplifying wrapper around `importlib.__import__()`. This means all semantics of the function are derived from `importlib.__import__()`. The most important difference between these two functions is that `import_module()` returns the specified package or module (e.g. `pkg.mod`), while `__import__()` returns the top-level package or module (e.g. `pkg`).  
  
```python
import importlib
a = importlib.import_module("a")
```### █✔█3817393(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 以下含有多行的代码，可以正常执行的有（ ）  
  
```PYTHON
s = 'a' + 'b' \
    + 'c' + 'd' \
    + 'e' + 'f' \

# 其他代码
```### █✔█3735004(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['', 'ABD']**  
  
### `str`类型的`join`方法用于将序列中的元素以指定的字符连接生成一个新的字符串，以下选项中合法的有 ( )  
  
`''.join(['1', '2', '3'])`### █✔█3717098(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['', 'BCD']**  
  
### 以下哪些选项的代码单独填入横线处，运行输出结果是`['x', 'y', 'z']`（ ）
```python
import copy


a = [1, 2, ['x', 'y']]
b = a
c = copy.copy(a)
d = copy.deepcopy(a)
a[2].append('z')
___________  # 需填入代码
```  
  
`print(d[2])`### █✔█1584894952859840514(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['']**  
  
### 关于可测试性，如下描述正确的有（）  
  
只有可测试性非常好才能开展DT测试，否则DT测试无法开展### █✔█1584897049902788609(多选)  
**rightAnswer: ['ABCD']**  
**wrongAnswer: ['', 'ABD']**  
  
###  
```python
class A:
    x = 0


__________  # 需填入代码
print(a.x, b.x)
```
以下哪些选项中的代码独立填入到横线处时，可以使得以上代码运行时输出`1 1`？（ ）  
  
```python
a = A()
b = A()
A.x = 1
```### █✔█1584897050137669634(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 如下关于`cProfile`输出信息, 哪些函数及其所有子函数（从调用到退出）消耗的累积时间大于0.01秒（）
```shell
         10104 function calls in 3.888 seconds

   Ordered by: standard name

   ncalls  tottime  percall  cumtime  percall filename:lineno(function)
        1    0.000    0.000    0.000    0.000 cProfile.py:133(__exit__)
        1    0.003    0.003    3.888    3.888 test_cprofile3.py:15(foo_2)
      100    0.018    0.000    3.885    0.039 test_cprofile3.py:20(foo_3)
    10000    3.866    0.000    3.866    0.000 test_cprofile3.py:25(foo_4)
        1    0.000    0.000    0.000    0.000 test_cprofile3.py:9(foo_1)
        1    0.000    0.000    0.000    0.000 {method 'disable' of '_lsprof.Profiler' objects}
```  
  
`foo_4`### █✔█3934720(多选)  
**rightAnswer: ['AD']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 已有`letters`变量：
```python
letters = ['a', 'b']
```
以下哪些选项的代码的执行结果为`ababab`（）  
  
```python
print("".join(letters * 3))
```### █✔█3734852(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['']**  
  
### 下面哪些对集合`x`的操作，可以删除元素`2`：
```python
x = {1, 2, 3, 4, 5}
```
**参考：`set`的相关方法说明：**
> `remove(elem)`
> Remove element `elem` from the set. Raises `KeyError` if `elem` is not contained in the set.

> `discard(elem)`
> Remove element `elem` from the set if it is present.

> `pop()`
> Remove and return an arbitrary element from the set. Raises `KeyError` if the set is empty.  
  
```python
x.remove(2)
```### █✔█3621530(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['', 'BCD']**  
  
### 下列关于产品发布代码中公网地址的使用，下列代码片段中不符合《华为Python语言编程规范》中“代码工程”章节的原则和建议的有（）  
  
```python
test_site = load_site_from_file() # test_site来自配置文件，并在产品资料中进行了说明，支持客户自行修改
http.client.HTTPConnection()  
```### █✔█3667093(多选)  
**rightAnswer: ['AB']**  
**wrongAnswer: ['', 'ACD']**  
  
### 下面代码打印`math`模块中`pi`，正确的有（）  
  
```python
import pi


print(pi)
```### █✔█1584897049831485441(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['']**  
  
### data1是程序内部数据，data2是来自外部输入的数据，下列代码片段中，不符合《华为Python语言编程规范》中“序列化”章节的要求和建议的是（）  
  
`shelve.load(data2)`### █✔█3817364(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['']**  
  
###  
```python
if ________:  # 横线处需填入代码
    print("True")
```
以下哪些代码填入到横线处，可使得上面的代码打印出`True`？（ ）  
  
```python
123
```### █✔█3717455(多选)  
**rightAnswer: ['ABCD']**  
**wrongAnswer: ['']**  
  
### 如下多个`format`相关代码，哪些选项的代码可以输出结果`foo bar`字符串（）  
  
```python
sample_set = ('foo', 'bar')
print('{0} {1}'.format(*sample_set))
```### █✔█3621456(多选)  
**rightAnswer: ['AC']**  
**wrongAnswer: ['']**  
  
### 以下选项符合《华为Python语言编程规范》中“文件”章节的要求和建议的有( )  
  
`path = os.getcwd() + '/' + myDirectory'`### █✔█1657955169085710338(多选)  
**rightAnswer: ['AC']**  
**wrongAnswer: ['ABC']**  
  
### 在当前工作目录下，有如下几个文件：
`test1.py`:
```python
from tests import test


test()
```

`tests/__init__.py`:
```python
_______  # 填写代码处 
```

`tests/testmodule.py`:
```python
def test():
    print("hello")
```
以下哪些选项的代码单独填入`__init__.py`中的横线处，运行`test1.py`可以输出 `hello`( )  
  
不填任何代码### █✔█3735003(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['AB', 'BCD']**  
  
### 下列反序列化代码中，符合《华为Python语言编程规范》的有：  
  
```python
import json
with open(file_name) as fd:  # 文件来自用户上传
    json.load(fd)
```### █✔█3963491(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: []**  
  
### 以下代码，哪些可正常执行():  
  
```print("abc\"ab")```### █✔█3862589(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABC']**  
  
### 下面哪些对集合x的操作，可以删除元素2：
```python
x = {1, 2, 3}
```  
  
```python
x ^= {2}
```### █✔█3735283(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['ABCD']**  
  
### 如下删除文件的操作中，哪些选项的代码符合《华为Python语言编程规范》中“代码工程”章节的原则、要求和建议（ ）  
  
`os.remove('filename.txt')`### █✔█3887741(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['ABCD']**  
  
### 不考虑编程规范，以下if语句的写法可以正确执行的有（）  
  
```python
if True:
print("OK")
```### █✔█1584894952864034817(多选)  
**rightAnswer: ['ABCD']**  
**wrongAnswer: []**  
  
### 关于可测试性，如下描述正确的有（）  
  
可定位性指输出信息支撑问题分析定位的能力。### █✔█3734855(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 下面的表达式运行时，不会产生异常的有（）  
  
```s1 = "%s" % "English"```### █✔█1584897050536128513(多选)  
**rightAnswer: ['AD']**  
**wrongAnswer: ['ABD', 'ABCD']**  
  
### 当无法确认目标文件的编码类型时，下列做法符合《华为Python语言编程规范》“文件”章节中的原则、要求与建议的有（）  
  
```python
import chardet


def try_print_unknown_encoding_file(file_path: str, mode: str):
    with open(file_path, 'rb') as f:
        enc = chardet.detect(f.read())["encoding"]
    try:
        with open(file_path, mode, encoding=enc) as f:
            for line in f:
                print(line)
    except UnicodeDecodeError:
        print("unknown file encoding")
```### █✔█1584897049542078465(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['ABCD']**  
  
### 以下哪些选项的代码输出结果为`True`（ ）  
  
```python
a = [1, 2, [3]]
b = a.copy()
a[2].append(4)
print(a == b)
```### █✔█1584900965881163777(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 每一种UML建模图都对应有各自不同的核心建模元素，其中顺序图（Sequence Diagram）的关键建模元素有哪些（  ）  
  
消息（Message）### █✔█1584894954608865281(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 小A对一个已有测试用例的模块代码进行重构，在重构代码的过程中，发现原有功能的一个BUG，为了方便，未提交已重构部分代码，直接顺手修改BUG，在保证已有测试用例都通过的前提下，一次性提交上库。后续对此BUG进行测试时发现修改方案并不完善，仍有问题，于是小A回退了所有重构和修改BUG部分的代码。请问在小A的重构过程中存在哪些问题（）  
  
重构没有小步提交### █✔█1584894952679485442(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如果输入条件规定了整型参数的范围及默认值，只用边界值分析方法，如下哪些可以作为测试数据（）  
  
默认值### █✔█3734850(多选)  
**rightAnswer: ['AD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
###  
```python
class B():
    def __init__(self):
        print('B')


class A(B):
    def __init__(self):
        ____________ # 需填入代码


a = A()
```
以下哪些选项中的代码单独填入到横线处，可以使得以上代码段输出`B`？（ ）  
  
`B.__init__(self)`### █✔█3717452(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['BC', 'ABCD']**  
  
### 已知：` x = [4, 1, 0, 3, 5]`， 下面哪些表达式操作可以将 `x`转变为` [4, 1, 3, 5]`（）  
  
`x[2:3] = []`### █✔█3717104(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如下表达式的值为`False`的有()  
  
`{3, 5, 6} > {4, 3, 5}`### █✔█3667106(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 以下哪些变量定义语句执行时会产生异常？（ ）  
  
`a = 10 20`### █✔█3667098(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 下列哪些选项符合《华为Python语言编程规范》中“类与面向对象”章节的原则、要求和建议（）  
  
```python
from abc import ABC, abstractmethod


# Base可能有多个不同实现的派生类
class Base(ABC):
    def __init__(self, base):
        self._base = base

    @abstractmethod
    def cal(self, a, b):
        pass


class Addition(Base):
    def cal(self, a, b):
        return a + b
```### █✔█3666975(多选)  
**rightAnswer: ['BC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如下代码中的命名，符合华为Python编程规范建议的有（ ）  
  
```python
def i(l, o):
    pass
```### █✔█3621579(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 下述哪些选项的说法符合《华为Python语言编程规范》中“变量作用域”章节的原则、要求和建议（）
```python
__all__ = []

_g_type = 1


def get_type():
    global _g_type
    return _g_type


def set_type(type):
    _g_type = type
```  
  
全局变量`_g_type`的命名违反规范，模块内使用的全局变量不能以下划线开头### █✔█3621560(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 在linux环境中，为了能够`import`在`/my_path`路径下的包(package)，以下做法不符合《华为Python语言编程规范》中“标准库”章节的要求和建议的有（）  
  
在代码中添加`sys.path.insert(0, '/my_path')`### █✔█3621464(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 以下哪些选项符合《华为Python语言编程规范》中“异常处理”章节的要求和建议（）  
  
```python
try:
    with open(file_name) as fd:
        content = fd.read()
except FileNotFoundError as e:
    do_something(file_name, e)
except UnicodeDecodeError as e:
    do_otherthing(file_name, e)
```### █✔█3211135(多选)  
**rightAnswer: ['BC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 下面哪些行为是华为开源软件使用规范明确禁止的？  
  
开源代码和自研代码目录隔离### █✔█1584900964601901058(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 安全应用的“linux安全设计”原则中，下述描述正确的有（）  
  
只给用户分配足够其完成任务的最小权限### █✔█2928344(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['ABCD']**  
  
### 针对重构方法，下列说法错误的有（）  
  
将值域上移到父类（即字段上移 Pull Up Field）会有效减少子类的成员变量，只需要搬移值域，不需要搬移对该值域的操作方法### █✔█3667050(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['ABCD']**  
  
### python会从下面哪些地方搜索模块(module)：  
  
python标准库路径### █✔█1584897050129281026(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: []**  
  
### 想要通过`cProfile`对`foo`函数进行运行耗时分析，以下哪些实现方式可以达成目标

**文档：**
> `cProfile.run(command, filename=None, sort=-1)`
This function takes a single argument that can be passed to the `exec()` function, and an optional file name.
In all cases this routine executes:
`exec(command, __main__.__dict__, __main__.__dict__)`
and gathers profiling statistics from the execution. 

> `class cProfile.Profile(timer=None, timeunit=0.0, subcalls=True, builtins=True)`
This class is normally only used if more precise control over profiling is needed than what the `cProfile.run()` function provides.
The `Profile` class can also be used as a context manager.
`enable()`
Start collecting profiling data.
`disable()`
Stop collecting profiling data.
`print_stats(sort=-1)`
Create a `Stats` object based on the current profile and print the results to stdout.  
  
```python
import cProfile


@cProfile.Profile
def foo():
    for _ in range(1000):
        pass


foo()
```### █✔█1584894952851451905(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: []**  
  
### 关于开发者测试（Developer Testing，DT），如下描述正确的有（）  
  
开发者测试为了实现测试前移，提前发现问题，只需要在本地完成DT测试，DT工程不需要部署到门禁。### █✔█3717096(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABC']**  
  
### 关于以下运算的打印结果，正确的有( )  
  
`print(5 / 2)` 结果为 2.5
