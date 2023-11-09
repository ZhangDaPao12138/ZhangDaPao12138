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
  
A:1584897052981407746  
```python
from a import a
```  
B:1584897052981407747  
```python
import importlib
a = importlib.import_module("a.a")
```  
C:1584897052985602049  
```python
import importlib
importlib.import_module("a.a")
```  
D:1584897052985602050  
```python
import importlib
a = importlib.import_module("a")
```  
  
### █✔█3817393(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 以下含有多行的代码，可以正常执行的有（ ）  
  
A:11254057  
```PYTHON
s = 'a' + 'b'
    + 'c' + 'd'
    + 'e' + 'f'
```  
B:11254058  
```PYTHON
s = 'a' + 'b' \
    + 'c' + 'd' \
    + 'e' + 'f'
```  
C:11254059  
```PYTHON
s = ('a' + 'b'
    + 'c' + 'd'
    + 'e' + 'f')
```  
D:11254060  
```PYTHON
s = 'a' + 'b' \
    + 'c' + 'd' \
    + 'e' + 'f' \

# 其他代码
```  
  
### █✔█3735004(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['', 'ABD']**  
  
### `str`类型的`join`方法用于将序列中的元素以指定的字符连接生成一个新的字符串，以下选项中合法的有 ( )  
  
A:11032736  
`''.join([1, 2, 3])`  
B:11032737  
`''.join('a', 'b')`  
C:11032738  
`''.join(['a', 'b'])`  
D:11032739  
`''.join(['1', '2', '3'])`  
  
### █✔█3717098(多选)  
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
  
A:11487226  
`print(a[2])`  
B:11487227  
`print(b[2])`  
C:11487228  
`print(c[2])`  
D:11487229  
`print(d[2])`  
  
### █✔█1584894952859840514(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['']**  
  
### 关于可测试性，如下描述正确的有（）  
  
A:1584894961865011202  
可测试性指软件发现故障并隔离、定位故障的能力，以及在一定的时间和成本前提下，进行测试设计、测试执行的能力  
B:1584894961865011203  
可测试性好的代码，更容易被测试，测试出来的问题更容易定位，可以降低测试成本，提升测试质量  
C:1584894961865011204  
可测试性主要包括可隔离性、可控制性、可观测性、可定位性  
D:1584894961865011205  
只有可测试性非常好才能开展DT测试，否则DT测试无法开展  
  
### █✔█1584897049902788609(多选)  
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
  
A:1584897053631524866  
```python
A.x = 1
a = A()
b = a
```  
B:1584897053631524867  
```python
A.x = 1
a = A()
b = A()
```  
C:1584897053631524868  
```python
a = A()
A.x = 1
b = A()
```  
D:1584897053631524869  
```python
a = A()
b = A()
A.x = 1
```  
  
### █✔█1584897050137669634(多选)  
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
  
A:1584897054126452737  
`foo_1`  
B:1584897054130647041  
`foo_2`  
C:1584897054130647042  
`foo_3`  
D:1584897054130647043  
`foo_4`  
  
### █✔█3934720(多选)  
**rightAnswer: ['AD']**  
**wrongAnswer: ['', 'ABCD']**  
  
### 已有`letters`变量：
```python
letters = ['a', 'b']
```
以下哪些选项的代码的执行结果为`ababab`（）  
  
A:11487623  
```python
print("".join(letters) * 3)
```  
B:11487624  
```python
letters.append(letters)
letters.append(letters)
print("".join(letters))
```  
C:11487625  
```python
letters.extend(letters)
letters.extend(letters)
print("".join(letters))
```  
D:11487626  
```python
print("".join(letters * 3))
```  
  
### █✔█3734852(多选)  
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
  
A:11437524  
```python
x.pop(2)
```  
B:11437525  
```python
del x[2]
```  
C:11437526  
```python
x.discard(2)
```  
D:11437527  
```python
x.remove(2)
```  
  
### █✔█3621530(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['', 'BCD']**  
  
### 下列关于产品发布代码中公网地址的使用，下列代码片段中不符合《华为Python语言编程规范》中“代码工程”章节的原则和建议的有（）  
  
A:11435470  
```python
http.client.HTTPConnection('www.python.org')
```  
B:11435471  
```python
urllib.request.urlopen('https://www.huawei.com')
```  
C:11435472  
```python
ftp = FTP('ftp.debian.org')
```  
D:11435473  
```python
test_site = load_site_from_file() # test_site来自配置文件，并在产品资料中进行了说明，支持客户自行修改
http.client.HTTPConnection()  
```  
  
### █✔█3667093(多选)  
**rightAnswer: ['AB']**  
**wrongAnswer: ['', 'ACD']**  
  
### 下面代码打印`math`模块中`pi`，正确的有（）  
  
A:11549907  
```python
from math import pi


print(pi)
```  
B:11549908  
```python
import math


print(math.pi)
```  
C:11549909  
```python
from math import pi


print(math.pi)
```  
D:11549910  
```python
import pi


print(pi)
```  
  
### █✔█1584897049831485441(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['']**  
  
### data1是程序内部数据，data2是来自外部输入的数据，下列代码片段中，不符合《华为Python语言编程规范》中“序列化”章节的要求和建议的是（）  
  
A:1584897053497307137  
`pickle.load(data1)`  
B:1584897053501501441  
`pickle.load(data2)`  
C:1584897053501501442  
`_pickle.load(data1)`  
D:1584897053501501443  
`shelve.load(data2)`  
  
### █✔█3817364(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['']**  
  
###  
```python
if ________:  # 横线处需填入代码
    print("True")
```
以下哪些代码填入到横线处，可使得上面的代码打印出`True`？（ ）  
  
A:11550310  
```python
"None"
```  
B:11550311  
```python
[]
```  
C:11550312  
```python
0.0001
```  
D:11550313  
```python
123
```  
  
### █✔█3717455(多选)  
**rightAnswer: ['ABCD']**  
**wrongAnswer: ['']**  
  
### 如下多个`format`相关代码，哪些选项的代码可以输出结果`foo bar`字符串（）  
  
A:10812315  
```python
sample_dict = {'a': 'foo', 'b': 'bar'}
print('{a} {b}'.format(**sample_dict))
```  
B:10812316  
```python
sample_tuple = 'foo', 'bar'
print('{0} {1}'.format(*sample_tuple))
```  
C:10812317  
```python
sample_list = ['foo', 'bar']
print('{0} {1}'.format(*sample_list))
```  
D:10812318  
```python
sample_set = ('foo', 'bar')
print('{0} {1}'.format(*sample_set))
```  
  
### █✔█3621456(多选)  
**rightAnswer: ['AC']**  
**wrongAnswer: ['']**  
  
### 以下选项符合《华为Python语言编程规范》中“文件”章节的要求和建议的有( )  
  
A:11550306  
`path = os.getcwd() + os.sep + file_name `  
B:11550307  
`path = os.getcwd() + '/myDirectory'`  
C:11550308  
`path = os.path.join(os.getcwd(), 'myDirectory')`  
D:11550309  
`path = os.getcwd() + '/' + myDirectory'`  
  
### █✔█1657955169085710338(多选)  
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
  
A:1657955169207345153  
`from tests.testmodule import *`  
B:1657955169207345154  
`from testmodule import *`  
C:1657955169211539457  
`from .testmodule import *`  
D:1657955169211539458  
不填任何代码  
  
### █✔█3735003(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['AB', 'BCD']**  
  
### 下列反序列化代码中，符合《华为Python语言编程规范》的有：  
  
A:11550402  
```python
import jsonpickle
jsonpickle.decode(some_data)  # some_data是来自网络传输的未经校验的数据
```  
B:11550403  
```python
import jsonpickle
jsonpickle.loads(some_data)  # some_data是来自网络传输的未经校验的数据
```  
C:11550404  
```python
import json
json.loads(some_data)  # some_data是来自网络传输的未经校验的数据
```  
D:11550405  
```python
import json
with open(file_name) as fd:  # 文件来自用户上传
    json.load(fd)
```  
  
### █✔█3963491(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: []**  
  
### 以下代码，哪些可正常执行():  
  
A:11718806  
```print('abc"ab")```  
B:11718807  
```print('abc"ab')```  
C:11718808  
```print("abc"ab")```  
D:11718809  
```print("abc\"ab")```  
  
### █✔█3862589(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABC']**  
  
### 下面哪些对集合x的操作，可以删除元素2：
```python
x = {1, 2, 3}
```  
  
A:11549911  
```python
x.pop()
```  
B:11549912  
```python
x -= {2}
```  
C:11549913  
```python
x &= {1, 3}
```  
D:11549914  
```python
x ^= {2}
```  
  
### █✔█3735283(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['ABCD']**  
  
### 如下删除文件的操作中，哪些选项的代码符合《华为Python语言编程规范》中“代码工程”章节的原则、要求和建议（ ）  
  
A:11549585  
`os.system('rm -f filename.txt')`  
B:11549586  
`shutil.rmtree('dirname')`  
C:11549587  
`os.rmdir('dirname')`  
D:11549588  
`os.remove('filename.txt')`  
  
### █✔█3887741(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['ABCD']**  
  
### 不考虑编程规范，以下if语句的写法可以正确执行的有（）  
  
A:11438161  
```python
if True:
        print("OK")
```  
B:11438162  
```python
if True: print("OK")
```  
C:11438163  
```PYTHON
if True:

    print("OK")
```  
D:11438164  
```python
if True:
print("OK")
```  
  
### █✔█1584894952864034817(多选)  
**rightAnswer: ['ABCD']**  
**wrongAnswer: []**  
  
### 关于可测试性，如下描述正确的有（）  
  
A:1584894961877594113  
可隔离性指软件元素（功能单元、模块/组件等）被分解/隔离的能力，也有称可分解性。  
B:1584894961881788417  
可控制性指对广义输入的控制能力，广义输入包括：被测对象的初始状态构造，被测对象的输入，注入到被测对象内部的异常。  
C:1584894961881788418  
可观测性指对广义输出的观察能力；广义输出包括：被测对象的内部状态或事件（过程），被测对象实际的输出（结果）。  
D:1584894961881788419  
可定位性指输出信息支撑问题分析定位的能力。  
  
### █✔█3734855(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 下面的表达式运行时，不会产生异常的有（）  
  
A:11118466  
```s1 = b"" + "中文"```  
B:11118467  
```s1 = "{}".format("中文")```  
C:11118468  
```s1 = "{}".format("English")```  
D:11118469  
```s1 = "%s" % "English"```  
  
### █✔█1584897050536128513(多选)  
**rightAnswer: ['AD']**  
**wrongAnswer: ['ABD', 'ABCD']**  
  
### 当无法确认目标文件的编码类型时，下列做法符合《华为Python语言编程规范》“文件”章节中的原则、要求与建议的有（）  
  
A:1584897054935953410  
```python
def try_print_unknown_encoding_file(file_path: str, mode: str):
    default_encodings = get_supported_encodings()  # 获取所有支持的编码类型

    for one_encoding in default_encodings:
        try:
            with open(file_path, mode, encoding=one_encoding) as f:
                for line in f:
                    print(line)
                break
        except UnicodeDecodeError:
            continue
        except IOError:
            break
```  
B:1584897054940147713  
```python
def try_print_unknown_encoding_file(file_path: str, mode: str):
    with open(file_path, mode, encoding='utf-8') as f:
        for line in f:
            print(line)
```  
C:1584897054940147714  
```python
def try_print_unknown_encoding_file(file_path: str, mode: str):
    with open(file_path, mode, encoding='ascii') as f:
        for line in f:
            print(line)
```  
D:1584897054940147715  
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
```  
  
### █✔█1584897049542078465(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['ABCD']**  
  
### 以下哪些选项的代码输出结果为`True`（ ）  
  
A:1584897052914298882  
```python
a = "hello"
b = a
a += "world"
print(a == b)
```  
B:1584897052914298883  
```python
a = [1, 2, 3]
b = a
a.append(4)
print(a == b)
```  
C:1584897052914298884  
```python
a = [1, 2, 3]
b = a.copy()
a.append(4)
print(a == b)
```  
D:1584897052914298885  
```python
a = [1, 2, [3]]
b = a.copy()
a[2].append(4)
print(a == b)
```  
  
### █✔█1584900965881163777(多选)  
**rightAnswer: ['BD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 每一种UML建模图都对应有各自不同的核心建模元素，其中顺序图（Sequence Diagram）的关键建模元素有哪些（  ）  
  
A:1584900973321859074  
控制流（Control Flow）  
B:1584900973326053378  
对象/角色（Object/Role）  
C:1584900973326053379  
状态（State）  
D:1584900973326053380  
消息（Message）  
  
### █✔█1584894954608865281(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 小A对一个已有测试用例的模块代码进行重构，在重构代码的过程中，发现原有功能的一个BUG，为了方便，未提交已重构部分代码，直接顺手修改BUG，在保证已有测试用例都通过的前提下，一次性提交上库。后续对此BUG进行测试时发现修改方案并不完善，仍有问题，于是小A回退了所有重构和修改BUG部分的代码。请问在小A的重构过程中存在哪些问题（）  
  
A:1584894965400809474  
不应在测试用例覆盖可能存在遗漏的情况下对代码进行重构  
B:1584894965405003777  
重构时将重构工作和BUG修改工作混做  
C:1584894965405003778  
对识别到的BUG的修改没有先建立测试用例，再实施修改  
D:1584894965405003779  
重构没有小步提交  
  
### █✔█1584894952679485442(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如果输入条件规定了整型参数的范围及默认值，只用边界值分析方法，如下哪些可以作为测试数据（）  
  
A:1584894961470746626  
最大值和最小值  
B:1584894961474940929  
最小值减1  
C:1584894961474940930  
最大值加1  
D:1584894961474940931  
默认值  
  
### █✔█3734850(多选)  
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
  
A:11437977  
`super().__init__()`  
B:11437978  
`super().__init__(self)`  
C:11437979  
`B.__init__()`  
D:11437980  
`B.__init__(self)`  
  
### █✔█3717452(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['BC', 'ABCD']**  
  
### 已知：` x = [4, 1, 0, 3, 5]`， 下面哪些表达式操作可以将 `x`转变为` [4, 1, 3, 5]`（）  
  
A:10812231  
`x[2] = []`  
B:10812232  
`del x[2]`  
C:10812233  
`x.remove(0)`  
D:10812234  
`x[2:3] = []`  
  
### █✔█3717104(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如下表达式的值为`False`的有()  
  
A:11550418  
`{3, 5, 4} < {4, 3, 5}`  
B:11550419  
`{5, 3} < {4, 3, 5}`  
C:11550420  
`{3, 5, 4} > {4, 3, 5}`  
D:11550421  
`{3, 5, 6} > {4, 3, 5}`  
  
### █✔█3667106(多选)  
**rightAnswer: ['CD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 以下哪些变量定义语句执行时会产生异常？（ ）  
  
A:11118490  
`a = 100, 200, 300`  
B:11118491  
`a = b = c = 10`  
C:11118492  
`a, b = 100, 300, 500`  
D:11118493  
`a = 10 20`  
  
### █✔█3667098(多选)  
**rightAnswer: ['ACD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 下列哪些选项符合《华为Python语言编程规范》中“类与面向对象”章节的原则、要求和建议（）  
  
A:10666002  
```python
class Summation:
    def __init__(self, base):
        self._base = base

    def add(self, a: int):
        self._base += a
```  
B:10666003  
```python
class Addition:
    def add(self, a: int, b: int) -> int:
        return a + b
```  
C:10666004  
```python
class Addition:
    @staticmethod
    def add(a: int, b: int) -> int:
        return a + b
```  
D:10666005  
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
```  
  
### █✔█3666975(多选)  
**rightAnswer: ['BC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 如下代码中的命名，符合华为Python编程规范建议的有（ ）  
  
A:11436034  
```python
def chooseABook():
    pass
```  
B:11436035  
```python
class SampleClass(Enum):
    pass
```  
C:11436036  
```python
CONSTANT_FLOAT_PI = 3.1415
```  
D:11436037  
```python
def i(l, o):
    pass
```  
  
### █✔█3621579(多选)  
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
  
A:11436006  
`get_type`函数中的`global`的使用违反规范  
B:11436007  
`set_type`函数中的`type`参数命名违反规范  
C:11436008  
`set_type`函数中的`_g_type`的命名违反规范  
D:11436009  
全局变量`_g_type`的命名违反规范，模块内使用的全局变量不能以下划线开头  
  
### █✔█3621560(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 在linux环境中，为了能够`import`在`/my_path`路径下的包(package)，以下做法不符合《华为Python语言编程规范》中“标准库”章节的要求和建议的有（）  
  
A:11549955  
运行代码前，在bash中执行`export PYTHONPATH=$PYTHONPATH:/my_path`  
B:11549956  
在代码中添加
```python
sys.path.insert(0, './')
sys.path.insert(0, './my_path')
```  
C:11549957  
在代码中添加`sys.path = ['/my_path']`  
D:11549958  
在代码中添加`sys.path.insert(0, '/my_path')`  
  
### █✔█3621464(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABCD']**  
  
### 以下哪些选项符合《华为Python语言编程规范》中“异常处理”章节的要求和建议（）  
  
A:11305530  
```python
# 自定义的异常类
class AuthenticationError(BaseException):
    def __init__(self, message=None):
        super(AuthenticationError, self).__init__(message)
        self.http_code = 404
```  
B:11305531  
```python
# 自定义的异常类
class AuthenticationError(Exception):
    def __init__(self, message=None):
        super(AuthenticationError, self).__init__(message)
        self.http_code = 404
```  
C:11305532  
```python
try:
    with open(file_name) as fd:
        ...
except OSError as e:
    raise UserDefined.InvalidFile('Please check file name') from e
```  
D:11305533  
```python
try:
    with open(file_name) as fd:
        content = fd.read()
except FileNotFoundError as e:
    do_something(file_name, e)
except UnicodeDecodeError as e:
    do_otherthing(file_name, e)
```  
  
### █✔█3211135(多选)  
**rightAnswer: ['BC']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 下面哪些行为是华为开源软件使用规范明确禁止的？  
  
A:11496996  
通过开源软件中心仓commit形式管理对开源原生代码的修改  
B:11496997  
片段引用  
C:11496998  
开源软件确认为自研  
D:11496999  
开源代码和自研代码目录隔离  
  
### █✔█1584900964601901058(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['BCD', 'ABCD']**  
  
### 安全应用的“linux安全设计”原则中，下述描述正确的有（）  
  
A:1584900970998214658  
对系统中的文件存取，要严格限制重要文件的存取，防止未被授权用户访问  
B:1584900971002408961  
对系统访问要进行严格限制，如：对允许登录用户的登录尝试次数，要进行限制  
C:1584900971002408962  
对系统补丁，因为业务不需要，所以，不需要定期安装  
D:1584900971002408963  
只给用户分配足够其完成任务的最小权限  
  
### █✔█2928344(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['ABCD']**  
  
### 针对重构方法，下列说法错误的有（）  
  
A:11436267  
提取接口（Extract Interface）和提取超类（Extract Superclass）均可提取共通代码  
B:11436268  
隐藏委托关系（Hide Delegate）会使代码层次更清晰，因此委托类的功能越多越好  
C:11436269  
当发现某个子类并未带来该有的派生价值时，可以考虑使用移除子类（Remove Subclass）手法进行重构  
D:11436270  
将值域上移到父类（即字段上移 Pull Up Field）会有效减少子类的成员变量，只需要搬移值域，不需要搬移对该值域的操作方法  
  
### █✔█3667050(多选)  
**rightAnswer: ['ABD']**  
**wrongAnswer: ['ABCD']**  
  
### python会从下面哪些地方搜索模块(module)：  
  
A:11032628  
sys.path 指定的路径列表  
B:11032629  
环境变量PYTHONPATH指定的相关路径  
C:11032630  
环境变量PATH指定的相关路径  
D:11032631  
python标准库路径  
  
### █✔█1584897050129281026(多选)  
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
  
A:1584897054118064129  
```python
import cProfile


def foo():
    for _ in range(1000):
        pass


cProfile.run('foo()')
```  
B:1584897054118064130  
```python
import cProfile


def foo():
    for _ in range(1000):
        pass


pr = cProfile.Profile()
pr.enable()
foo()
pr.disable()
pr.print_stats()
```  
C:1584897054118064131  
```python
import cProfile


def foo():
    for _ in range(1000):
        pass


with cProfile.Profile() as pr:
    foo()

pr.print_stats()
```  
D:1584897054118064132  
```python
import cProfile


@cProfile.Profile
def foo():
    for _ in range(1000):
        pass


foo()
```  
  
### █✔█1584894952851451905(多选)  
**rightAnswer: ['ABC']**  
**wrongAnswer: []**  
  
### 关于开发者测试（Developer Testing，DT），如下描述正确的有（）  
  
A:1584894961848233985  
DT主要目的是测试前移，提前发现问题，后端问题解决的成本远大于前端。  
B:1584894961852428289  
重构提倡小步重构，快速反馈，需要频繁的运行DT测试用例（主要是UT/IT等基于PC级的测试工程），确保功能不变，所以DT的构建效率很关键。  
C:1584894961852428290  
多人协同开发，采用分支开发合并到主干的方式，为了保证主干健康，需要将DT工程（主要是UT/IT等基于PC级的测试工程）部署到门禁，构建时间需要满足门禁要求。  
D:1584894961852428291  
开发者测试为了实现测试前移，提前发现问题，只需要在本地完成DT测试，DT工程不需要部署到门禁。  
  
### █✔█3717096(多选)  
**rightAnswer: ['BCD']**  
**wrongAnswer: ['ABC']**  
  
### 关于以下运算的打印结果，正确的有( )  
  
A:11305181  
`print((50 - 5*6) / 4)` 结果为 5  
B:11305182  
`print(8 / 2)` 结果为 4.0  
C:11305443  
`print(7 // 2)` 结果为 3  
D:11305444  
`print(5 / 2)` 结果为 2.5  
  
