- 👋 Hi, I’m @ZhangDaPao12138
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ZhangDaPao12138/ZhangDaPao12138 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
### ●●●1584897051316269057●●●  
**score: 2**  
**myAnswer: ['1584897056538177540']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 以下代码的运行结果是( )
```python
def func():
    yield (x for x in range(3))


for x in func():
    print(next(x))
```  
  
A: 1584897056538177538  
`(0, 1, 2)`  
B: 1584897056538177539  
0
1
2  
C: 1584897056538177540  
`0`  
D: 1584897056538177541  
`<generator object func.<locals>.<genexpr> at 0x000001F152299480>`（地址可能在不同运行环境中有所不同）  
### ○○○1584897050011840513○○○  
**score: 2**  
**myAnswer: ['1584897053858017284']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
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
  
A: 1584897053858017282  
```
[11, 22]
```  
B: 1584897053858017283  
```
[11, 22, 0, 1, 2, 3]
```  
C: 1584897053858017284  
```
[11, 22, 0, 1, 2, 3, 0, 1, 2, 3]
```  
D: 1584897053858017285  
产生异常  
### ○○○1584897049386889218○○○  
**score: 2**  
**myAnswer: ['1584897052616503299']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 执行以下代码的输出是( )
```python
d2 = datetime.datetime(5, 6, 7, 8, 9, 10)
print(d2.year, " Q", d2.month // 4 + 1, sep='')
```
**参考文档：**
>`datetime(year, month, day, hour=0, minute=0, second=0, microsecond=0, tzinfo=None, *, fold=0)`
The `year`, `month` and `day` arguments are required  
  
A: 1584897052612308993  
```10 Q2```  
B: 1584897052616503298  
```5 Q2```  
C: 1584897052616503299  
```5 Q3```  
D: 1584897052616503300  
```10 Q3```  
### ○○○1584894954063605762○○○  
**score: 2**  
**myAnswer: ['1584894964272541699']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 需求描述要清晰、需求可验收。小明看到以下关于设备数据采集功能相关的需求，请你帮忙审核下，需求满足清晰、 可验收标准的是（）  
  
A: 1584894964272541697  
设备支持温度、功耗等信息实时统计  
B: 1584894964272541698  
数据支持FTP协议传输  
C: 1584894964272541699  
支持新老特性兼容  
D: 1584894964272541700  
数据采集性能提升10%左右  
### ○○○1584894953145053186○○○  
**score: 2**  
**myAnswer: ['1584894962468990979']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 在一个文字处理软件的设计中，需要支持用户在编辑中的撤销和重做等动作，为了实现该功能，以下哪种设计模式最适合该功能的实现（ ）  
  
A: 1584894962468990977  
观察者模式（Observer Pattern）  
B: 1584894962468990978  
命令模式（Command Pattern）  
C: 1584894962468990979  
访问者模式（Visitor Pattern）  
D: 1584894962473185282  
享元模式（Flyweight Pattern)  
### ○○○1584894953052778497○○○  
**score: 2**  
**myAnswer: ['1584894962271858691']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 某个被测对象的因子取值情况如下表所示，当使用N-wise方法进行因子组合时，N=3时对应的测试用例个数是多少（）
因子a：3个取值
因子b：4个取值
因子c：5个取值
因子d：2个取值  
  
A: 1584894962267664385  
12  
B: 1584894962271858690  
24  
C: 1584894962271858691  
40  
D: 1584894962271858692  
60  
E: 1584894962276052993  
120  
### ○○○1584894952524296194○○○  
**score: 2**  
**myAnswer: ['1584894961143590914']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 针对以下成绩计算程序片段，满足“语句覆盖”的测试用例是（）
```c
if (score < 60) grade = "C";
else if (score < 80) grade = "B";
else if (score < 90) grade = "B+";
else grade = "A";
```  
  
A: 1584894961139396610  
(59,79,90,91)  
B: 1584894961139396611  
(60,61,89,90)  
C: 1584894961143590914  
(59,80,90,91)  
D: 1584894961143590915  
(59,79,89,90)  
### ○○○1579281042928508930○○○  
**score: 2**  
**myAnswer: ['1579281043452796932']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 以下哪项关于开源软件原生代码修改的说法不正确？  
  
A: 1579281043452796930  
不更改开源软件原生代码的数据结构，保持兼容性  
B: 1579281043452796931  
对开源软件原生代码进行修改区分管理，可以解决开源与自研代码耦合问题  
C: 1579281043452796932  
若对开源软件原生代码进行了修改，修改代码必须与原生代码区分管理  
D: 1579281043452796933  
对开源软件原生代码修改，建议尽量封装成函数或宏方式，提高扩展性  
### ○○○4006764○○○  
**score: 2**  
**myAnswer: ['11717251']**  
**rightAnswer: []**  
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
  
A: 11717249  
依恋情结（ Feature Envy）  
B: 11717250  
数据泥团（Data Clumps）  
C: 11717251  
中间人（Middle Man）  
D: 11717252  
狎昵关系（Inappropriate Intimacy）/内幕交易（Insider Trading）  
### ○○○3963500○○○  
**score: 2**  
**myAnswer: ['11718752']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
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
  
A: 11718750  
start
end
show  
B: 11718751  
start
show
end  
C: 11718752  
start
None
end  
D: 11718753  
start
end
None  
### ●●●3963492●●●  
**score: 2**  
**myAnswer: ['11717778']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 下列哪个选项符合《华为Python语言编程规范》中“类与面向对象”章节的原则、要求和建议（）  
  
A: 11717776  
```python
import sys


class Base:
    def __init__(self):
        self.running = False

    def start(self):
        self.running = True


class Addition(Base):
    def start(self, a, b):
        super().start()
        result = a + b
        sys.stdout.write(str(result))
```  
B: 11717777  
```python
import sys


class Base:
    def __init__(self):
        self.running = False

    def start(self, *args):
        self.running = True


class Addition(Base):
    def __init__(self):
        self.running = False

    def start(self, *args):
        super().start(*args)
        result = sum(*args)
        sys.stdout.write(str(result))
```  
C: 11717778  
```python
import sys


class Base:
    def __init__(self):
        self.running = False

    def start(self, *args):
        self.running = True


class Addition(Base):
    def start(self, *args):
        super().start(*args)
        result = sum(*args)
        sys.stdout.write(str(result))
```  
D: 11717779  
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
```  
### ○○○3949573○○○  
**score: 2**  
**myAnswer: ['11542209']**  
**rightAnswer: []**  
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
  
A: 11542207  
D档状态下的“左旋”转移（Transition）中不需要检查车辆行驶状态，应该删除监护条件（Guard conditions）限制  
B: 11542208  
D档状态下的`“右旋”`转移（Transition）中不需要检查车辆行驶状态，应该删除监护条件（Guard conditions）限制  
C: 11542209  
N档状态下的“左旋”转移（Transition）中不需要检查车辆行驶状态，应该删除监护条件（Guard conditions）限制  
D: 11542210  
N档状态下的`“按下P按键”`转移（Transition）中不需要检查车辆行驶状态，应该删除监护条件（Guard conditions）限制  
### ●●●3934704●●●  
**score: 2**  
**myAnswer: ['11487134']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“运算符”章节的原则、要求和建议（ ）  
  
A: 11487132  
比较两个list内容是否相同：
```python
if list1 is list2:
```  
B: 11487133  
比较两个时间是否相等：
```python
if time1 is time2:
```  
C: 11487134  
比较两个tuple的内容是否相同：
```python
if tuple1 == tuple2:
```  
D: 11487135  
判断tuple内容是否为空：
```python
if my_tuple is ():
```  
### ○○○3887735○○○  
**score: 2**  
**myAnswer: ['11335951']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 以下代码的运行结果是( )
```python
def func():
    yield (x for x in range(3))


for x in func():
    print(tuple(x))
```  
  
A: 11335949  
`(0, 1, 2)`  
B: 11335950  
0
1
2  
C: 11335951  
`0`  
D: 11335952  
`<generator object func.<locals>.<genexpr> at 0x000001F152299480>`（地址可能在不同运行环境中有所不同）  
### ○○○3887342○○○  
**score: 2**  
**myAnswer: ['11487600']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 关于下面的代码的输出，正确的是：
```python
language = u"中文"
print(len(language), hasattr(language, "encode"))
```
  
  
A: 11487598  
`2 True`  
B: 11487599  
`4 True`  
C: 11487600  
`2 False`  
D: 11487601  
`4 False`  
### ●●●3862596●●●  
**score: 2**  
**myAnswer: ['11550356']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 以下代码的输出结果是（ ）
```python
def func(a, *b):
    for item in b:
        a += item
    return a


m = 0
print(func(m, 1, 1))
```  
  
A: 11550354  
0  
B: 11550355  
1  
C: 11550356  
2  
D: 11550357  
产生异常  
### ●●●3817397●●●  
**score: 2**  
**myAnswer: ['11118765']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
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
  
A: 11118763  
hello python  
B: 11118764  
hello world  
C: 11118765  
AttributeError: 'function' object has no attribute 'test_2  
D: 11118766  
AttributeError: module 'tests' has no attribute 'test2  
### ●●●3817392●●●  
**score: 2**  
**myAnswer: ['11118692']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 关于以下代码，说法正确的是（）

```python
class A:
    a = 42
    b = list(a + i for i in range(10))
    print(b)


A()
```  
  
A: 11118690  
代码输出为`[42, 43, 44, 45, 46, 47, 48, 49, 50, 51]`  
B: 11118691  
代码输出为`[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]`  
C: 11118692  
代码无法执行，存在语法错误，变量`a`未定义  
D: 11118693  
代码能正常执行，但是没有任何输出  
### ●●●3817384●●●  
**score: 2**  
**myAnswer: ['11118555']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 以下代码的执行结果为（）

```python
a = [0, 1, 2, 3]
for a[-1] in a:
    print(a[-1])
```  
  
A: 11118553  
抛出异常  
B: 11118554  
`0 1 2 3`  
C: 11118555  
`0 1 2 2`  
D: 11118556  
`0 1 2`  
### ○○○3816402○○○  
**score: 2**  
**myAnswer: ['11436250']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“函数与方法”章节的要求和建议（）  
  
A: 11436248  
```python
def division(x, y):
    if y != 0:
        print(x / y)


result = division(1, 2)
```  
B: 11436249  
```python
def division(x, y):
    if abs(y) > 1e-5:
        print(x / y)


result = division(1, 2)
```  
C: 11436250  
```python
def division(x, y):
    try:
        print(x / y)
    except ZeroDivisionError:
        print('除数不能为0')


result = division(1, 2)
```  
D: 11436251  
```python
def division(x, y):
    if y != 0:
        print(x / y)


division(1, 2)
```  
### ○○○3717462○○○  
**score: 2**  
**myAnswer: ['11487677']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“变量作用域”章节的要求和建议（）  
  
A: 11487675  
```python
def func():
    global acc
    acc = 2


func()
print(acc)
```  
B: 11487676  
```python
_acc = 1


def func():
    print(_acc)


func()
```  
C: 11487677  
```python
_acc = 1


def func():
    global _acc
    print(_acc)


func()
```  
D: 11487678  
```python
_acc = 1


def func():
    global _acc
    _acc = "None"


func()
print(_acc)
```  
### ○○○3717458○○○  
**score: 2**  
**myAnswer: ['11550485']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
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
  
A: 11550483  
True
True  
B: 11550484  
True
False  
C: 11550485  
False
True
  
D: 11550486  
False
False  
### ○○○3678138○○○  
**score: 2**  
**myAnswer: ['11426957']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
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
  
  
A: 11426955  
装饰者(Decorator)模式  
B: 11426956  
职责链(Chain of Responsibility)模式  
C: 11426957  
策略(Strategy)模式  
D: 11426958  
状态(State)模式  
### ●●●3667100●●●  
**score: 2**  
**myAnswer: ['11438067']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 以下代码会输出什么( )
`print(int("1" + "2") + 2)`  
  
A: 11438065  
报错  
B: 11438066  
`5`  
C: 11438067  
`14`  
D: 11438068  
`32`  
### ○○○3667090○○○  
**score: 2**  
**myAnswer: ['11550284']**  
**rightAnswer: []**  
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
  
A: 11550202  
```
B's __new__() invoked
A's __new__() invoked
A's __init__() invoked
```  
B: 11550283  
```
B's __new__() invoked
B's __init__() invoked
A's __new__() invoked
A's __init__() invoked
```  
C: 11550284  
```
B's __init__() invoked
B's __new__() invoked
A's __init__() invoked
A's __new__() invoked
```  
D: 11550285  
```
B's __new__() invoked
B's __init__() invoked
A's __new__() invoked
```  
### ○○○3661663○○○  
**score: 2**  
**myAnswer: ['11059762']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 下述哪个选项符合《华为Python语言编程规范》中“控制语句”章节的要求和建议（ ）  
  
A: 11059760  
```python
def func(x):
    if x > 0:
        return x,True
    elif x < 0:
        return x
    else:
        print("error")
```  
B: 11059761  
```python
def fn(x):
    for i in range(x):
        if i > 4:
            return i
    else:
        print("{} is not greater than 4".format(x))
        return 0
```  
C: 11059762  
```python
def func(a):
    if a:
        return a
    else:
        raise Exception("invalid value")
        do_something_else() 
```  
D: 11059763  
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
```  
### ○○○3658966○○○  
**score: 2**  
**myAnswer: ['11498094']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 假设有个算法的输入对象是两个名为S_Op和S_Num的栈，
算法的执行过程如下：
如果满足条件 “S_Num中元素个数大于等于2”且“S_Op中元素个数大于等于1”，则循环依次执行下面的操作步骤
    1、从 S_Num 中弹出1个操作数 a 
    2、从 S_Num 中弹出1个操作数 b
    3、从 S_Op 中弹出一个运算符 op
    4、将 a op b 的结果压入 S_Num
上述流程结束后S_Num栈顶的元素值就是算法的输出值。
则下面哪个S_Op和S_Num栈（左边栈底，右边栈顶）应用上述算法之后其值不等于24？（）  
  
A: 11498092  
S_Op  : *
S_Num : 24 1  
B: 11498093  
S_Op  : /
S_Num : 24 1  
C: 11498094  
S_Op  : / * - + 
S_Num : 2 4 6 8 10  
D: 11498095  
S_Op  : + +
S_Num : 2 4 6 8 10  
### ○○○3658962○○○  
**score: 2**  
**myAnswer: ['11497725']**  
**rightAnswer: []**  
**wrongAnswer: ['D']**  
  
  
### 下列关于软件开发和软件测试说法正确的是（）  
  
A: 11497722  
软件测试就是发现所有错误  
B: 11497723  
编码时尽可能多使用全局变量  
C: 11497724  
尽可能使用高级语言编写程序  
D: 11497725  
系统测试的主要方法是白盒法  
### ○○○3658961○○○  
**score: 2**  
**myAnswer: ['11497188']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 在进行二进制文件差异分析时，需要分析差异产生的根因，并尝试制定差异消除方案。对于引入原因明确但无法消除，且容易验证的差异，被定义为可解释差异。下列哪个选项不属于可解释差异（）  
  
A: 11497186  
签名文件  
B: 11497187  
校验和文件  
C: 11497188  
文档类文件  
D: 11497189  
ini文件  
### ●●●3658959●●●  
**score: 2**  
**myAnswer: ['11497924']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 给定一个数组A[N]，每一项都是长度为M的字符串。假设这些N个字符串已经按照字典顺序在A[N]中排序。如果使用二分查找法在A[N]中查找某一个字符串时（如果有多个匹配，在找到第一个成功的就结束），下述哪一个是对应算法的最坏时间复杂度？（）  
  
A: 11497922  
O(Log(N))  
B: 11497923  
O(Log(M))  
C: 11497924  
O(M*Log(N))  
D: 11497925  
O(N*Log(M)  
### ○○○3621568○○○  
**score: 2**  
**myAnswer: ['11550005']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### data是来自外部的数据，PyYAML是最新版本，下列反序列化操作中，不符合《华为Python语言编程规范》的是（）  
  
A: 11550003  
`yaml.load(data)`
  
B: 11550004  
`yaml.load_all(data, Loader=SafeLoader)`
  
C: 11550005  
`yaml.safe_load(data)`
  
D: 11550006  
`yaml.safe_load_all(data)`
  
### ●●●3621563●●●  
**score: 2**  
**myAnswer: ['11550364']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 以下哪个选项符合《华为Python语言编程规范》中“异常处理”章节的要求和建议（）  
  
A: 11550362  
```python
try:
    do_something()
except SomeException:
    raise
except Exception as e:
    do_something(e)
```  
B: 11550363  
```python
def control_statement_in_finally(param):
    ret = -1
    try:
        ret = 1 / param
    finally:
        return ret  
```  
C: 11550364  
```python
def control_statement_in_finally(param):
    ret = -1
    try:
        ret = 1 / param
    except ZeroDivisionError:
        do_something()
    finally:
        do_finally()
    return ret
```  
D: 11550365  
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
```  
### ○○○3621516○○○  
**score: 2**  
**myAnswer: ['11436113']**  
**rightAnswer: []**  
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
  
A: 11436111  
```
 Cannot create a consistent method resolution order (MRO) for bases GrandParent, Parent
```  
B: 11436112  
```
Hello GrandParent
Hello GrandParent
Hello GrandParent
Hello Parent
Hello Child
```  
C: 11436113  
```
Hello GrandParent
Hello Parent
Hello Child
```  
D: 11436114  
```
Hello GrandParent
Hello GrandParent
Hello Parent
Hello Child
```  
### ○○○3621506○○○  
**score: 2**  
**myAnswer: ['11550517']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### entities中的对象，只会被顺序遍历一次，且不需要长期持有，下列代码符合《华为Python语言编程规范》中“性能与资源管理”章节的原则、要求与建议的是（）
```python
class Entity:
    def __init__(self, eid = 0):
        self.__eid = eid
```  
  
A: 11550515  
```python
entities = [Entity(i) for i in range(1000)]
```  
B: 11550516  
```python
entities = (Entity(i) for i in range(1000))
```  
C: 11550517  
```python
entities = []
for i in range(1000):
    entities.append(Entity(i))
```  
D: 11550518  
```python
entities = [None] * 1000
for i in range(1000):
    entities.append(Entity(i))
```  
### ○○○3621504○○○  
**score: 2**  
**myAnswer: ['11550509']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 下述哪个选项的代码符合《华为Python语言编程规范》中“函数与方法”章节的要求和建议（）  
  
A: 11550507  
```python
def fun(arg_0, arg_1='', arg_2=[]):
    arg_2.append(arg_0)
    arg_2.append(arg_1)
    print(arg_2)
```  
B: 11550508  
```python
def fun(arg_0, arg_1='', arg_2=None):
    arg_2 = [] if arg_2 is None else arg_2
    arg_2.append(arg_0)
    arg_2.append(arg_1)
    print(arg_2)
```  
C: 11550509  
```python
def fun(arg_0, arg_1='', arg_2={}):
    arg_2.update({"arg_0": arg_0})
    arg_2.update({"arg_1": arg_1})
    print(arg_2)
```  
D: 11550510  
```python
def fun(arg_0, arg_1='', arg_2=set()):
    arg_2.add(arg_0)
    arg_2.add(arg_1)
    print(arg_2)
```  
### ○○○3621495○○○  
**score: 2**  
**myAnswer: ['11487653']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 关于用pdb设置断点，下列说法正确的是?  
  
A: 11487651  
一行只能设置一个断点  
B: 11487652  
断点可以设置在空行和注释行，其效果等价于设置在其上一行代码处  
C: 11487653  
只能为当前已经被加载的文件设置断点  
D: 11487654  
可以在import语句行设置断点  
### ○○○3621459○○○  
**score: 2**  
**myAnswer: ['11438039']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 虚拟环境管理工具tox可用于对将要发布的python库文件进行多版本环境下的兼容测试。配置文件tox.ini有这样的内容: 
```python
[tox]
envlist = {py36,py27}-django15
```
对它的含义理解，如下描述中正确的是？（）  
  
A: 11438037  
tox运行两个环境下的测试：py27-django15环境的python版本只能是python 2.7，py36-django15的python版本只能是python 3.6  
B: 11438038  
tox运行一个测试环境：该环境python基础版本为3.6或2.7  
C: 11438039  
tox运行一个测试环境：该环境同时有2.6和3.7版本的python  
D: 11438040  
tox运行两个环境下的测试：py27-django15和py36-django15。如果后面配置了basepython字段，环境的python版本由basepython指定；否则，由环境名中的pyxx来决定  
### ○○○3621455○○○  
**score: 2**  
**myAnswer: ['11550304']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 在一个8核心CPU的机器上运行仅使用了threading库的Python程序（假定使用CPython，并且除了threading库以外未调用其他任何库），则此程序中同一时刻最多有几个线程在执行()  
  
A: 11550302  
1  
B: 11550303  
2  
C: 11550304  
4  
D: 11550305  
8  
### ●●●3582828●●●  
**score: 2**  
**myAnswer: ['11369846']**  
**rightAnswer: ['D']**  
**wrongAnswer: []**  
  
  
### 根据《身份和访问管理安全设计规范》，以下哪种场景不应该产生安全告警（ ）  
  
A: 11369843  
连续登录认证失败达到系统设定的次数  
B: 11369844  
敏感功能的开启，比如端口镜像  
C: 11369845  
身份认证凭证即将过期或已过期  
D: 11369846  
业务模块加载失败  
### ○○○3582821○○○  
**score: 2**  
**myAnswer: ['11296502']**  
**rightAnswer: []**  
**wrongAnswer: ['A']**  
  
  
### 在一个简化的虚拟农场游戏中， 对于农场（Farm）的设计需要满足产品多样性和灵活生产的诉求：农场可以养动物（Animal），如养马（A_Horse）、养牛（A_Cattle）等；还可以培养植物（Plant），如种菜（P_Vegetables）、种水果（P_Fruitage）等；为了简化设计，假设要求每个农场都要生产一种动物和一种植物，不同的农场生产不同的动植物，若采用抽象工厂 模式（Abstract Factory Pattern）来设计，以下模型图中能正确表达这一设计模式的是(  )  
  
A: 11296502  
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/10dd700f-a80a-4db3-8b3e-276b9a3a6563.png" alt="" />  
B: 11296503  
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/f249fae5-cdcc-45a6-b7dd-7352a87290c0.png" alt="" />  
C: 11296504  
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/cbd99172-685d-4b2f-8891-f2e709f28bab.png" alt="" />  
D: 11296505  
<img src="https://proxy.ilearning.huawei.com/edxs3proxy/ilearningexam1/9db04570-79cb-49d3-b6e8-2ed6694ec09b.png" alt="" />  
### ○○○3249797○○○  
**score: 2**  
**myAnswer: ['11497372']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 两台设备间需要通过外部网络传输和协商秘钥信息，为了防止传输过程中信息被攻击者篡改，下面哪个方法可以识别出信息被篡改：  
  
A: 11497370  
使用CRC32校验  
B: 11497371  
使用SHA512校验  
C: 11497372  
使用ASE256进行加密保护  
D: 11497373  
使用TLS协议来传输信息  
### ●●●3249796●●●  
**score: 2**  
**myAnswer: ['11497293']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 基于《密码算法应用规范》,下列哪种随机数生成方式自身会出现安全漏洞？  
  
A: 11497291  
Linux操作系统的/dev/random设备接口  
B: 11497292  
OpenSSL1.1.X的RAND_priv_bytes  
C: 11497293  
NIST SP 800-90A标准中的DualEC-DRBG生成器  
D: 11497294  
JDK的java.security.SecureRandom  
### ●●●3133572●●●  
**score: 2**  
**myAnswer: ['11426937']**  
**rightAnswer: ['C']**  
**wrongAnswer: []**  
  
  
### 某系统在启动时会一次性读取配置文件信息，并将其存储在类型为Configuration(类名)的对象中供其他模块使用。在这个场景下，以下做法正确的是（ ）  
  
A: 11426935  
将生成器(Builder)模式应用于Configuration  
B: 11426936  
将抽象工厂(Abstract Factory)模式应用于Configuration  
C: 11426937  
将单件/单例(Singleton)模式应用于Configuration  
D: 11426938  
将备忘录(Memento)模式应用于Configuration  
### ○○○2974541○○○  
**score: 2**  
**myAnswer: ['11508352']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### SQL注入是指后台数据库对用户输入数据的合法性没有判断或过滤不严，攻击者可以在web页面中插入额外的SQL语句，实现对后台数据库的非法访问操作。以下关于SQL Injection（SQL注入）的说法错误的是哪个？  
  
A: 11508350  
SQL Injection 安全漏洞可以攻击系统数据库，篡改数据库数据和获取未授权的信息。  
B: 11508351  
SQL Injection可以通过危及客户端安全，来盗取用户个人敏感数据。  
C: 11508352  
SQL Injection 主要是来自用户或者外界的非信任源的数据在进行SQL查询时，没有过滤或者过滤不完备，外部字符串包含特定字符，改变了原本语句的查询本意。  
D: 11508353  
SQL Injection 安全漏洞可以通过安全的输入校验机制来预防。  
### ○○○2952955○○○  
**score: 2**  
**myAnswer: ['10851493']**  
**rightAnswer: []**  
**wrongAnswer: ['C']**  
  
  
### 某公司欲开发一个软件系统的在线文档帮助系统，用户可以在任何一个查询上下文中输入查询关键字，如果当前查询环境下没有相关内容，则系统会将查询按照一定的顺序转发给其他查询环境。基于上述需求，采用下面哪种模式最为合适？（ ）  
  
A: 10851491  
职责链(Chain of Responsibility)模式  
B: 10851492  
桥接(Bridge)模式  
C: 10851493  
装饰(Decorator)模式  
D: 10851494  
适配器(Adapter)模式  
### ○○○1584900965881163777○○○  
**score: 3**  
**myAnswer: ['1584900973326053378', '1584900973326053379', '1584900973326053380']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 每一种UML建模图都对应有各自不同的核心建模元素，其中顺序图（Sequence Diagram）的关键建模元素有哪些（  ）  
  
A: 1584900973321859074  
控制流（Control Flow）  
B: 1584900973326053378  
对象/角色（Object/Role）  
C: 1584900973326053379  
状态（State）  
D: 1584900973326053380  
消息（Message）  
### ●●●1584894954608865281●●●  
**score: 3**  
**myAnswer: ['1584894965405003777', '1584894965405003778', '1584894965405003779']**  
**rightAnswer: ['BCD']**  
**wrongAnswer: []**  
  
  
### 小A对一个已有测试用例的模块代码进行重构，在重构代码的过程中，发现原有功能的一个BUG，为了方便，未提交已重构部分代码，直接顺手修改BUG，在保证已有测试用例都通过的前提下，一次性提交上库。后续对此BUG进行测试时发现修改方案并不完善，仍有问题，于是小A回退了所有重构和修改BUG部分的代码。请问在小A的重构过程中存在哪些问题（）  
  
A: 1584894965400809474  
不应在测试用例覆盖可能存在遗漏的情况下对代码进行重构  
B: 1584894965405003777  
重构时将重构工作和BUG修改工作混做  
C: 1584894965405003778  
对识别到的BUG的修改没有先建立测试用例，再实施修改  
D: 1584894965405003779  
重构没有小步提交  
### ○○○1584894952679485442○○○  
**score: 3**  
**myAnswer: ['1584894961474940929', '1584894961474940930', '1584894961474940931']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 如果输入条件规定了整型参数的范围及默认值，只用边界值分析方法，如下哪些可以作为测试数据（）  
  
A: 1584894961470746626  
最大值和最小值  
B: 1584894961474940929  
最小值减1  
C: 1584894961474940930  
最大值加1  
D: 1584894961474940931  
默认值  
### ○○○3734850○○○  
**score: 3**  
**myAnswer: ['11437978', '11437979', '11437980']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### ```python
class B():
    def __init__(self):
        print('B')


class A(B):
    def __init__(self):
        ____________ # 需填入代码


a = A()
```
以下哪些选项中的代码单独填入到横线处，可以使得以上代码段输出`B`？（ ）  
  
A: 11437977  
`super().__init__()`  
B: 11437978  
`super().__init__(self)`  
C: 11437979  
`B.__init__()`  
D: 11437980  
`B.__init__(self)`  
### ●●●3717452●●●  
**score: 3**  
**myAnswer: ['10812232', '10812233', '10812234']**  
**rightAnswer: ['BCD']**  
**wrongAnswer: []**  
  
  
### 已知：` x = [4, 1, 0, 3, 5]`， 下面哪些表达式操作可以将 `x`转变为` [4, 1, 3, 5]`（）  
  
A: 10812231  
`x[2] = []`  
B: 10812232  
`del x[2]`  
C: 10812233  
`x.remove(0)`  
D: 10812234  
`x[2:3] = []`  
### ○○○3717104○○○  
**score: 3**  
**myAnswer: ['11550419', '11550420', '11550421']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 如下表达式的值为`False`的有()  
  
A: 11550418  
`{3, 5, 4} < {4, 3, 5}`  
B: 11550419  
`{5, 3} < {4, 3, 5}`  
C: 11550420  
`{3, 5, 4} > {4, 3, 5}`  
D: 11550421  
`{3, 5, 6} > {4, 3, 5}`  
### ○○○3667106○○○  
**score: 3**  
**myAnswer: ['11118491', '11118492', '11118493']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 以下哪些变量定义语句执行时会产生异常？（ ）  
  
A: 11118490  
`a = 100, 200, 300`  
B: 11118491  
`a = b = c = 10`  
C: 11118492  
`a, b = 100, 300, 500`  
D: 11118493  
`a = 10 20`  
### ○○○3667098○○○  
**score: 3**  
**myAnswer: ['10666003', '10666004', '10666005']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 下列哪些选项符合《华为Python语言编程规范》中“类与面向对象”章节的原则、要求和建议（）  
  
A: 10666002  
```python
class Summation:
    def __init__(self, base):
        self._base = base

    def add(self, a: int):
        self._base += a
```  
B: 10666003  
```python
class Addition:
    def add(self, a: int, b: int) -> int:
        return a + b
```  
C: 10666004  
```python
class Addition:
    @staticmethod
    def add(a: int, b: int) -> int:
        return a + b
```  
D: 10666005  
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
### ○○○3666975○○○  
**score: 3**  
**myAnswer: ['11436035', '11436036', '11436037']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 如下代码中的命名，符合华为Python编程规范建议的有（ ）  
  
A: 11436034  
```python
def chooseABook():
    pass
```  
B: 11436035  
```python
class SampleClass(Enum):
    pass
```  
C: 11436036  
```python
CONSTANT_FLOAT_PI = 3.1415
```  
D: 11436037  
```python
def i(l, o):
    pass
```  
### ○○○3621579○○○  
**score: 3**  
**myAnswer: ['11436007', '11436008', '11436009']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
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
  
A: 11436006  
`get_type`函数中的`global`的使用违反规范  
B: 11436007  
`set_type`函数中的`type`参数命名违反规范  
C: 11436008  
`set_type`函数中的`_g_type`的命名违反规范  
D: 11436009  
全局变量`_g_type`的命名违反规范，模块内使用的全局变量不能以下划线开头  
### ●●●3621560●●●  
**score: 3**  
**myAnswer: ['11549956', '11549957', '11549958']**  
**rightAnswer: ['BCD']**  
**wrongAnswer: []**  
  
  
### 在linux环境中，为了能够`import`在`/my_path`路径下的包(package)，以下做法不符合《华为Python语言编程规范》中“标准库”章节的要求和建议的有（）  
  
A: 11549955  
运行代码前，在bash中执行`export PYTHONPATH=$PYTHONPATH:/my_path`  
B: 11549956  
在代码中添加
```python
sys.path.insert(0, './')
sys.path.insert(0, './my_path')
```  
C: 11549957  
在代码中添加`sys.path = ['/my_path']`  
D: 11549958  
在代码中添加`sys.path.insert(0, '/my_path')`  
### ●●●3621464●●●  
**score: 3**  
**myAnswer: ['11305531', '11305532', '11305533']**  
**rightAnswer: ['BCD']**  
**wrongAnswer: []**  
  
  
### 以下哪些选项符合《华为Python语言编程规范》中“异常处理”章节的要求和建议（）  
  
A: 11305530  
```python
# 自定义的异常类
class AuthenticationError(BaseException):
    def __init__(self, message=None):
        super(AuthenticationError, self).__init__(message)
        self.http_code = 404
```  
B: 11305531  
```python
# 自定义的异常类
class AuthenticationError(Exception):
    def __init__(self, message=None):
        super(AuthenticationError, self).__init__(message)
        self.http_code = 404
```  
C: 11305532  
```python
try:
    with open(file_name) as fd:
        ...
except OSError as e:
    raise UserDefined.InvalidFile('Please check file name') from e
```  
D: 11305533  
```python
try:
    with open(file_name) as fd:
        content = fd.read()
except FileNotFoundError as e:
    do_something(file_name, e)
except UnicodeDecodeError as e:
    do_otherthing(file_name, e)
```  
### ○○○3211135○○○  
**score: 3**  
**myAnswer: ['11496997', '11496998', '11496999']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 下面哪些行为是华为开源软件使用规范明确禁止的？  
  
A: 11496996  
通过开源软件中心仓commit形式管理对开源原生代码的修改  
B: 11496997  
片段引用  
C: 11496998  
开源软件确认为自研  
D: 11496999  
开源代码和自研代码目录隔离  
### ○○○1584900964601901058○○○  
**score: 3**  
**myAnswer: ['1584900971002408961', '1584900971002408962', '1584900971002408963']**  
**rightAnswer: []**  
**wrongAnswer: ['BCD']**  
  
  
### 安全应用的“linux安全设计”原则中，下述描述正确的有（）  
  
A: 1584900970998214658  
对系统中的文件存取，要严格限制重要文件的存取，防止未被授权用户访问  
B: 1584900971002408961  
对系统访问要进行严格限制，如：对允许登录用户的登录尝试次数，要进行限制  
C: 1584900971002408962  
对系统补丁，因为业务不需要，所以，不需要定期安装  
D: 1584900971002408963  
只给用户分配足够其完成任务的最小权限  
### ●●●2928344●●●  
**score: 3**  
**myAnswer: ['11436267', '11436268', '11436270']**  
**rightAnswer: ['ABD']**  
**wrongAnswer: []**  
  
  
### 针对重构方法，下列说法错误的有（）  
  
A: 11436267  
提取接口（Extract Interface）和提取超类（Extract Superclass）均可提取共通代码  
B: 11436268  
隐藏委托关系（Hide Delegate）会使代码层次更清晰，因此委托类的功能越多越好  
C: 11436269  
当发现某个子类并未带来该有的派生价值时，可以考虑使用移除子类（Remove Subclass）手法进行重构  
D: 11436270  
将值域上移到父类（即字段上移 Pull Up Field）会有效减少子类的成员变量，只需要搬移值域，不需要搬移对该值域的操作方法  
