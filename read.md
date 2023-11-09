### █✔█3735001(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: []**  
  
### 在Linux环境下，想要提升某Python程序的调度优先级，以使计算任务能够更快完成。以下代码中，能够将自身进程的调度优先级提到最高的是（ ）

**参考**
`os.setpriority`的文档描述：
> `os.setpriority(which, who, priority)`

> Set program scheduling priority. The value **which** is one of **PRIO_PROCESS**, **PRIO_PGRP**, or **PRIO_USER**, and **who** is interpreted relative to **which** (a process identifier for **PRIO_PROCESS**, process group identifier for **PRIO_PGRP**, and a user ID for **PRIO_USER**). A zero value for **who** denotes (respectively) the calling process, the process group of the calling process, or the real user ID of the calling process. **priority** is a value in the range -20 to 19. The default priority is 0; lower priorities cause more favorable scheduling.  
  
`os.setpriority(PRIO_PROCESS, 0)`### █✔█3667109(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果是（ ）

```python
class Foo:
    @property
    def x(self):
        return 10

    def get_y(self):
        return self.__y

    def set_y(self, value):
        self.__y = min(value, 20)

    y = property(get_y, set_y)


my_foo_object = Foo()

my_foo_object.y = 30
b = my_foo_object.y - my_foo_object.x
print(b)
```  
  
产生异常### █✔█3621554(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 如下选项不符合《华为Python语言编程规范》中“外部数据校验”章节的要求和建议的是（）  
  
```python
tmp_file = 'abc.tmp'
os.remove("/tmp/log/%s" % tmp_file)
```### █✔█3717462(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'D', 'A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“变量作用域”章节的要求和建议（）  
  
```python
_acc = 1


def func():
    global _acc
    _acc = "None"


func()
print(_acc)
```### █✔█3667047(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['B']**  
  
### 以下代码的输出结果是（ ）

```python
i = 3


def foo(x):
    def bar():
        return i
    for i in x:
        pass
    return bar()


def foo_1(x):
    def bar():
        return i
    y = [i for i in x]
    return bar()


print(foo(["x", "y"]), foo_1(["x", "y"]))
```  
  
3 3### █✔█1584898267354050562(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 如下Python代码的输出为（）
```python
import collections


a = range(10)
print(isinstance(a, collections.Iterable))
print(isinstance(a, collections.Iterator))
```  
  
False, False### █✔█3717100(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
### 已提供`module_a`，下列哪个选项符合《华为Python语言编程规范》中“包与模块”章节的原则、要求和建议（）
```python
# module_a.py
__all__ = ['ClassA']


class ClassA:
    pass


class ClassB:
    pass
```  
  
```python
# module_c.py
import module_a


def test():
    cls_a = module_a.ClassA()
    cls_b = module_a.ClassB()
```### █✔█1584897049433026562(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 执行下面代码的输出结果是( )
```python
import functools


int_base2 = functools.partial(int, base=2)
int_base16 = functools.partial(int, base=16)
print(int_base2('1000000'))
print(int_base16('1101'))
```
**参考文档：**
>`functools.partial(func, /, *args, **keywords)`
>Return a new partial object which when called will behave like `func` called with the positional arguments `args` and keyword arguments `keywords`. If more arguments are supplied to the call, they are appended to `args`. If additional keyword arguments are supplied, they extend and override `keywords`.  
  
```
64
1101
```### █✔█1584897049760182273(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['', 'B']**  
  
### 当前文件夹下一个测试文件`test_hello.py`，含有以下用例：

```python
def test_a():
    print('hello')
```

以下哪个命令不能执行这个用例（）
**参考文档**

>**Pytest: specifying which tests to run**
>
>Pytest supports several ways to run and select tests from the command-line.
>
>1. Run tests in a module: `pytest test_mod.py`
>2. You can invoke testing through the Python interpreter from the command line: `python -m pytest [...]`
>3. Run tests by node ids
>   Each collected test is assigned a unique nodeid which consist of the module filename followed by specifiers like class names, function names and parameters from parametrization, separated by :: characters.
>   To run a specific test within a module:
>   `pytest test_mod.py::test_func`  
  
`pytest test_hello.py::test_a`### █✔█3952096(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['']**  
  
### 以下代码，输出的结果是：
```python
print([x*x for x in range(4)])
```  
  
```[1, 2, 3, 4]```### █✔█1584897050271887361(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['']**  
  
### 下述哪个选项符合《华为Python语言编程规范》中“数据模型”章节的要求和建议（）  
  
```python
getcontext().prec = 1
print(Decimal(1) / Decimal(7))
```### █✔█3717107(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果为（ ）
```python
class Foo:
    name = 'Hello'

    def say_hello(self):
        print(self.name)

    @classmethod
    def bar(cls):
        cls.name = 'Bye'


foo_one = Foo()
foo_two = Foo()
foo_one.bar()
foo_one.say_hello()
foo_two.say_hello()
```  
  
Bye
Bye### █✔█1584897049382694914(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'D']**  
  
### 以下代码输出结果是( )
```python
dt = datetime.datetime(2022, 2, 22)
dt2 = datetime.timedelta(4)
print(dt + dt2)
```
**参考文档：**
>`datetime.timedelta(days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0)`
>All arguments are optional and default to 0. Arguments may be integers or floats, and may be positive or negative.  
  
```2022-02-22  4:00:00```### █✔█1584894955028295681(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下代码的执行结果是（）
```python
from decimal import Decimal, ROUND_UP


print(Decimal('9.532').quantize(Decimal('0.01'), rounding=ROUND_UP))
print(Decimal('9.536').quantize(Decimal('0.01'), rounding=ROUND_UP))
```
**参考文档：**
>`quantize(exp, rounding=None, context=None)`
>Return a value equal to the first operand after rounding and having the exponent of the second operand. 

>**Rounding modes**
>decimal.`ROUND_UP`
Round away from zero.  
  
`9.54`
`9.53`### █✔█1584894952524296194(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['', 'C', 'A']**  
  
### 针对以下成绩计算程序片段，满足“语句覆盖”的测试用例是（）
```c
if (score < 60) grade = "C";
else if (score < 80) grade = "B";
else if (score < 90) grade = "B+";
else grade = "A";
```  
  
(59,79,89,90)### █✔█3717106(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果为（）

```python
a = ('string',)
for i in range(2):
    a = (a,)
    print(a)
```  
  
```python
(('string',),'string',)
((('string',),'string',),'string',)
```### █✔█1584897050057977858(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['', 'A']**  
  
### 执行以下代码，在第5行`set_trace()`生效并进入调试模式以后，以下哪个命令可以打印出`say`方法的源码？
```python
import pdb


def say() -> int:
    pdb.set_trace()
    a = 90
    b = 1100
    c = b - a
    return c


say()
```
**参考文档：**
> **Debugger Commands**

>`source expression`
   Try to get source code for the given object and display it.
`pp expression`
>   Like the p command, except the value of the expression is pretty-printed using the pprint module.
`p expression`
   Evaluate the expression in the current context and print its value  
  
`source say`### █✔█3963496(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['']**  
  
### 如下Python代码的输出为：
```python
class Yrange:
    def __init__(self, n):
        self.i = 0
        self.n = n

    def __iter__(self):
        return self

    def __next__(self):
        if self.i < self.n:
            i = self.i
            self.i += 1
            return i
        else:
            raise StopIteration()


y = Yrange(5)
print(list(y))
print(list(y))
```  
  
[0]
[1]### █✔█1584898268218077186(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['', 'D']**  
  
### 下面对字典的操作，输出的结果是：
```python
print({1: 1, 2: 4, 3: 9, 4: 16, 5: 25}.pop(4))  
```  
  
```{1: 1, 2: 4, 3: 9, 5: 25}```### █✔█1584897049848262657(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### `s`为含有`n`个元素的`set`对象，`x`为可能在`s`中包含的对象，使用CPython解释器时，执行`x in s`的平均时间复杂度为（ ）  
  
O(n*logn)### █✔█1584897050011840513(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'C', 'A']**  
  
### 如下代码的打印结果为（）

```python
from multiprocessing import Process
 
nums = [11, 22]
 
def run_p1():
    for i in range(4):
        nums.append(i)

def run_p2():    
    for i in range(4):
        nums.append(i)
    print(nums)

if __name__ == '__main__': 
    p1 = Process(target=run_p1)
    p2 = Process(target=run_p2)
    p1.start()
    p1.join()
    p2.start()
    p2.join()
```  
  
产生异常### █✔█1584897049474969602(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下用例中，断言1和断言2的执行结果分别为（）
```python
import unittest
from unittest.mock import Mock


class MyTestCase(unittest.TestCase):
    def test_sqrt(self):
        mock_obj = Mock(return_value=4)
        mock_obj(16)
        mock_obj(17)
        mock_obj.assert_any_call(16)  # 断言1
        mock_obj.assert_called_with(16)  # 断言2
```
**参考文档：**
>`assert_any_call(*args, **kwargs)`:
assert the mock has been called with the specified arguments.
The assert passes if the mock has ever been called, unlike `assert_called_with() `and `assert_called_once_with()` that only pass if the call is the most recent one, and in the case of `assert_called_once_with()` it must also be the only call.

>`assert_called_with(*args, **kwargs)`:
This method is a convenient way of asserting that calls are made in a particular way.  
  
失败
失败### █✔█3816402(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['', 'C', 'B', 'A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“函数与方法”章节的要求和建议（）  
  
```python
def division(x, y):
    if y != 0:
        print(x / y)


division(1, 2)
```### █✔█3621312(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'D']**  
  
### 如下代码的运行结果是（）
```python
class Test(object):
    def process_data(self, data=[]):
        # 排序
        data.sort()
        # 追加结束符
        data.append("End")
        return data


test1 = Test()
print(test1.process_data())
print(test1.process_data())
test2 = Test()
print(test2.process_data(data=["Name:123", "Age:34"]))
print(test2.process_data())
```  
  
```python
['End']
['End', 'End']
['Age:34', 'Name:123', 'End', 'End', 'End']
['Age:34', 'Name:123', 'End', 'End', 'End', 'End']
```### █✔█1584898268901748737(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 以下代码输出结果是（ ）
```python
def reg(func):
    print('running register')
    return func


@reg
def f1():
    print('running f1')


print('running main')
```  
  
running main### █✔█3666978(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['']**  
  
### 以下哪个选项符合《华为Python语言编程规范》中“异常处理”章节的原则、要求和建议（）  
  
```python
try:
    with open(file_name) as fd:
        ...
except (FileNotFoundError, PermissionError):
    log_something(...)
```### █✔█3717456(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'A']**  
  
### 如下正则表达式相关代码的输出是（ ）

```PYTHON
import re


sentence = 'we are humans'
matched = re.match(r'(.*) (.*) (.*)', sentence)
print(matched.group())
```  
  
```AttributeError: 'NoneType' object has no attribute 'group'```### █✔█3717449(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 请问如下代码的执行结果是什么？（ ）
```python
class AException(Exception):
    def __str__(self):
        return "Catch A Exception"


class BException(AException):
    def __str__(self):
        return "Catch B Exception"


try:
    try:
        raise BException
    except AException:
        raise
except Exception as exc:
    print(str(exc))
```  
  
执行时产生未捕获的异常### █✔█3934553(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下代码的执行结果描述正确的是（）  
  
```python
False << 1
```
结果为False### █✔█1584897049663713281(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出为（）

```python
from collections import deque


dq = deque([1])
dq.extend([2, 3])
dq.extendleft([4, 5])
print(list(dq))
```

**参考**

`deque`相关文档描述：
> `extend(iterable)`
>
> Extend the right side of the deque by appending elements from the `iterable` argument.
>
> `extendleft(iterable)`
>
>Extend the left side of the deque by appending elements from `iterable`. Note, the series of left appends results in reversing the order of elements in the `iterable` argument.  
  
[[5, 4], 1, [2, 3]]### █✔█3817370(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C']**  
  
### 以下进行值相等比较的表达式，哪个选项不符合《华为Python语言编程规范》中“运算符与表达式”这一章节中的要求和建议（ ）  
  
```
(1,) is tuple([1])
```### █✔█3621484(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 如下闭包函数结合列表推导代码的计算结果是：

```PYTHON
def multipliers():
    funcs = []
    for i in range(4):
        def closure(x):
            return x * i
        funcs.append(closure)
    return funcs


print([m(2) for m in multipliers()])
```  
  
SyntaxError### █✔█3663828(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'A']**  
  
### 关于编码和解码，以下说法错误的是（   ）  
  
`'北京'.encode('utf8')` 执行不会报错### █✔█3963495(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['', 'C']**  
  
### 如下代码的输出结果是（）
```python
def multipliers():
    return [lambda x: i * x for i in range(5)]


print([m(2) for m in multipliers()])
```  
  
`[8, 8, 8, 8, 8]`### █✔█3667048(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果是（ ）
```python
class A:
    x = 1


class B(A):
    pass


class C(A):
    pass


B.x = 2
A.x = 3
print(A.x, B.x, C.x)
```  
  
3 2 1### █✔█3621451(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['']**  
  
### 下面代码的输出结果是（ ）
```python
s = ["seashell", "gold", "pink", "brown", "purple", "tomato"]
print(s[1:4:2])
```  
  
`['gold', 'brown']`### █✔█1584898267953836033(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['', 'A']**  
  
### 以下代码运行输出结果是（ ）

```python
def test(n):
    prev, cur = 2, 2
    for _ in range(n):
        yield cur
        prev, cur = cur, cur*prev


if __name__ == '__main__':
    value = 0
    for i in test(5):
        value = i
    print(value)
```  
  
256### █✔█3667108(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'D', 'A']**  
  
### 假设文件`file.txt`的内容为：

```
huawei
```

以下代码执行后的`file.txt`文件内容是？（假定`file.txt`没有被其他进程读写）

```python
with open("file.txt", "wt") as file:
    file.write("hello")
    file.write("world")
```  
  
```
huawei
hello
world
```### █✔█3663830(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果是（ ）
```python
print(float("230" * int('2')))
```  
  
`230230`### █✔█3621463(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 关于类的方法排列顺序，以下哪个选项符合《华为Python语言编程规范》的要求和建议（）  
  
```python
class Example:
    def __new__(cls):
        ...

    def __init__(self):
        ...

    @property
    def value(self):
        ...

    def _private(self):
        ...

    def example(self):
        ...

    @classmethod
    def test(cls):
        ...
```### █✔█3921589(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 执行以下代码的输出结果是( )
```python
import time
from threading import Thread


def countdown(n):
    while n > 0:
        print('T-minus', n)
        n -= 1
        time.sleep(5)


# Create and launch a thread
t = Thread(target=countdown, args=(3,))
t.start()
t.join()
print("end")
```  
  
```shell
end
T-minus 3
T-minus 2
T-minus 1
```### █✔█3667110(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['']**  
  
### 以下开发测试版本所用的断言，哪个选项不符合《华为Python语言编程规范》中“代码测试”章节的要求和建议（）  
  
```python
import unittest


class TestCaseDemo(unittest.TestCase):
    def test_object_is_in_collection (self):
        x = set([1,2,3,4])
        y = set([1,3,5])
        self.assertNotIn(5, x - y)
        self.asserIn(5, y - x)
```### █✔█1584898269509922818(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['', 'A']**  
  
### 以下关于`Docstring`的处理代码执行结果为( )

```python
def sample_function():
    """This is a sample function always return True."""
    return True


print(sample_function.__doc__[10: 16])
```  
  
`True`### █✔█3667143(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['']**  
  
### 以下代码的输出结果是（）

```python
import asyncio


async def say_after(delay, what):
    await asyncio.sleep(delay)
    print(what)


async def main():
    task1 = asyncio.create_task(say_after(1, 'hello1'))
    task2 = asyncio.create_task(say_after(2, 'world1'))

    await say_after(1, 'hello2')
    await say_after(2, 'world2')
    await task1
    await task2


asyncio.run(main())
```  
  
```
hello2
hello1
world1
world2
```### █✔█1584897050049589249(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['', 'D']**  
  
### 执行以下代码，在第2行`breakpoint()`生效并进入调试模式以后，以下哪个命令序列可以打印出c变量的值？

```python
def say() -> int:
    breakpoint()
    a = 90
    b = 1100
    c = b - a
    return c
```
  
  
`n`
`n`
`p c`### █✔█1584897049642741762(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C', 'A']**  
  
### 以下代码的运行输出结果是

```python
from collections import deque


dq = deque([1], 3)
dq.extend([2, 1, 3, 1])
print(list(dq))
```

**参考**

`deque`相关文档描述：
> `class collections.deque([iterable[, maxlen]])`
>
> Returns a new `deque` object initialized left-to-right (using `append()`) with data from `iterable`. If `iterable` is not specified, the new `deque` is empty.
>
> If `maxlen` is not specified or is `None`, deques may grow to an arbitrary length. Otherwise, the deque is bounded to the specified maximum length. Once a bounded length deque is full, when new items are added, a corresponding number of items are discarded from the opposite end. 
>
> `extend(iterable)`
> Extend the right side of the deque by appending elements from the `iterable` argument.  
  
`[1, 3, 1]`### █✔█3887738(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['A']**  
  
### 以下代码的执行结果正确的是（）  
  
```python
2.0 << 2
```
结果为8### █✔█3667104(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: []**  
  
### 以下代码运行结果是（ ）
```python
class Demo:
    def check(self):
        return "Demo"

    def display(self):
        print(self.check())


class DemoDerived(Demo):
    def check(self):
        return "Derived"


Demo().display()
DemoDerived().display()
```  
  
产生异常### █✔█1584898267580542977(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 以下代码输出结果是()

```python
class B(Exception):
    pass


class C(B):
    pass


class D(C):
    pass


for cls in [B, C, D]:
    try:
        raise cls()
    except B:
        print("B", end=",")
    except D:
        print("D", end=",")
    except C:
        print("C", end=",")
```  
  
不输出任何信息### █✔█3621497(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['B']**  
  
### 下述哪个选项符合《华为Python语言编程规范》中“数据模型”章节的要求和建议（）  
  
```python
if type(user) == User:
    print(user.name)
```### █✔█1584894951593160706(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['D']**  
  
### 常见的白盒测试代码覆盖率分为：语句覆盖、判定覆盖、条件覆盖、判定/条件覆盖、条件组合覆盖、路径覆盖。以下选项对四种代码覆盖率定义描述正确的是（）  
  
条件组合覆盖：设计的测试用例应该使得每个判定中的各个条件的各种可能组合都全量覆盖。### █✔█1584897050028617730(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 执行如下代码的输出为（）

```python
from threading import Thread

def work1(nums):
    nums.append(2)

def work2(nums):
    nums.append(3)
    print(nums)

g_nums = [0, 1]
t1 = Thread(target=work1, args=(g_nums,))
t2 = Thread(target=work2, args=(g_nums,))
t1.start()
t1.join()
t2.start()
t2.join()
```  
  
```
[0, 1, 2, 3]
```### █✔█3816403(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“变量作用域”章节的要求和建议（）  
  
```python
_global = 1
def test():
    local_number = 2
    if local_number == _global:
        raise MyException
```### █✔█3717458(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'D', 'A']**  
  
### 运行以下代码的输出结果是（ ）
```python
class Foo:
    @classmethod
    def create_one(cls):
        return cls()

    @staticmethod
    def create_two():
        return Foo()


class Bar(Foo):
    pass


bar_one = Bar.create_one()
bar_two = Bar.create_two()
print(isinstance(bar_one, Bar))
print(isinstance(bar_two, Bar))
```  
  
False
False### █✔█1584898269266653185(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['A']**  
  
### 以下程序输出结果是（ ）
```python
def func(a):
    n = a

    def func1():
        print('n=', n)

    def func2():
        nonlocal n
        n = a + 2

    return func1, func2


f1, f2 = func(3)
f1()
f2()
f1()
```  
  
产生异常### █✔█3621502(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'D']**  
  
### 如下代码输出结果是（ ）
```python
l = [1, 3, 5]
li = iter(l)
print(3 in li)
print(3 in li)
```  
  
```
False, True
```### █✔█3862602(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 以下代码执行输出结果为（ ）
```python
class Parrot(object):
    def __init__(self):
        self._voltage = 100000

    @property
    def voltage(self):
        return self._voltage

    @voltage.setter
    def voltage(self, value):
        if value < 0:
            raise ValueError("Invalid voltage value")
        self._voltage = value


p = Parrot()
p.voltage = -1
print(p.voltage)
```  
  
```100000```### █✔█1584897049445609474(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 下面这段代码的输出结果是( )：

```python
import itertools


a_list = [("Animal", "cat"),
          ("Animal", "dog"),
          ("Bird", "peacock"),
          ("Bird", "pigeon")]

an_iterator = itertools.groupby(a_list, lambda x: x[0])
for key, group in an_iterator:
    key_and_group = {key: list(group)}
    print(key_and_group)
```
**参考文档：**

>`itertools.groupby(iterable, key=None)`
Make an iterator that returns consecutive keys and groups from the `iterable`. The `key` is a function computing a key value for each element. If not specified or is `None`, `key` defaults to an identity function and returns the element unchanged. Generally, the `iterable` needs to already be sorted on the same `key` function.  
  
```
{'cat': [('Animal', 'cat')]}
{'dog': [('Animal', 'dog')]}
{'peacock': [('Bird', 'peacock')]}
{'pigeon': [('Bird', 'pigeon')]}
```### █✔█1660570312776900609(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['A']**  
  
### 执行以下代码的输出结果是（）

```python
x = 0
y = 0


def f():
    x = 1

    class C:
        x = x
        y = y

    print(C.x, C.y)


f()
```  
  
1 0### █✔█3862598(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['A']**  
  
### 以下程序，运行后结果可能是（）

```python
class MyClass():
    pass

myclass = MyClass()
print(myclass)
print(type(myclass))
yourclass = type('YourClass', (), {})
print(yourclass)
print(type(yourclass))
```  
  
```
<__main__.MyClass object at 0x000001E431AA7A88>;
<class '__main__.MyClass'>;
<class '__main__.YourClass'>;
<class 'type'>;
```### █✔█1584897049487552513(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['A']**  
  
### 以下代码执行时，`print`语句产生的打印结果为（ ）
```python
from unittest.mock import Mock
import unittest
import math


class TestSqrt(unittest.TestCase):
    def test_sqrt(self):
        mock_func = Mock(return_value=4.0, side_effect=math.sqrt)
        print(mock_func(9.0))


if __name__ == '__main__':
    unittest.main()
```
**参考文档：**
>```class unittest.mock.Mock(spec=None, side_effect=None, return_value=DEFAULT, wraps=None, name=None, spec_set=None, unsafe=False, **kwargs)```
Create a new ```Mock``` object. ```Mock``` takes several optional arguments that specify the behaviour of the Mock object:

>```side_effect```: A function to be called whenever the Mock is called.  
If you pass in a function it will be called with same arguments as the mock and unless the function returns the ```DEFAULT``` singleton the call to the mock will then return whatever the function returns. If the function returns ```DEFAULT``` then the mock will return its normal value (from the ```return_value```).

>```return_value```: The value returned when the mock is called. By default this is a new Mock (created on first access).  
  
`None`### █✔█3921609(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['D']**  
  
### 如下程序的输出结果是（）
```python
result = list(filter(lambda x: x % 2, range(4)))
print(result)
```  
  
```
None
```### █✔█1666686844074614785(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 以下哪个选项中的代码单独填入到横线处时，整段代码运行输出结果为`Jun 19,Monday`（ ）
```python
from datetime import datetime


date1 = datetime(2023, 6, 19)
date2 = ______  # 横线处需填入代码
print(date2)
```

**参考：**
> **strftime() and strptime() Format Codes**
> `%a`  Weekday as locale’s abbreviated name. Example: Sun, Mon, …, Sat (en_US)
> `%A`  Weekday as locale’s full name.  Example: Sunday, Monday, …, Saturday (en_US)
> `%b`  Month as locale’s abbreviated name. Example: Jan, Feb, …, Dec (en_US)
> `%B`  Month as locale’s full name. Example: January, February, …, December (en_US)  
  
`datetime.strftime(date1, '%b %d,%a')`### █✔█3621448(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: []**  
  
### 语句`print(eval('2+4'))`执行后的输出结果是()
  
  
`eval('2+4')`### █✔█3667100(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 以下代码会输出什么( )
`print(int("1" + "2") + 2)`  
  
`32`### █✔█1584897049865039873(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['D']**  
  
### `s`为含有`n`个元素的`list`对象，`x`为可能在`s`中包含的对象，使用CPython解释器时，执行`x in s`的平均时间复杂度为（ ）  
  
O(n*logn)### █✔█3887742(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 下述哪个选项的代码不符合《华为Python语言编程规范》中“函数与方法”章节的要求和建议（）  
  
```python
from dataclasses import dataclass


@dataclass
class Student:
    name: str
    age: int
    gender: str
    height: int


def process_student_info(student):
    print(student.name)


process_student_info(Student("bob", 19, "male", None))
process_student_info(Student("keri", 21, "female", None))
```### █✔█3921610(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
### 如下Python程序的输出是：
```python
data = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
result = [data[row][2] for row in range(3)]
print(result)
```  
  
```
[3, 6, 8]
```### █✔█3621482(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 关于函数多装饰器应用的场景，以下代码执行的结果为：

```python
def decorator_function_a(function):
    def inner_function():
        print("decorator a running..")
        function()
    return inner_function


def decorator_function_b(function):
    def inner_function():
        function()
        print("decorator b running..")
    return inner_function


@decorator_function_a
@decorator_function_b
def sample_function():
    print("sample function running..")


if __name__ == "__main__":
    sample_function()
```  
  
```python
decorator a running..
sample function running..
sample function running..
decorator b running..
```### █✔█3621517(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 对于`Example`成员的访问，以下哪个选项符合《华为Python语言编程规范》中“类与面向对象”章节的要求和建议（）

```python
class Example:
    def __init__(self, eid, value):
        self._eid = eid
        self._value = value

    @property
    def eid(self):
        return self._eid

    @property
    def value(self):
        return self._value
```  
  
```python
a = Example('a', 'test')
eid_a = a.eid
```### █✔█3621563(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['B', 'A']**  
  
### 以下哪个选项符合《华为Python语言编程规范》中“异常处理”章节的要求和建议（）  
  
```python
try:
    fp = open('test_read.txt', encoding='utf8')
    print(fp.read())
except FileNotFoundError:
    pass
except UnicodeDecodeError:
    pass
finally:
    fp.close()
```### █✔█1656558871400423426(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['B']**  
  
### 以下代码的输出结果是（）
```python
from decimal import Decimal


x1 = Decimal(0.000001) + Decimal(0.0000001)
print(x1 == Decimal(0.0000011))

x2 = Decimal("0.000001") + Decimal("0.0000001")
print(x2 == Decimal("0.0000011"))
```  
  
False
False### █✔█1584897051450486786(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 以下代码的执行结果为（）

```python
s = (1,)
t = (2)
print(s + t)
```  
  
运行时抛出异常### █✔█3621553(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C']**  
  
### 在生成一串无需改变的固定常量时,下列哪个选项符合《华为Python语言编程规范》中“性能与资源管理”章节的要求和建议（）

```python
LANGUAGE_LIST1 = ['en', 'en_US', 'ar', 'ar_AE', 'ar_BH', 'be', 'de', 'de_CH', 'de_DE_EURO', 'ru', 'el', 'zh_CN']

LANGUAGE_LIST2 = ('en', 'en_US', 'ar', 'ar_AE', 'ar_BH', 'be', 'de', 'de_CH', 'de_DE_EURO', 'ru', 'el', 'zh_CN')
```  
  
都不符合### █✔█1584897051316269057(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 以下代码的运行结果是( )
```python
def func():
    yield (x for x in range(3))


for x in func():
    print(next(x))
```  
  
`<generator object func.<locals>.<genexpr> at 0x000001F152299480>`（地址可能在不同运行环境中有所不同）### █✔█1584897049386889218(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 执行以下代码的输出是( )
```python
d2 = datetime.datetime(5, 6, 7, 8, 9, 10)
print(d2.year, " Q", d2.month // 4 + 1, sep='')
```
**参考文档：**
>`datetime(year, month, day, hour=0, minute=0, second=0, microsecond=0, tzinfo=None, *, fold=0)`
The `year`, `month` and `day` arguments are required  
  
```10 Q3```### █✔█1584894954063605762(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 需求描述要清晰、需求可验收。小明看到以下关于设备数据采集功能相关的需求，请你帮忙审核下，需求满足清晰、 可验收标准的是（）  
  
数据采集性能提升10%左右### █✔█1584894953145053186(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 在一个文字处理软件的设计中，需要支持用户在编辑中的撤销和重做等动作，为了实现该功能，以下哪种设计模式最适合该功能的实现（ ）  
  
享元模式（Flyweight Pattern)### █✔█1584894953052778497(单选)  
**rightAnswer: ['E']**  
**wrongAnswer: ['C', 'A']**  
  
### 某个被测对象的因子取值情况如下表所示，当使用N-wise方法进行因子组合时，N=3时对应的测试用例个数是多少（）
因子a：3个取值
因子b：4个取值
因子c：5个取值
因子d：2个取值  
  
120### █✔█1579281042928508930(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C', 'A']**  
  
### 以下哪项关于开源软件原生代码修改的说法不正确？  
  
对开源软件原生代码修改，建议尽量封装成函数或宏方式，提高扩展性### █✔█4006764(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 如下代码存在哪种坏味道（请忽略不同编程语言的规范差异）（ ）
```cpp
class User {
private:
    ContactInfo contactInfo;

public:
    void GetUserAddress(Address& address)
    {
        address.Country = contactInfo.GetCountry();
        address.City = contactInfo.GetCity();
        address.Street = contactInfo.GetStreet();
        address.Community = contactInfo.GetCommunity();
        address.Building = contactInfo.GetBuilding();
        address.Floor = contactInfo.GetFloor();
    }
};
```  
  
狎昵关系（Inappropriate Intimacy）/内幕交易（Insider Trading）### █✔█3963500(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C', 'A']**  
  
### 以下代码的运行结果是（ ）
```python
def decorate(func):
    def wrapper():
        print('start')
        func()
        print('end')
    return wrapper


@decorate
def show():
    return 'show'


print(show())
```  
  
start
end
None### █✔█3963492(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['B', 'A']**  
  
### 下列哪个选项符合《华为Python语言编程规范》中“类与面向对象”章节的原则、要求和建议（）  
  
```python
import sys


class Base:
    def __init__(self):
        self.running = False

    def start(self, *args):
        self.running = True


class Addition(Base):
    def __init__(self):
        Base.__init__(self)
        self.running = True
```### █✔█3949573(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 某汽车变速箱通过旋钮换挡，换挡旋钮只能左右旋转依次切换档位，如图旋钮上从左到右的档位依次是`P-R-N-D-S`档，注意并不能循环换挡（即P档下左旋仍为P档，S档时右旋仍为S档）。
![image](https://proxy.ilearning.huawei.com/edxs3proxy/exam-public/rtf/d5c3f03145a9456e9079e2d598d6e797_a86a733257204378be4b19331f8cf67f_1.png)
变速箱的换挡逻辑规则如下：
1）由于P档是停车挡，任何档位直接进入P档停车是很常用的功能，所以车辆另外设置了单独的P档按键。
2）车辆在静止状态`（车速<1）`下任意档位按下P档按键会直接进入P档。
3）出于行驶安全考虑和避免误操，车辆行驶状态`（车速>=1）`下按下P档按键不会立刻进入P档，需要长按P档按键`(按下>5秒)`才会强制进入P档。
4）车辆行驶状态`（车速>=1）`下通过换挡旋钮只能在D和S档之间切换，其他档位间旋钮旋转无效。
5）忽略空档滑行等情况，车辆处于P档或N档时一定为静止状态`（车速<1）`，而处于其他档位时则可能为行驶状态`（车速>=1）`。
变速箱控制软件设计人员根据上述换挡逻辑绘制了状态图，大家评审时提出很多意见，请你指出这些意见中错误的是（）
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/c5f1da6d-0d7c-4267-881d-bf57a0bbbf4e.png"  />  
  
N档状态下的`“按下P按键”`转移（Transition）中不需要检查车辆行驶状态，应该删除监护条件（Guard conditions）限制### █✔█3934704(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“运算符”章节的原则、要求和建议（ ）  
  
判断tuple内容是否为空：
```python
if my_tuple is ():
```### █✔█3887735(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C', 'D']**  
  
### 以下代码的运行结果是( )
```python
def func():
    yield (x for x in range(3))


for x in func():
    print(tuple(x))
```  
  
`<generator object func.<locals>.<genexpr> at 0x000001F152299480>`（地址可能在不同运行环境中有所不同）### █✔█3887342(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 关于下面的代码的输出，正确的是：
```python
language = u"中文"
print(len(language), hasattr(language, "encode"))
```
  
  
`4 False`### █✔█3862596(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 以下代码的输出结果是（ ）
```python
def func(a, *b):
    for item in b:
        a += item
    return a


m = 0
print(func(m, 1, 1))
```  
  
产生异常### █✔█3817397(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 有如下几个文件，目录结构及文件内容如下：
```shell
.
├── test1.py
└── tests
    ├── __init__.py
    └── test2.py
```

`test1.py`:
```python
from tests import test2


test2.test_2()
```

`tests/__init__.py`:
```python
import test2


def test2():
    print('hello python')
```

`tests/test2.py`:
```python
def test_2():
    print('hello world')
```
运行test1.py的结果是：  
  
AttributeError: module 'tests' has no attribute 'test2### █✔█3817392(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 关于以下代码，说法正确的是（）

```python
class A:
    a = 42
    b = list(a + i for i in range(10))
    print(b)


A()
```  
  
代码能正常执行，但是没有任何输出### █✔█3817384(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 以下代码的执行结果为（）

```python
a = [0, 1, 2, 3]
for a[-1] in a:
    print(a[-1])
```  
  
`0 1 2`### █✔█3678138(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 如下代码重构时推荐使用哪种设计模式（请忽略不同语言的规范和语法差异）（ ）
```cpp
class Object {
public:
    void ExecuteCmd(uint32_t cmd)
    {
        if (mode == WORKING) {
            DoSomething();
            mode = GetNewMode(cmd);
        } else if (mode == REST) {
            DoOtherthings();
            mode = GetNewMode(cmd);
        } else if (/* ... */) {
            /* ... ... */
        }
    }
private:
    uint32_t mode;
};
```
  
  
状态(State)模式### █✔█3667090(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 以下代码的执行结果为（ ）
```python
class A:
    def __new__(self):
        print("A's __new__() invoked")
        return object.__new__(self)

    def __init__(self):
        print("A's __init__() invoked")


class B(A):
    def __new__(self):
        print("B's __new__() invoked")

    def __init__(self):
        print("B's __init__() invoked")


obj1 = B()
obj2 = A()
```  
  
```
B's __new__() invoked
B's __init__() invoked
A's __new__() invoked
```### █✔█3661663(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 下述哪个选项符合《华为Python语言编程规范》中“控制语句”章节的要求和建议（ ）  
  
```python
over_flag = False

for i in range(0,5):
    for j in range(0,3):
        if j == i:
            over_flag = True
            break
            print("i的值为：%d")
    if  over_flag:
        break
```### █✔█3658966(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 假设有个算法的输入对象是两个名为S_Op和S_Num的栈，
算法的执行过程如下：
如果满足条件 “S_Num中元素个数大于等于2”且“S_Op中元素个数大于等于1”，则循环依次执行下面的操作步骤
    1、从 S_Num 中弹出1个操作数 a 
    2、从 S_Num 中弹出1个操作数 b
    3、从 S_Op 中弹出一个运算符 op
    4、将 a op b 的结果压入 S_Num
上述流程结束后S_Num栈顶的元素值就是算法的输出值。
则下面哪个S_Op和S_Num栈（左边栈底，右边栈顶）应用上述算法之后其值不等于24？（）  
  
S_Op  : + +
S_Num : 2 4 6 8 10### █✔█3658962(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['D', 'A']**  
  
### 下列关于软件开发和软件测试说法正确的是（）  
  
系统测试的主要方法是白盒法### █✔█3658961(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C', 'A']**  
  
### 在进行二进制文件差异分析时，需要分析差异产生的根因，并尝试制定差异消除方案。对于引入原因明确但无法消除，且容易验证的差异，被定义为可解释差异。下列哪个选项不属于可解释差异（）  
  
ini文件### █✔█3658959(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 给定一个数组A[N]，每一项都是长度为M的字符串。假设这些N个字符串已经按照字典顺序在A[N]中排序。如果使用二分查找法在A[N]中查找某一个字符串时（如果有多个匹配，在找到第一个成功的就结束），下述哪一个是对应算法的最坏时间复杂度？（）  
  
O(N*Log(M)### █✔█3621568(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### data是来自外部的数据，PyYAML是最新版本，下列反序列化操作中，不符合《华为Python语言编程规范》的是（）  
  
`yaml.safe_load_all(data)`
### █✔█3621516(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 下面这段代码的输出结果是（）

```python
class GrandParent:
    def __init__(self):
        print("Hello GrandParent")


class Parent(GrandParent):
    def __init__(self):
        super().__init__()
        print("Hello Parent")


class Child(GrandParent, Parent):
    def __init__(self):
        super().__init__()
        print("Hello Child")


if __name__ == '__main__':
    c = Child()
```  
  
```
Hello GrandParent
Hello GrandParent
Hello Parent
Hello Child
```### █✔█3621506(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'D', 'A']**  
  
### entities中的对象，只会被顺序遍历一次，且不需要长期持有，下列代码符合《华为Python语言编程规范》中“性能与资源管理”章节的原则、要求与建议的是（）
```python
class Entity:
    def __init__(self, eid = 0):
        self.__eid = eid
```  
  
```python
entities = [None] * 1000
for i in range(1000):
    entities.append(Entity(i))
```### █✔█3621504(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“函数与方法”章节的要求和建议（）  
  
```python
def fun(arg_0, arg_1='', arg_2=set()):
    arg_2.add(arg_0)
    arg_2.add(arg_1)
    print(arg_2)
```### █✔█3621495(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['C', 'A']**  
  
### 关于用pdb设置断点，下列说法正确的是?  
  
可以在import语句行设置断点### █✔█3621459(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 虚拟环境管理工具tox可用于对将要发布的python库文件进行多版本环境下的兼容测试。配置文件tox.ini有这样的内容: 
```python
[tox]
envlist = {py36,py27}-django15
```
对它的含义理解，如下描述中正确的是？（）  
  
tox运行两个环境下的测试：py27-django15和py36-django15。如果后面配置了basepython字段，环境的python版本由basepython指定；否则，由环境名中的pyxx来决定### █✔█3621455(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 在一个8核心CPU的机器上运行仅使用了threading库的Python程序（假定使用CPython，并且除了threading库以外未调用其他任何库），则此程序中同一时刻最多有几个线程在执行()  
  
8### █✔█3582828(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['A']**  
  
### 根据《身份和访问管理安全设计规范》，以下哪种场景不应该产生安全告警（ ）  
  
业务模块加载失败### █✔█3582821(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 在一个简化的虚拟农场游戏中， 对于农场（Farm）的设计需要满足产品多样性和灵活生产的诉求：农场可以养动物（Animal），如养马（A_Horse）、养牛（A_Cattle）等；还可以培养植物（Plant），如种菜（P_Vegetables）、种水果（P_Fruitage）等；为了简化设计，假设要求每个农场都要生产一种动物和一种植物，不同的农场生产不同的动植物，若采用抽象工厂 模式（Abstract Factory Pattern）来设计，以下模型图中能正确表达这一设计模式的是(  )  
  
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/9db04570-79cb-49d3-b6e8-2ed6694ec09b.png" alt="" />### █✔█3249797(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### 两台设备间需要通过外部网络传输和协商秘钥信息，为了防止传输过程中信息被攻击者篡改，下面哪个方法可以识别出信息被篡改：  
  
使用TLS协议来传输信息### █✔█3249796(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 基于《密码算法应用规范》,下列哪种随机数生成方式自身会出现安全漏洞？  
  
JDK的java.security.SecureRandom### █✔█3133572(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 某系统在启动时会一次性读取配置文件信息，并将其存储在类型为Configuration(类名)的对象中供其他模块使用。在这个场景下，以下做法正确的是（ ）  
  
将备忘录(Memento)模式应用于Configuration### █✔█2974541(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C', 'A']**  
  
### SQL注入是指后台数据库对用户输入数据的合法性没有判断或过滤不严，攻击者可以在web页面中插入额外的SQL语句，实现对后台数据库的非法访问操作。以下关于SQL Injection（SQL注入）的说法错误的是哪个？  
  
SQL Injection 安全漏洞可以通过安全的输入校验机制来预防。### █✔█2952955(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 某公司欲开发一个软件系统的在线文档帮助系统，用户可以在任何一个查询上下文中输入查询关键字，如果当前查询环境下没有相关内容，则系统会将查询按照一定的顺序转发给其他查询环境。基于上述需求，采用下面哪种模式最为合适？（ ）  
  
适配器(Adapter)模式### █✔█1654755970344558594(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C']**  
  
### 下列哪个选项的代码单独填到横线处时，符合《华为Python语言编程规范》中“并行与并发”章节的原则、要求和建议：()

```python
import subprocess


if __name__ == "__main__":
    proc = subprocess.Popen('ping 192.168.23.45 -t')
    ______  # 在横线处填写代码
```  
  
```python
try:
    outs, errs = proc.communicate()
except subprocess.TimeoutExpired:
    proc.kill()
```### █✔█1584897049944731650(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
###  
```python
n = 1

def func(a):
    n = a

    def func1():
        global n
        n = a + 1

    def func2():
        print('n={}'.format(n))

    return func1, func2


f1, f2 = func(3)
f1()
f2()
```
运行以上代码的输出结果是（）  
  
`n=4`### █✔█1584897049412055041(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 以下代码会输出什么( )
```python
a = 2
b = "6"
print(math.fsum([1, a, 3, 4, 5, b]))
```
**参考文档：**
>`math.fsum(iterable)`
>Return an accurate floating point sum of values in the iterable. Avoids loss of precision by tracking multiple intermediate partial sums:  
  
执行错误### █✔█3667102(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 以下为test.py文件的内容：
```python
import sys


print(sys.argv[1])
```
使用`python test.py Hello world`命令运行这个脚本，输出为（ ）  
  
Hello world### █✔█3921607(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['B']**  
  
### 执行如下代码的输出是（）

```python
class B(Exception):
    pass


class C(B):
    pass


class D(C):
    pass


exc = []
for cls in [B, C, D]:
    try:
        raise cls()
    except B:
        exc.append("B")
    except C:
        exc.append("C")
    except D:
        exc.append("D")
print("".join(exc))
```  
  
BBB### █✔█3663896(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 对于以下代码的运行输出结果，正确的说法是（ ）

```python
class Person:
    __slots__ = ('name', 'age')


person = Person()
person.name = 'John'
person.name = 'Kate'
person.nationality = 'CN'
person.nationality = 'UK'
print(f"{person.name} is from {person.nationality}")
```  
  
Kate is from CN### █✔█3734858(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['A']**  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“表达式”章节的原则、要求和建议（ ）  
  
```python
exact_division0 = lambda x: 10 // x
print(exact_division0(0))
```### █✔█3667141(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 以下代码执行结果是（）
```python
result = [1, 2, 3, 4, 5]
result[1:3] = 'abc'
print(result[2])
```  
  
b### █✔█3621471(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
### 如下程序输出正确的是：

```python
class ListMetaclass(type):
    def __new__(cls, name, bases, attrs):
        print(name)
        print(bases)
        attrs['add'] = lambda self, value: self.append(value)
        return type.__new__(cls, name, bases, attrs)


class DefinedList(list, metaclass=ListMetaclass):
    pass


definedList = DefinedList()
definedList.add(1)
```  
  
```
ListMetaclass
 (<class 'type'>,)
```### █✔█3887748(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 在独占CPU运行的情况下，如下Python代码的输出为（）
```python
import threading
import time


mutex_1 = threading.Lock()
mutex_2 = threading.Lock()


def test1():
    print("in test1 lock 1")
    mutex_1.acquire()
    time.sleep(3)
    mutex_2.acquire(timeout=1)
    print("in test1 step lock 2")
    mutex_1.release()


def test2():
    print("in test2 lock 2")
    mutex_2.acquire()
    time.sleep(3)
    mutex_1.acquire()
    print("in test2 step lock 1")
    mutex_1.release()
    mutex_2.release()


if __name__ == '__main__':
    t1 = threading.Thread(target=test1)
    t2 = threading.Thread(target=test2)
    t1.start()
    time.sleep(1)
    t2.start()
    t1.join()
    t2.join()
```  
  
in test1 lock 1
in test2 lock 2
in test2 step lock 1
in test1 step lock 2### █✔█3934718(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['C']**  
  
### 如下代码执行后的打印结果为：

```python
foo = 1


def sample_function(bar):
    global foo

    def inner_function(baz):
        foo = baz
        return foo

    inner_function(bar)
    return foo


if __name__ == "__main__":
    print(sample_function(100))
```  
  
产生异常### █✔█3621488(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 以下代码执行后的打印输出为（）

```python
t1 = (1, 2)
t2 = t1 * 2
t3 = t1 + t2
print(t3)
```  
  
`(1, 2, 1, 2, 1, 2)`### █✔█1584897049873428482(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### `s`为含有`n`个元素的`list`对象，使用CPython解释器时，执行`t = s[:]`的平均时间复杂度为（ ）  
  
O(n*logn)### █✔█1584897051391766530(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: []**  
  
### 以下代码执行输出结果是（ ）
```python
def foo():
    return 1, 2, 3


result = foo()
print(result)
```  
  
产生异常### █✔█3621539(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['B']**  
  
### 如下正则表达式相关代码的输出是（ ）

```PYTHON
import re


sentence = 'we are humans'
matched = re.match(r'(.*) (.*) (.*)', sentence)
print(matched.groups())
```  
  
```AttributeError: 'NoneType' object has no attribute 'groups'```### █✔█1584897049730822145(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: ['D']**  
  
### 以下测试用例将依次运行哪几个参数组合的测试()

```python
import pytest


@pytest.mark.parametrize('x', [2])
@pytest.mark.parametrize('y', [3, 4])
def test_func(x, y): 
    assert x + y > 0

```

**参考材料：**

>**@pytest.mark.parametrize: parametrizing test functions**
>
>The builtin `pytest.mark.parametrize` decorator enables parametrization of arguments for a test function.
>To get all combinations of multiple parametrized arguments you can stack `parametrize` decorators.
>
>```python
>import pytest
>
>
>@pytest.mark.parametrize("x", [0, 1])
>@pytest.mark.parametrize("y", [2, 3])
>def test_foo(x, y):
>    pass
>```
>
>This will run the test with the arguments set to `x=0/y=2`, `x=1/y=2`, `x=0/y=3`, and `x=1/y=3` exhausting parameters in the order of the decorators  
  
用例报错### █✔█1584897051215605761(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['B']**  
  
### 以下代码的输出结果为（ ）

```python
class OneDigitNumericValue():
    def __init__(self):
        self.value = 0

    def __get__(self, obj, type=None) -> object:
        return self.value

    def __set__(self, obj, value) -> None:
        self.value = value


class Foo:
    number = OneDigitNumericValue()


my_foo_object = Foo()
my_second_foo_object = Foo()
my_third_foo_object = Foo()

my_foo_object.number = 1
my_second_foo_object.number = 2
my_third_foo_object.number = 3

print(my_foo_object.number)
print(my_second_foo_object.number)
print(my_third_foo_object.number)
```  
  
3
3
3### █✔█2991122(单选)  
**rightAnswer: ['A']**  
**wrongAnswer: ['D']**  
  
### 在unittest框架中，如下哪个测试方法命名符合默认的命名约定（）  
  
abctest### █✔█1658281017115422722(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C']**  
  
### 已知'中'和'文'的UTF-8编码为 0xE4B8AD 和 0xE69687，以下哪个代码段能打印出字符串`中文`( )  
  
`print('\xe4\xb8\xad\xe6\x96\x87'.decode())`### █✔█3921593(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 如下程序的输出结果是（）
```python
args = (0, 1, 2, 3)
f = lambda *args: sum(args[::2])
print(f(1, 2, 3, 4))
```  
  
```
6
```### █✔█1584897049961508866(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
###  
```python
nums = [4, 1, 3, 2]
rev = reversed(nums)
print(sorted(rev), sorted(rev))
```
上面的这段代码的打印结果为（）  
  
`[] [1, 2, 3, 4]`### █✔█1584897050263498754(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: ['A']**  
  
### 下述哪个选项的代码**不**符合《华为Python语言编程规范》中“数据模型”章节的原则、要求和建议（ ）  
  
```python
print("Hello, %s" % name)
```### █✔█3621468(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: []**  
  
### 下面的程序执行过程中，类`AA`的`__init__`函数被调用了（ ）次

```python
class AA:
    def __init__(self):
        pass


class BB(AA):
    def __init__(self):
        AA.__init__(self)


class CC(AA):
    def __init__(self):
        AA.__init__(self)


class DD(BB, CC):
    def __init__(self):
        BB.__init__(self)
        CC.__init__(self)


dd = DD()
```  
  
4### █✔█3716754(单选)  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
### 以下执行SQL命令的代码均使用了外部数据，其中哪个符合《华为Python语言编程规范》中“外部数据校验”章节的原则、要求和建议（ ）  
  
```python
sql = "SELECT * FROM table WHERE id={0}".format(value)
connection.execute(sql)
```### █✔█3621499(单选)  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
### 下述哪个选项符合《华为Python语言编程规范》中“控制语句”这一章节中的要求和建议（ ）  
  
```python
def func(x):
    print(x)
    return x + 1  
```### █✔█3934552(单选)  
**rightAnswer: ['B']**  
**wrongAnswer: ['C']**  
  
### 如下程序的输出结果可能是（）

```python
dicts = {"a": 1, "b": 2, "c": 3}
results = {key.upper(): value for key, value in dicts.items()}
print(results)
```  
  
```
['a', 'b', 'c']
```
