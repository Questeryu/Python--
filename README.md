# Python 从入门到放弃

申明：本文档是结合网络MOOC教学及《Python入门到实践》及官方文档学习的学习笔记！作为一个非专业程序员，可能不入大咖法眼，为什么还要去写，学习这个呢？为什么要去学习编程呢？

> ①感谢前期开发的牛人，尽然开发出这么好的东西，使得信息传播
>
> ②人类早期出行还在使用马车的时候，慢慢的随着工业革命的爆发，蒸汽机的出现使得马车的市场缩小，再后来内燃机的出现，出现最让人羡慕又赚钱的技能——驾驶，后来互联网时代的到来，无人驾驶的出现，之前的职业岗位被替换掉，又繁衍出一些新的岗位，试想一想以前的马车这个行业还有多少，再后来，驾驶也变成了一项生活的必要技能，也许N年以后这个岗位再慢慢的消失。
>
> ​	这个社会也同样遵循着“物竞天择，适者生存”的法则，因此一些占用资源而不健康的公司迟早会被淘汰，取而代之的是那些推动人类进步的公司，他们才配享有更多的资源
>
> ③在我们现在这个时代，人工智能的出现，显然最重要的不是算法，那是什么呢？数据（Data），为什么是数据呢？因为无论是人工智能还是机器学习都需要用大量的数据去喂它。
>
> ④这个世界对很多不进步的人（不健康的公司）来说的很残忍的，其实是越来残忍，我见过和我一同毕业的同龄人早早的就停止了进步，现在来看早已经被时代甩在了身后； 生活太安逸，不愿意跳出自己的舒适圈，也许是人类基因所决定。宁愿吃生活中的苦，也不愿意吃学习上面的苦。求其本质：生活中的苦是被动吃的，而学习中的苦是要主动吃的！归根结底：没有自学能力，
>
> ​	因此我不得不去自学，其二，编程也是自己兴趣使然

首先题目为什么是从入门到放弃，有2种解释：

> ①你会使用这个工具（tool），而且是把它当作一种潜意识，你不会可以去记它，真正的做到了内化，就如走路，呼吸，心跳。
> ②你学过了，隐隐约约记得，后来感觉太难了，因此我们又回到了我们的主题

​		我希望我们做第一种人！
当你学完之后发现，它还是一个工具，你要学的很多，统计学、数学、网络方面的原理；当你早期的思维是错误的时候，在以后的时间的它会呈复利的增长，所以发现自己的错误，面对=>改善。
感谢我遇到那些改变我思维（想法）的人。ありがとう。哈哈，明年准备去日本，因此等把这个内化之后，我就去盘日语和英语（you can teach me)，然后去环游世界 哈哈哈（起飞失败，疫情影响）

## print()函数 

​		在这里这些可能不懂，后面你会用到的，先学哇，就像我不知道，学这个有什么用，但我还是去学了。我知道我这样很很难说服一些人，纸上读来终觉浅，绝知此事要躬行。后来无意间在计算股票的时候我竟然神奇般的使用上了它。如果你看不懂不要紧，你可以参考网上的资源，自学就是这个样子的 本人非程序员，直接盘它就OK了

### 设置指定位置，可以多次使用


```python
#设置指定位置，可以多次使用
print("{0} {1} {0}".format("hello","or"))
#使用列表格式化
person = {"name":"opcai","age":20}
print("My name is {name} . I am {age} years old .".format(**person))
```

    hello or hello
    My name is opcai . I am 20 years old .


###  通过列表格式化


```python
#通过列表格式化
stu = ["opcai","linux","MySQL","Python"]
print("My name is {0[0]} , I love {0[1]} !".format(stu))

```

### 数字格式化  and 输出大括号
#数字格式化

#数字 格式 输出 描述
 3.1415926 {:.2f} 3.14 =====>保留小数点后两位
3.1415926 {:+.2f} +3.14 =====>带符号保留小数点后两位
-1 {:+.2f} -1.00 =====>带符号保留小数点后两位
2.71828 {:.0f} 3 =====>不带小数
5 {:0>2d} 05 =====>数字补零 (填充左边, 宽度为2)
5 {:x<4d} 5xxx =====>数字补x (填充右边, 宽度为4)
10 {:x<4d} 10xx =====>数字补x (填充右边, 宽度为4)
1000000 {:,} 1,000,000 =====>以逗号分隔的数字格式
0.25 {:.2%} 25.00% =====>百分比格式
1000000000 {:.2e} 1.00e+09 =====>指数记法
13 {:10d} 13 =====>右对齐 (默认, 宽度为10)
13 {:<10d} 13 =====>左对齐 (宽度为10)
13 {:^10d} 13 =====>中间对齐 (宽度为10)

-------------------输出大括号-------------------
print("{} {{0}}".format("opcai_linux"))首先我们从布尔指令入手吧
关于布尔值的介绍 给你们介绍一个“狠人” 乔治 布尔
逻辑关系应该能用符号表示。
这个等等再说
## 程序安装


```python
#这个不写了 自己去研究，百度一下你就知道，如果你连这个搞不定，那你就不要搞了，决定去做一件事情很难，
#而把这件事情坚持下去又是一个层次
#当然这里不是就是让你去学什么，因为这个和我关系不大
```

# 变量和简单数据类型

## 变量 


```python
message = "Hello Python world!"
print(message) #其中message就是变量
```

    Hello Python world!


## 字符串


```python
"this is string"
```




    'this is also string'




```python
'this is also string'
```




    'this is also string'



### 使用方法修改字符串的大小写


```python
name="questeryu"
print(name.title())
#title 是将字符中的首字母进行大写
```

    Questeryu

在这个示例中，小写的字符串"questeryu"存储到了变量name中。在print()语句中，方法
title()出现在这个变量的后面。方法是Python可对数据执行的操作。在name.title()中，name后
面的句点（.）让Python对变量name执行方法title()指定的操作。每个方法后面都跟着一对括号，
这是因为方法通常需要额外的信息来完成其工作。这种信息是在括号内提供的。函数title()不
需要额外的信息，因此它后面的括号是空的。
title()以首字母大写的方式显示每个单词，即将每个单词的首字母都改为大写。这很有用，
因为你经常需要将名字视为信息。例如，你可能希望程序将值Ada、ADA和ada视为同一个名字，
并将它们都显示为Ada。

```python
#还有如下操作
print(name.upper()) #字母全部大写
a=name.upper()
print(a)
print (a.lower()) #字母全部小写
```

    QUESTERYU
    QUESTERYU
    questeryu


### 合并（拼接）字符串


```python
first_name="Quester"
last_name="yu"
full_name=first_name+" "+last_name
print(full_name)
```

    Quester yu



```python
#展示用+表示字符串的链接
print("hello "+full_name+"!")
```

    hello Quester yu!



```python
#还有可以用乘法来运算
x="3 "
print(x*3)  #可以看到输出3个3
```

    3 3 3 


### 删除空白字符串中的空格（rstrip(尾部),lstrip(首部),strip(首尾))


```python
#可以剔除字符串开头的空白，或同时剔除字符串两端的空白。为此，可分别使用方法lstrip()：和strip()：
a= "   python  "
print(len(a))#a字符串的长度 长度为“12”；
print(a.rstrip())#删除尾部空格 output："   python“
print(len(a.rstrip())) #删除尾部空格后，字符串的长度 长度为：“9”；

print(a.lstrip())#删除字符串开头的空格  output："python   "
print(len(a.lstrip())) #删除字符串开头的空格 字符串的长度 长度为：“8”
print(a.strip())# #删除字符串首尾空格
print(len(a.strip()))#输出字符长长度
#总结：rstrip()删除
```

    11
       python
    9
    python  
    8
    python
    6


## 数字 （这个就比较简单了，还有运算，小学二年级）


```python
#在Python中，可对整数执行加（+）减（-）乘（*）除（/）运算。
#比如计算1+1等于几这个无聊的问题，听说有人为了证明1+1=2专门还写了一本书：
a=1+1
b=3+4
c=a*b
d=a**b #表示a的b次方
print(a,b,d,sep="\n")
#还有四则混合运算 其实是和数学是一样一样的 三角函数、逻辑 and or not 、布尔值：True and Flase
```

    2
    7
    128


##  浮点数


```python
'''Python将带小数点的数字都称为浮点数。大多数编程语言都使用了这个术语，它指出了这样
一个事实：小数点可出现在数字的任何位置。每种编程语言都须细心设计，以妥善地处理浮点数，
确保不管小数点出现在什么位置，数字的行为都是正常的。
从很大程度上说，使用浮点数时都无需考虑其行为。你只需输入要使用的数字，Python通常
都会按你期望的方式处理它们：'''
a=0.2+0.1
b=0.1+0.3
print (a,b,sep="\n")
```

    0.30000000000000004
    0.4


​    


```python
#但需要注意的是，结果包含的小数位数可能是不确定的：
a=0.2+0.1
b=0.3
print (a,b,a==b,sep="\n") #这里输出的结果为False 说明a!=b
'''所有语言都存在这种问题，没有什么可担心的。Python会尽力找到一种方式，以尽可能精确
地表示结果，但鉴于计算机内部表示数字的方式，这在有些情况下很难。就现在而言，暂时忽略
多余的小数位数即可,在后面我会去讲解这个玩意的（需要时处理多余小数位的方式）'''
```

    0.30000000000000004
    0.3
    False


##  使用函数str()避免类型错误 


```python
age = 23
message = "Happy " + age + "rd Birthday!"
#这段代码会运行错误! TypeError: can only concatenate str (not "int") to str
# 这里的原因就是类型错误 因为“age”是一个int型
```


    ---------------------------------------------------------------------------
    
    TypeError                                 Traceback (most recent call last)
    
    <ipython-input-62-669a0a352e97> in <module>
          1 age = 23
    ----> 2 message = "Happy " + age + "rd Birthday!"
          3 #这段代码会运行错误! TypeError: can only concatenate str (not "int") to str
          4 # 这里的原因就是类型错误 因为“age”是一个int型
          5 print(type(age))


    TypeError: can only concatenate str (not "int") to str



```python
print(type(age))
```

    <class 'int'>


## Python之禅


```python
import this  #讲解写代码的一些规范
'''Python程序员笃信代码可以编写得漂亮而优雅。编程是要解决问题的，设计良好、高效而漂
亮的解决方案都会让程序员心生敬意。随着你对Python的认识越来越深入，并使用它来编写越来
越多的代码，有一天也许会有人站在你后面惊呼：“哇，代码编写得真是漂亮！”'''
```

    The Zen of Python, by Tim Peters
    
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!


# List(列表）

## 什么是列表（list）
    列表由一系列按特定顺序排列的元素组成。你可以创建包含字母表中所有字母、数字0~9或
所有家庭成员姓名的列表；也可以将任何东西加入列表中，其中的元素之间可以没有任何关系。
鉴于列表通常包含多个元素，给列表指定一个表示复数的名称（如letters、digits或names）是
个不错的主意。
在Python中，用方括号（[]）来表示列表，并用逗号来分隔其中的元素。下面是一个简单的

```python
#举个栗子（哈哈哈）
color=["yellow","black","red","green","purple"]
print(color)
#将每一个元素打印出来 这里利用一个循环吧
for i in color:
    print (i)
#是不是很简单呢！
```

    ['yellow', 'black', 'red', 'green', 'purple']
    yellow
    black
    red
    green
    purple


## 访问list 元素


```python
#访问列表元素
test=[1,2,3,4,56,7,8,6,443,3,2,2,23,23,]
print(test[3])
```

    4



    ---------------------------------------------------------------------------
    
    AttributeError                            Traceback (most recent call last)
    
    <ipython-input-7-06056aaa51a4> in <module>
          2 test=[1,2,3,4,56,7,8,6,443,3,2,2,23,23,]
          3 print(test[3])
    ----> 4 print(test[3].title())


    AttributeError: 'int' object has no attribute 'title'



```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[0].title())   #将元素的首字母大写
```

    Trek



```python
print(bicycles[3].title()) #title 是将英文单词的首字母进行大写
print(bicycles[3].upper()) #upper 是将英文所有的都大写
print("\n",bicycles[3].lower()) #lower 是将英文小写

''''Python为访问最后一个列表元素提供了一种特殊语法。通过将索引指定为-1，可让Python返
回最后一个列表元素：'''
print(bicycles[-1])
print()
#这里要说明的是：Python 的索引是从零（0）开始的，这点请明确
```

    Specialized
    SPECIALIZED
    
     specialized
    specialized


​    


```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
a=len(bicycles)
for i in range(4):
    message="my fist bicycle was a "+bicycles[i].title()+"."
    print(message)
```

    my fist bicycle was a Trek.
    my fist bicycle was a Cannondale.
    my fist bicycle was a Redline.
    my fist bicycle was a Specialized.



```python

```

## 修改、添加和删除元素 


```python
names=["万总","大和","奇数","你好"]
#我们修改list中的第一个元素 这里记住Python的索引是从零开始的
names[0]="大家"
print(names) #可以看到将list中的第一个元素（“万和”修改为“大家”）
```

    ['大家', '大和', '奇数', '你好']


### 在列表中添加元素（append）
1. 在列表末尾添加元素
在列表中添加新元素时，最简单的方式是将元素附加到列表末尾。给列表附加元素时，它将
添加到列表末尾。继续使用前一个示例中的列表，

```python
names.append("大疆无人机")
print(names) # append 是在list尾部添加元素，而不影响列表中的其他所有元素
```

    ['大家', '大和', '奇数', '你好', '大疆无人机']

方法append()让动态地创建列表易如反掌，例如，你可以先创建一个空列表，再使用一系列的
append()语句添加元素。

```python
#创建一个空列表
users=[]
users.append("Jack")
users.append("Tom")
users.append("china")
print(users)
```

    ['Jack', 'Tom', 'china']


### 在列表中插入元素（insert）

使用方法insert()可在列表的任何位置添加新元素。为此，你需要指定新元素的索引和值。


```python
users.insert(0,"linda")
print(users)
```

    ['linda', 'Jack', 'Tom', 'china']


### 从列表中删除元素(del and pop) 
 说明：“del”是删除list 中的元素，没有返回值=>del names[2] ===>删除第三个元素，
        （记住Python的索引是从零开始的）
    "pop"是删除list中的元素，并且有返回值====>names.pop[2]

```python
#  del 的使用方法
#这次我们还是使用上次的list====>names
users=['linda', 'Jack', 'Tom', 'china']
del users[0]
print(users)#可以看到将list中的第一个元素（“linda“删除了；
#使用del语句将值从列表中删除后，你就无法再访问它了
```

    ['Jack', 'Tom', 'china']



```python
#  使用 pop()进行元素的删除
#  有时候，你要将元素从列表中删除，并接着使用它的值。
#我们重新建立一个list 文件，顺便复习一下3.3.1 and 3.3.2 的元素的添加和插入
#-----------------------------------------------------
#首先我们建立一个空的list
products=[]
#我们复习一下 append吧！
products.append("nihao") #每次只能添加一个元素=========>append
products.append(2)
products.append("中国")
#再复习一下在list中插入元素这个函数吧=====>insert
products.insert(1,"Videos")#括号中的“1”是索引“1”，也就是第2个元素，索引是从0开始的
#现在我们用pop()将第2个元素删除
a=products.pop(1)
products.pop(1)
print(products)
print("删除的值是:'{}'".format(a))  #设置指定位置，可以多次使用，这个可以查看1.1 print()函数
```

    ['nihao', '中国']
    删除的值是:'Videos'


   别忘了，每当你使用pop()时，被弹出的元素就不再在列表中了。
如果你不确定该使用del语句还是pop()方法，下面是一个简单的判断标准：如果你要从列表
中删除一个元素，且不再以任何方式使用它，就使用del语句；如果你要在删除元素后还能继续
使用它，就使用方法pop()。

### 根据值删除元素 remove()

有时候，你不知道要从列表中删除的值所处的位置。如果你只知道要删除的元素的值，可使
用方法remove()。


```python
#这次建立一个数字list吧
x=[1,2,3,5,3,2,4,5,4,4,34,53,5,54,35]
#现在用remove来删除list中的值
x.remove(2) #这里只删除元素中前面的一个值
print (x)
```

    [1, 3, 5, 3, 2, 4, 5, 4, 4, 34, 53, 5, 54, 35]


注意： 方法remove()只删除第一个指定的值。如果要删除的值可能在列表中出现多次，就需要
使用循环来判断是否删除了所有这样的值


```python
#这里试着写一下，后面会学习的 ===============>这里用一个if 语句吧（了解）
x=[1,2,3,5,3,2,4,5,4,4,34,53,5,54,35]
a,b=2,0
for i in x:
    if 2 in x:
        x.remove(a)
        b+=1
print(x)
print("\n共有'{}'{}个".format(a,b))
```

    [1, 3, 5, 3, 4, 5, 4, 4, 34, 53, 5, 54, 35]
    
    共有'2'2个


### 组织列表

元素的排列顺序常常是无法预测的，因为你并非总能控制用户提供数据
的顺序。这虽然在大多数情况下都是不可避免的，但你经常需要以特定的顺序呈现信息。有时候，
你希望保留列表元素最初的排列顺序，而有时候又需要调整排列顺序。Python提供了很多组织列
表的方式，可根据具体情况选用。

使用方法sort()对列表进行永久性排序 

使用函数sorted()对列表进行临时排序

### 使用方法sort()对列表进行永久性排序 

Python方法sort()让你能够较为轻松地对列表进行排序


```python
A=['数学','语文','地理','英语','化学','日本语']
A.sort()
print(A)
#方法sort()（见）永久性地修改了列表元素的排列顺序。现在，汽车是按字母顺序排列的，
#再也无法恢复到原来的排列顺序
```

    ['化学', '地理', '数学', '日本语', '英语', '语文']



```python
#可以将字符串反向传递出来，在这里只需要向函数sort（）传递参数reverse=True即可
A.sort(reverse=True)
print(A) #这个是对元素永久性的修改
```

    ['语文', '英语', '日本语', '数学', '地理', '化学']


### 使用函数sorted()对列表进行临时排序 


```python
# 要保留列表元素原来的排列顺序，同时以特定的顺序呈现它们，可使用函数sorted()
print ("原始list是:{}\n 使用sorted函数后的list是:{}".format(A,sorted(A)))

#调用函数sorted()后，列表元素的排列顺序并没有变。如果你要按与字母顺
#序相反的顺序显示列表，也可向函数sorted()传递参数reverse=True。如下：
s=["a","C","F","d","e","ww"]
print(s)
print(sorted(s,reverse=True)) #“reverse”不是指按与字母顺序相反的顺序排列列表元素，
#而只是反转列表元素的排列顺序：=================>切记，切记，切记。。。。
```

    原始list是:['语文', '英语', '日本语', '数学', '地理', '化学']
     使用sorted函数后的list是:['化学', '地理', '数学', '日本语', '英语', '语文']
    ['a', 'C', 'F', 'd', 'e', 'ww']
    ['ww', 'e', 'd', 'a', 'F', 'C']


#### 倒着打印列表 


```python
# 使用reverse函数进行反转
#举个栗子
d=[1,2,3,6,7,8,6,5,4] 
#反向打印
d.reverse()  #反向排序
print(d) 
d.reverse()  #反向排序，回到原来的list顺序
print(d)
```

    [4, 5, 6, 8, 7, 6, 3, 2, 1]
    [1, 2, 3, 6, 7, 8, 6, 5, 4]


#### 字符串的长度计算 （len( )） 


```python
f=d
print (f,"\n'f'字符串的长度是{}".format(len(f)))
```

    [1, 2, 3, 6, 7, 8, 6, 5, 4] 
    'f'字符串的长度是9


## 使用列表时避免索引错误 

刚开始使用列表时，经常会遇到一种错误。假设你有一个包含三个元素的列表，却要求获取
第四个元素：


```python
#举例：
# list中有3个元素
e=[1,2,5]
print(e[3]) #这里的3是索引3，也就是第四个元素
#IndexError: list index out of range(list索引超出范围)
```


    ---------------------------------------------------------------------------
    
    IndexError                                Traceback (most recent call last)
    
    <ipython-input-28-5857a3c5decd> in <module>
          2 # list中有3个元素
          3 e=[1,2,5]
    ----> 4 print(e[3]) #这里的3是索引3，也就是第四个元素
          5 #IndexError: list index out of range(list索引超出范围)


    IndexError: list index out of range



```python
#=======================方法一=================================
# 如果你想访问list的最后一个元素
# ① 使用len（）函数获得字符串长度，最后一个元素的索引：len（）-1 如下：
a=e[len(e)-1]
print(a)
```

    5



```python
#=======================方法二=================================
#②在不知道元素个数的情况下可以使用[-1]
print(e[-1])
# 2种方法自己看情况使用
```

    5



```python
x=[]
#列表x不包含任何元素，因此Python返回一条索引错误消息：
print(x[-1])
#======>关闭程序前，务必消除这个错误。
```


    ---------------------------------------------------------------------------
    
    IndexError                                Traceback (most recent call last)
    
    <ipython-input-33-2dda8d82dcff> in <module>
          1 x=[]
          2 #列表x不包含任何元素，因此Python返回一条索引错误消息：
    ----> 3 print(x[-1])


    IndexError: list index out of range


# 操作列表

## 遍历整个列表

你经常需要遍历列表的所有元素，对每个元素执行相同的操作
需要对列表中的每个元素都执行相同的操作时，可使用Python中的for循环。


```python
#下面使用for循环来打印名单中的所有名字：
names = ['Linda','alice', 'david', 'carolina']
for i in names:
    print(i,end="\t")
```

    Linda	alice	david	carolina	

## 深入地研究循环

循环这种概念很重要，因为它是让计算机自动完成重复工作的常见方式之一,
这里要感谢我的第一家（Omron）公司，因为创始人（立石一真）说过 机器能干的事情就让机器去干吧！

这个概念很重要，请你一定要去阅读官方文档，
最好的 Python 教程，是官方网站上的 The Python Tutorial
地址：

https://docs.python.org/zh-cn/3/tutorial/index.html (for v.3.7.2）
http://www.pythondoc.com/pythontutorial3/ (for v.3.6.3)
你必须要这个循坏概念彻底的可在自己的脑中，就像我们吃饭一样，变成一种潜意识行为
，这样你后期才能够专注与自己的模型设计，从而产出更多的东西      
for循环
https://docs.python.org/zh-cn/3/tutorial/controlflow.html#for-statements

## 使用函数range() 


```python
for value in range(1,5):
    print(value,end="\t")
#上述代码好像应该打印数字1~5，但实际上它不会打印数字5
#因为Range(1,5)不包含最后一位数字
```

    1	2	3	4	

### 使用 range()创建数字列表 

要创建数字列表，可使用函数list()将range()的结果直接转换为列表。如果将range()作为                        
list()的参数，输出将为一个数字列表。


```python
print(list(range(1,4))) #将range（）元素直接转化为list
#输出0~20之间的偶数
print((list(range(0,21,2)))) #使用函数range()时，还可指定步长
```

    [1, 2, 3]
    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20]



```python
#创建0~10的平方为一个元素集合
we=[]
for i in range(11):
    i=i**2
    we.append(i)
print(we)
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100]


### 对数字列表执行简单的统计计算 

有几个专门用于处理数字列表的Python函数。                         
例如，你可以轻松地找出数字列表的最大值、最小值和总和：函数分别是 max(),min(),sum()


```python
#接上面个的元素list
print(max(we),min(we),sum(we),end="\n")
```

    100 0 385


## 列表解析 

前面介绍的生成列表squares的方式包含三四行代码，而列表解析让你只需编写一行代码就                
能生成这样的列表。列表解析将for循环和创建新元素的代码合并成一行，并自动附加新元素。


```python
box=[x**2 for x in range(11)]
print(box)
#这个表达式，我也是第一次接触，也要刻在脑子中
```

    [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100]


## 使用列表的一部分

要创建切片，可指定要使用的第一个元素和最后一个元素的索引。与函数range()一样，          
Python在到达你指定的第二个索引前面的元素后停止。要输出列表中的前三个元素，需要指定索引0~3，       
这将输出分别为0、1和2的元素。

### 切片


```python
colors=["yellow","blue","red","black","green","purple"]
#我们用切片输出前三个元素
print(colors[0:3])
#如果你要提取列表的第2~4个元素，可将起始索引指定为1，并将终止索引指定为4：
print(colors[1:4])
#如果你没有指定第一个索引，Python将自动从列表开头开始：
print(colors[:4])
#要让切片终止于列表末尾，也可使用类似的语法
print(colors[2:])
#还有一个索引（负数索引）如果一个list很大你不知道后面的数字，\
#这时你想要最后三个值，这时就使用负数切片
print(colors[-3:])
```

    ['yellow', 'blue', 'red']
    ['blue', 'red', 'black']
    ['yellow', 'blue', 'red', 'black']
    ['red', 'black', 'green', 'purple']
    ['black', 'green', 'purple']


处理数据时，可使用切片来进行批量处理；编写Web应用程序时，
可使用切片来分页显示信息，并在每页显示数量合适的信息。

### 复制列表 

要复制列表，可创建一个包含整个列表的切片，方法是同时省略起始索引和终止索引（[:]）。
这让Python创建一个始于第一个元素，终止于最后一个元素的切片，即复制整个列表。


```python
colors=["yellow","blue","red","black","green","purple"]
my_colors=colors[:]
print(my_colors)
```

    ['yellow', 'blue', 'red', 'black', 'green', 'purple']



```python
#为核实我们确实有两个列表，下面在每个列表中都添加一种color
colors=["yellow","blue","red","black","green","purple"]
my_colors=colors[:]

my_colors.append("boron")
colors.append("pick")
print("my_colors is {},\ncolors is {}".format(my_colors,colors))
```

    my_colors is ['yellow', 'blue', 'red', 'black', 'green', 'purple', 'boron'],
    colors is ['yellow', 'blue', 'red', 'black', 'green', 'purple', 'pick']


✳顺便你可以复习一下第三章中的3.3.6 and 3.3.7 的内容 进行对元素的排列


```python
colors=["yellow","blue","red","black","green","purple"]
my_colors=colors  

my_colors.append("bron")
colors.append("pick")
print("my_colors is {},\ncolors is {}".format(my_colors,colors))
```

    my_colors is ['yellow', 'blue', 'red', 'black', 'green', 'purple', 'boron', 'pick'],
    colors is ['yellow', 'blue', 'red', 'black', 'green', 'purple', 'boron', 'pick']


这里将colors赋给my_colors，而不是将colors的副本存储到my_colors。
这种语法实际上是让Python将新变量my_colors关联到包含在colors中的列表，因此这两个
变量都指向同一个列表。鉴于此，当我们将'pick'添加到colors中时，它也将出现在
my_colors中；同样，虽然'bron'好像只被加入到了my_colors中，但它也将出现在这
两个列表中。

现在暂时不要考虑这个示例中的细节。基本上，当你试图使用列表的副本时，如果结果
出乎意料，请确认你像第一个示例那样使用切片复制了列表。

## 元组

list适合储存在程序Run期间可变的数据集，list可以修改，
but sometimes 你需要创建一列不可修改的元素，元组可以满足这种需求，
Python将不能修改的值称为不可变的，而不可变的的list被称为元组。

### 定义元组 

元组看起来就像列表，但使用=====>圆括号<======而不是方括号来标识。定义元组后，就可以使用索引来
访问其元素，就像访问列表元素一样。


```python
names=("nihao","Alice","aruike","Tom","Bob")
print(names[2].title(),names[3],end="\t")
```

    Aruike Tom	


```python
a=list(names) #是将元组转化为list
print(a)
print(type(a))
#b[2]="bbbb"
print(a)
# Question：怎么把list转化为元组？====================================
```

    ['nihao', 'Alice', 'aruike', 'Tom', 'Bob']
    <class 'list'>
    ['nihao', 'Alice', 'aruike', 'Tom', 'Bob']



```python
#下面进行一个元素值的修改
names=("nihao","Alice","aruike","Tom","Bob")
a=list(names)
print(a)
a[2]="linda"#这一句是在list中替换元素，而元组中的元素是不可以修改的 如下：
names[2]="linda"
print(names) #这一句会报错，原因是元组中的元素是不可以修改的
print(a)
#在list中怎么修改list中的元素？？？？？？========================
```

    ['nihao', 'Alice', 'aruike', 'Tom', 'Bob']



    ---------------------------------------------------------------------------
    
    TypeError                                 Traceback (most recent call last)
    
    <ipython-input-27-283a519036b2> in <module>
          4 print(a)
          5 a[2]="linda"#这一句是在list中替换元素，而元组中的元素是不可以修改的 如下：
    ----> 6 names[2]="linda"
          7 print(names) #这一句会报错，原因是元组中的元素是不可以修改的
          8 print(a)


    TypeError: 'tuple' object does not support item assignment


### 遍历元组中的所有值    

像列表一样，也可以使用for循环来遍历元组中的所有值：


```python
names=("nihao","Alice","aruike","Tom","Bob")
for i in names[:-1]: #这里你可以使用（4.5.1切片）切片，选择性的遍历元组中的值
    print("{}".format(i))
print("\n")
for x in names:#这个是遍历元组中的所有值
    print(x)
    
```

    nihao
    Alice
    aruike
    Tom


​    
    nihao
    Alice
    aruike
    Tom
    Bob


##  设置代码格式

随着你编写的程序越来越长，有必要了解一些代码格式设置约定。请花时间让你的代码尽可
能易于阅读；让代码易于阅读有助于你掌握程序是做什么的，也可以帮助他人理解你编写的代码。
为确保所有人编写的代码的结构都大致一致，Python程序员都遵循一些格式设置约定。学会
编写整洁的Python后，就能明白他人编写的Python代码的整体结构——只要他们和你遵循相同的
指南。要成为专业程序员，应从现在开始就遵循这些指南，以养成良好的习惯。

### 格式设置指南

Python格式设置指南的编写者深知，代码被阅读的次数比编写的次数多。代码编写出来后，
调试时你需要阅读它；给程序添加新功能时，需要花很长的时间阅读代码；与其他程序员分享代
码时，这些程序员也将阅读它们。

### 缩进 、 行长and空行

很多Python程序员都建议每行不超过80字符。最初制定这样的指南时，在大多数计算机中，
终端窗口每行只能容纳79字符；当前，计算机屏幕每行可容纳的字符数多得多，为何还要使用79
字符的标准行长呢？这里有别的原因。专业程序员通常会在同一个屏幕上打开多个文件，使用标
准行长可以让他们在屏幕上并排打开两三个文件时能同时看到各个文件的完整行。PEP 8还建议
注释的行长都不超过72字符，因为有些工具为大型项目自动生成文档时，会在每行注释开头添加
格式化字符。
空行不会影响代码的运行，但会影响代码的可读性。Python解释器根据水平缩进情况来解读
代码，但不关心垂直间距。

# if语句 

编程时经常需要检查一系列条件，并据此决定采取什么措施。在
Python中，if语句让你能够检查程序的当前状态，并据此采取相应的
措施。


```python
cars = ['audi', 'bmw', 'subaru', 'toyota']
for i in cars:
    if i=='bmw':
        print(i.upper())
    else:
        print(i.title())
#这个例子主要说将list中的元素打印出来，如果第二个元素是“bmw”将其打印出为大写
#其他元素打印为首字母大写
```

    Audi
    BMW
    Subaru
    Toyota


## 条件测试 

每条if语句的核心都是一个值为True或False的表达式，这种表达式被称为条件测试。Python
根据条件测试的值为True还是False来决定是否执行if语句中的代码。如果条件测试的值为True，
Python就执行紧跟在if语句后面的代码；如果为False，Python就忽略这些代码。


```python
aodi=1
bmw=1
aodi==bmw
```




    True



### 检查多个条件 

你可能想同时检查多个条件，例如，有时候你需要在两个条件都为True时才执行相应的操作，
而有时候你只要求一个条件为True时就执行相应的操作。在这些情况下，关键字and和or可助你
一臂之力。

#### 使用and 和 or 检查多个条件 

要检查是否两个条件都为True，可使用关键字and将两个条件测试合而为一；如果每个测试
都通过了，整个表达式就为True；如果至少有一个测试没有通过，整个表达式就为False。


```python
#判断2个人的年龄是否都大于100岁，这里开个玩笑，也许将来有一天人类的年龄会有100岁的
#就拿Tom and Bob 吧！
Tom_age=23
Bob_age=55
Tom_age>100 and Bob_age<100
```




    False




```python
Tom_age>100 or Bob_age<100 #这个就是数学上面的“与” “或” “非”；这里要主要运算的优先顺序
```




    True


5-6 人生的不同阶段：设置变量age 的值，再编写一个if-elif-else 结构，根据age
的值判断处于人生的哪个阶段。
 如果一个人的年龄小于2 岁，就打印一条消息，指出他是婴儿。
 如果一个人的年龄为2（含）～4 岁，就打印一条消息，指出他正蹒跚学步。
 如果一个人的年龄为4（含）～13 岁，就打印一条消息，指出他是儿童。
 如果一个人的年龄为13（含）～20 岁，就打印一条消息，指出他是青少年。
 如果一个人的年龄为20（含）～65 岁，就打印一条消息，指出他是成年人。
 如果一个人的年龄超过65（含）岁，就打印一条消息，指出他是老年人。

```python
age=input("输入年龄:age")
age=int(age)
if age>65:
         print("old man") 
elif 20<age<65:
         print("成年人")
elif 13<age<=20:
    print("青少年")
elif 4<age<=13:
    print("儿童")
else:
    print("婴儿还小孩子")
#输入后按Ctrl+Enter
```

    输入年龄:age56
    成年人



```python
#如果2个list中包含相同的元素，那么怎么才能找到它们的并集呢？
W=[1,2,2,4,4,5,6,7,5,3,3]
Z=[6,5,4,3,3,4,3,2,2]
Y=[]
for i in W:
    if i in Z:
        Y.append(i)
    else:
        pass
print(Y) #将2个表中含有的公共元素打印为list ，这个功能就相当于并集， 
```

    [2, 2, 4, 4, 5, 6, 5, 3, 3]


# 字典 

你可以创
建一个表示人的字典，然后想在其中存储多少信息就存储多少信息：
姓名、年龄、地址、职业以及要描述的任何方面。你还能够存储任意
两种相关的信息，如一系列单词及其含义，一系列人名及其喜欢的数
字，以及一系列山脉及其海拔等。

## 一个简单的字典 

与大多数编程概念一样，要熟练使用字典，也需要一段时间的练习。使用字典一段时间后，
你就会明白为何它们能够高效地模拟现实世界中的情形。

键—值对是两个相关联的值。指定键时，Python将返回与之相关联的值。键和值之间用冒号
分隔，而键—值对之间用逗号分隔。在字典中，你想存储多少个键—值对都可以。


```python
#举个栗子  存储一个用户名和密码的字典 如下：
#在Python中，字典用放在花括号{}中的一系列键—值对表示，如前面的示例所示：
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
print(User_informations)
```

    {'Tom': 3323, 'Bob': '00324', 'Linda': 55443}


### 访问字典中的值 


```python
#要获取与键相关联的值，可依次指定字典名和放在方括号内的键，如下所示：
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
print(User_informations['Tom'])
print("\nTom的密码是：{}".format(User_informations['Tom']))
```

    3323
    
    Tom的密码是：3323


### 添加键—值对 

字典是一种动态结构，可随时在其中添加键—值对。要添加键—值对，可依次指定字典名、用
方括号括起的键和相关联的值。


```python
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
print(User_informations)

#新增2个键值对
User_informations['Jack']=3456
User_informations['Lilei']=6654
print(User_informations)
#可以看到输出后新增加了2个键值对 如下输出：
```

    {'Tom': 3323, 'Bob': '00324', 'Linda': 55443}
    {'Tom': 3323, 'Bob': '00324', 'Linda': 55443, 'Jack': 3456, 'Lilei': 6654}


   这个字典的最终版本包含四个键—值对，键—值对的排列顺序与添加顺序不同。          
   Python不关心键—值对的添加顺序，而只关心键和值之间的关联关系。

### 先创建一个空字典 

有时候，在空字典中添加键—值对是为了方便，而有时候必须这样做。为此，可先使用一对
空的花括号定义一个字典，再分行添加各个键—值对。例如，下例演示了如何以这种方式创建字典


```python
Cars={} #创建字典用大括号
print(type(Cars))  #查看集合类型
#下面2句话是将在空的字典里建立2个键值对
Cars['Aodi']=200000
Cars['Bmw']=1000000
#打印字典
print(Cars) 
```

    <class 'dict'>
    {'Aodi': 200000, 'Bmw': 1000000}


### 修改字典中的值

要修改字典中的值，可依次指定字典名、用方括号括起的键以及与该键相关联的新值。


```python
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
#Next we will change ‘Tom’s password and Linda's password
#为了更好的展示，我们把他们的密码都设置为字母
#修改如下：
print('变更前的'+str(User_informations))
User_informations['Tom']='Hello'
User_informations['Linda']='purple'
print('变更后的'+str(User_informations))
```

    变更前的{'Tom': 3323, 'Bob': '00324', 'Linda': 55443}
    变更后的{'Tom': 'Hello', 'Bob': '00324', 'Linda': 'purple'}



```python

```

### 删除键—值对  (del)

对于字典中不再需要的信息，可使用del语句将相应的键—值对彻底删除。使用del语句时，
必须指定字典名和要删除的键。


```python
User_informations={'Tom': 'Hello', 'Bob': '00324', 'Linda': 'purple'} 
del User_informations['Tom'] #注意：删除的键—值对永远消失了。
print(User_informations)
```

    {'Bob': '00324', 'Linda': 'purple'}


## 遍历字典 

探索各种遍历方法前，先来看一个新字典，它用于存储有关网站用户的信息。下面的字典存
储一名用户的用户名、名和姓：

### 遍历字典中的所有键值对


```python
user_0 = {
'username': 'efermi',
'first': 'enrico',
'last': 'fermi',
}
for key,value in user_0.items():
    print('\nkey'+key)
    print("value"+value)
```


    keyusername
    valueefermi
    
    keyfirst
    valueenrico
    
    keylast
    valuefermi


一个Python字典可能只包含几个键—值对，也可能包含数百万个键—值对。鉴于字典可能包含
大量的数据，Python支持对字典遍历。字典可用于以各种方式存储信息，因此有多种遍历字典的
方式：可遍历字典的所有键—值对、键或值。


```python
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
for key,value in User_informations.items():
    print(key,value)
```

    Tom 3323
    Bob 00324
    Linda 55443


### 遍历字典中的所有键 (keyes())

在不需要使用字典中的值时，方法keys()很有用。

遍历字典时，会默认遍历所有的键，因此，如果将上述代码中的for i in User_informations.keys():替换为for i in User_informations:，输出将不变。 如果显式地使用方法keys()可让代码更容易理解，你可以选择这样做，但如果你愿意，也可 省略它。


```python
#方法一 使用keys  ==========>这种方法比较清楚的表达，当然你用方法二也是可以的
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
for i in User_informations.keys():
    print(i)
    #print(i.upper())  #这里是将元素的key全部大写输出，
    #还记的第三章讲过的字符串的处理吗：upper，lower，title
```

    Tom
    Bob
    Linda



```python
#方法二：
for i in User_informations:
    print(i.upper()) #复习前面的内容 upper
```

    TOM
    BOB
    LINDA


### 遍历字典中的所有值 

如果你感兴趣的主要是字典包含的值，可使用方法values()，它返回一个值列表，而不包含
任何键。


```python
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
for i in User_informations.values():
    print (i,end="\t")
```

    3323	00324	55443	


```python
#想在我们再深入的想一下 怎么把values变成一个list？
#建立一个空list
User_informations={'Tom':3323,'Bob':'00324',"Linda":55443}
Values=[]
for i in User_informations.values():
    Values.append(i)  #这里就是
print(Values)
```

    [3323, '00324', 55443]



```python
# ①list中有重复项
#我们修改如下字典中的‘Tom’和‘Linda’的Value是相同时，看看输出的list时什么
User_informations={'Tom':3323,'Bob':'00324',"Linda":3323}
Values=[]
for i in User_informations.values():
    Values.append(i)  #这里就是之前讲过的append（）===>复习
print(Values)
```

    [3323, '00324', 3323]


这种做法提取字典中所有的值，而没有考虑是否重复。涉及的值很少时，这也许不是问题，
但如果很多呢？最终的列表可能包含大量的重复项。为剔除重复项，可使用集合（set）。
集合类似于列表，但每个元素都必须是独一无二的：看到输出的list中有重复的元素，那么如果要去掉重复值的话，该怎么处理？元组、列表、集合、字典的区别https://www.cnblogs.com/maruobo/p/9669463.html


```python
#②剔除重复项
User_informations={'Tom':3323,'Bob':'00324',"Linda":3323}
Values=[]
#使用set剔除重复项
for i in set(User_informations.values()):
    Values.append(i)
print(Values)
#可以对比①和②的区别，根据自己的需求进行选择  
```

    [3323, '00324']


## 嵌套

 有时候，需要将一系列字典存储在列表中，或将列表作为值存储在字典中，这称为嵌套。你
可以在列表中嵌套字典、在字典中嵌套列表甚至在字典中嵌套字典。正如下面的示例将演示的，
嵌套是一项强大的功能。 

### 字典列表

这里我还没有找到一个好一点的栗子

### 在字典中储存list 


```python

```

### 在字典中储存字典 


```python
#这个程序要好好研究一哈  字典应用比较全面
users = {
'aeinstein': {
'first': 'albert',
'last': 'einstein',
'location': 'princeton',
},
'mcurie': {
'first': 'marie',
'last': 'curie',
'location': 'paris',
},
}
for username, user_info in users.items():
    print("\nusername:"+username)
    full_name=user_info['first']+user_info["last"]
    location=user_info['location']
    
    print("\tfull_name:"+full_name.title())
    print("\tlocation:"+location)
```


    username:aeinstein
    	full_name:Alberteinstein
    	location:princeton
    
    username:mcurie
    	full_name:Mariecurie
    	location:paris



```python
#再来写一个
people={
    'Tom':
    {'age':23,
     'gender':"boy",
     'height':168,
        },
    "Linda":
    {'age':25,
    'gender':'girl',
    'height':166
    }
}
for name,information in people.items():
    print("\n{}'s age is:{},gender is:{},Height is:{}" \
        .format(name,information['age'], \
        information['gender'],information['height']))
    #真一行写的真长，不建议这样做 如果真的需要写这么长的code
    #建议换行 [空格]+'\'
    #应该看的懂吧
```


    Tom's age is:23,gender is:boy,Height is:168
    
    Linda's age is:25,gender is:girl,Height is:166


# 用户输入和while循环

大多数程序都旨在解决最终用户的问题，为此通常需要从用户那
里获取一些信息。例如，假设有人要判断自己是否到了投票的年龄，
要编写回答这个问题的程序，就需要知道用户的年龄，这样才能给出
答案。因此，这种程序需要让用户输入其年龄，再将其与投票年龄进
行比较，以判断用户是否到了投票的年龄，再给出结果。
这里要介绍一个函数==========>input()

## 函数input()的工作原理 

函数input()让程序暂停运行，等待用户输入一些文本。获取用户输入后，Python将其存储在
一个变量中，以方便你使用。
例如，下面的程序让用户输入一些文本，再将这些文本呈现给用户：


```python
#==============>注意在Jupyter NotBook中输入后再次按‘Ctrl’+‘enter’程序方可执行下一步
message=input("")
print(message)
```

    ewritweutpoieungvnkr;en
    ewritweutpoieungvnkr;en


### 编写清晰的程序

每当你使用函数input()时，都应指定清晰而易于明白的提示，准确地指出你希望用户提供
什么样的信息——指出用户该输入任何信息的提示都行，如下所示：


```python
name = input("Please input your name: ")
print("Hello, " + name +" I ♥ U" " !")
```

    Please input your name: Questeryu
    Hello, Questeryu I ♥ U !


### 使用intput()来获取数值输入 


```python
#使用函数input()时，Python将用户输入解读为字符串。
age=input("how old are you?")
print(age)
print(type(age)) #可以看到输出的数字时字符串类型
#接下来我们要验证输入的是字符还是数字 如下：（数字可以进行加减运算，而字符串是不可以的）
age=age+1  #见程序报错=====>can only concatenate str (not "int") to str
print(age)
```

    how old are you?23
    23
    <class 'str'>



    ---------------------------------------------------------------------------
    
    TypeError                                 Traceback (most recent call last)
    
    <ipython-input-25-51879af4cc99> in <module>
          4 print(type(age)) #可以看到输出的数字时字符串类型
          5 #接下来我们要验证输入的是字符还是数字 如下：（数字可以进行加减运算，而字符串是不可以的）
    ----> 6 age=age+1
          7 print(age)


    TypeError: can only concatenate str (not "int") to str



```python
#对于上面的程序，我们怎么处理呢？根据它的报错，进行类型转化 srt转化为int 如下：
age=input("how old are you?")
print(age)
print(type(age)) #可以看到输出的数字时字符串类型
#==================进行类型转化=================================
age=int(age)  #将str型转化为int型 这个样子就可以进行运算了
age=age+1 
print(age)
#在这里主要涉及到关于关于类型的转化的的相关运算
```

    how old are you?23
    23
    <class 'str'>
    24


### 求模运算符（说白了 就是取余） 

处理数值信息时，求模运算符（%）是一个很有用的工具，它将两个数相除并返回余数：

这个怎么讲啊，没有什么东西可以讲啊，这个是小学数学，就说10除以3商和余数是set少，不要给我说你不会
如果你真的不会，相信你也不会看到这里的
这里要注意的一点就是============>被除数不等于零  如下：


```python
a=10%0
print(a)
```


    ---------------------------------------------------------------------------
    
    ZeroDivisionError                         Traceback (most recent call last)
    
    <ipython-input-28-a0b5039d5445> in <module>
    ----> 1 a=10/0
          2 print(a)


    ZeroDivisionError: division by zero



```python
x=10%3  #取余也就是求模RUN
print(x)
```

    1


## while 循环简介

for循环用于针对集合中的每个元素都一个代码块，而while循环不断地运行，直到指定的条
件不满足为止。

### 使用while 循环 


```python
#你可以使用while循环来数数， 如下：
a=1
while a<=5:
    print(a)
    a+=1
```

    1
    2
    3
    4
    5


### 让用户选择何时退出

 这里我们程序中设计一个退出的功能
#告诉程序当输入某个值的情况下，就退出当前的while循环 
#那么我们就设计一个退出的条件：while a!=“你好”的时候退出当前的while循环 如下：
a=0
while a!="你好":#如果程序条件为False  
    a=input()
    if a !="你好":
        print (a)
print ("循环结束")

### 在循环中使用continue和break

要返回到循环开头，并根据条件测试结果决定是否继续执行循环，可使用continue语句，它
不像break语句那样不再执行余下的代码并退出整个循环。例如，来看一个从1数到10，但只打印
其中偶数的循环：


```python
#continue的使用 如下：
a=0
while a<11:
    a+=1
    if a%2!=0:  #如果这里是“a%2==0 那么它打印出来的就是奇数循环
        continue  #如果if条件成立就执行 ‘Continue'后======>执行while循环
    print(a)
```

    2
    4
    6
    8
    10



```python
#break的使用（break是直接结束了这个循环，
a=-1
while a<11:
    a+=1
    if a%2!=0:
        break 
    print(a)
```

    0


### 避免无限循环

每个while循环都必须有停止运行的途径，这样才不会没完没了地执行下去。例如，下面的
循环从1数到5：


```python
x=1
while x<=5:
    print(x)
    x+=1  #如果程序缺少这一个步骤的话，程序将会无限的运行下去
#每个程序员都会偶尔因不小心而编写出无限循环，在循环的退出条件比较微妙时尤其如此。
#如果程序陷入无限循环 可以按停止按钮来结束循环，（这里根据编译器的不同结束方法也不相同，这里请百度）
```

    1
    2
    3
    4
    5


## 使用while 循环来处理列表和字典 

到目前为止，我们每次都只处理了一项用户信息：获取用户的输入，再将输入打印出来或作
出应答；循环再次运行时，我们获悉另一个输入值并作出响应。然而，要记录大量的用户和信息，
需要在while循环中使用列表和字典。
for循环是一种遍历列表的有效方式，但在for循环中不应修改列表，否则将导致Python难以
跟踪其中的元素。要在遍历列表的同时对其进行修改，可使用while循环。通过将while循环同列
表和字典结合起来使用，可收集、存储并组织大量输入，供以后查看和显示。

===这点要记住了哦=====>要在遍历列表的同时对其进行修改，可使用while循环。通过将while循环同列表和字典结合起来使用，可收集、存储并组织大量输入，供以后查看和显示。

### 在列表之间移动元素 


```python
unconfirmed_users = ['alice', 'brian', 'candace']
confirmed_users = []
# 验证每个用户，直到没有未验证用户为止
# 将每个经过验证的列表都移到已验证用户列表中
while unconfirmed_users:
    current_user = unconfirmed_users.pop()
    print("Verifying user: " + current_user.title())
    confirmed_users.append(current_user)
# 显示所有已验证的用户
print("\nThe following users have been confirmed:")
for confirmed_user in confirmed_users:
      print(confirmed_user.title())
```

    Verifying user: Candace
    Verifying user: Brian
    Verifying user: Alice
    
    The following users have been confirmed:
    Candace
    Brian
    Alice



```python
#进行一个数据迁移吧（将A列表中的数据迁移到B别表中）如下：
A=['we','er','tyr','yiuytr','dgh','uhg','sdfs']
B=[]
while A:
    C=A.pop()   
    B.append(C.title())
print("A列表是：",A)
print("B列表是：",B)
#可以看到完整的将A列表中的数据迁移到B列表中
```

    A列表是： []
    B列表是： ['Sdfs', 'Uhg', 'Dgh', 'Yiuytr', 'Tyr', 'Er', 'We']


# 函 数

要执行函数定义的特定任务，可调用该函数。需要在程序中多次
执行同一项任务时，你无需反复编写完成该任务的代码，而只需调用
执行该任务的函数，让Python运行其中的代码。你将发现，通过使用
函数，程序的编写、阅读、测试和修复都将更容易。


```python
#其实也相当于子程序，接下来我们写一个函数，并且调用子程序并打印输出
def nihao():
    print("hello Questeryu")
#上面开头"def"告知Python定义一个函数    
nihao()
```

    hello Questeryu


## 定义一个函数

下面是一个打印问候语的简单函数，名为greet_user()：


```python
def greet_user():
    """显示简单的问候语"""
    print("Hello!")
greet_user()
```

    Hello!


这个示例演示了最简单的函数结构。①处的代码行使用关键字def来告诉Python你要定义一个
函数。这是函数定义，向Python指出了函数名，还可能在括号内指出函数为完成其任务需要什么
样的信息。在这里，函数名为greet_user()，它不需要任何信息就能完成其工作，因此括号是空
的（即便如此，括号也必不可少）。最后，定义以冒号结尾。
紧跟在def greet_user():后面的所有缩进行构成了函数体。②处的文本是被称为文档字符串
（docstring）的注释，描述了函数是做什么的。文档字符串用三引号括起，Python使用它们来生成
有关程序中函数的文档。
代码行print("Hello!")（见③）是函数体内的唯一一行代码，greet_user()只做一项工作：
打印Hello!。
要使用这个函数，可调用它。函数调用让Python执行函数的代码。要调用函数，可依次指定
函数名以及用括号括起的必要信息，如④处所示。由于这个函数不需要任何信息，因此调用它时
只需输入greet_user()即可。和预期的一样，它打印Hello!：

### 向函数传递信息 


```python
#将上面的代码修改一下 ，让输出带有名字的函数
def greet_user(name): #在括号中传入一个name
    """显示简单的问候语"""
    print("Hello!"+name)
greet_user('Lisa')
#同样我们可以调用"Tom"
greet_user('tom')
```

    Hello!Lisa
    Hello!tom


### 实参和形参 

前面定义函数greet_user()时，要求给变量username指定一个值。调用这个函数并提供这种
信息（人名）时，它将打印相应的问候语。
在函数greet_user()的定义中，变量username是一个形参——函数完成其工作所需的一项信
息。在代码greet_user('jesse')中，值'jesse'是一个实参。实参是调用函数时传递给函数的信
息。我们调用函数时，将要让函数使用的信息放在括号内。在greet_user('jesse')中，将实参
'jesse'传递给了函数greet_user()，这个值被存储在形参username中。

## 传递实参 

鉴于函数定义中可能包含多个形参，因此函数调用中也可能包含多个实参。向函数传递实参
的方式很多，可使用位置实参，这要求实参的顺序与形参的顺序相同；也可使用关键字实参，其
中每个实参都由变量名和值组成；还可使用列表和字典。下面来依次介绍这些方式。

### 位置实参 

你调用函数时，Python必须将函数调用中的每个实参都关联到函数定义中的一个形参。为此，
最简单的关联方式是基于实参的顺序。这种关联方式被称为位置实参。
为明白其中的工作原理，来看一个显示宠物信息的函数。这个函数指出一个宠物属于哪种动
物以及它叫什么名字，如下所示：


```python
def describe_pet(animal_type, pet_name):
    """显示宠物的信息"""
    print("\nI have a " + animal_type + ".")
    print("My " + animal_type + "'s name is " + pet_name.title() + ".")
describe_pet('hamster', 'harry')
```


    I have a hamster.
    My hamster's name is Harry.



```python

def sun(a,b):
    '''计算a+b的值，and a的b次方'''
    print('a+b的值是：'+str(a+b)+'\na的b次方是：'+str(pow(a,b))+'\n')
sun(3,2)
#你可以多次调用函数
sun(3,4)
#关键参数 如下：
sun(b=3,a=5)  
```

    a+b的值是：5
    a的b次方是：9
    
    a+b的值是：7
    a的b次方是：81
    
    a+b的值是：8
    a的b次方是：125


​    


```python
def sun(a=2,b=5):  #这里这个值定义一个默认值 当调用sun（）函数时候，默认输出如下：
    '''计算a+b的值，and a的b次方'''
    print('a+b的值是：'+str(a+b)+'\na的b次方是：'+str(pow(a,b))+'\n')
sun(3,2)
#默认输出
sun() #=============>这个就是默认值sun(a=2,b=5)
```

    a+b的值是：5
    a的b次方是：9
    
    a+b的值是：7
    a的b次方是：32


​    

## 返回值 

函数并非总是直接显示输出，相反，它可以处理一些数据，并返回一个或一组值。函数返回
的值被称为返回值。在函数中，可使用return语句将值返回到调用函数的代码行。返回值让你能
够将程序的大部分繁重工作移到函数中去完成，从而简化主程序。

### 返回简单值 


```python
def sum(a,b):
    c=a+b
    return c #这里就是返回值为c；
message=sum(3,5)
print(message)

```

    8


### 返回字典

函数可返回任何类型的值，包括列表和字典等较复杂的数据结构。例如，下面的函数接受姓
名的组成部分，并返回一个表示人的字典：


```python
def build_person(first_name, last_name):
    """返回一个字典，其中包含有关一个人的信息"""
    person = {'first': first_name, 'last': last_name}
    return person
musician = build_person('jimi', 'hendrix')
print(musician)
```

    {'first': 'jimi', 'last': 'hendrix'}



```python
def user_inf(user,password):
    '''记录用户的姓名和密码的字典'''
    person={user:password}
    return person
c=[]
user_inf('Tom',1234)
c.append(user_inf('Tom',1234))
print(c)
```

    [{'Tom': 1234}]


### 传递列表 


```python
#写一个返回斐波那契数列的列表（而不是把它打印出来）的函数，非常简单:
def fib(n):
    """Return a list containing the Fibonacci series up to n."""
    result = []
    a,b=0,1
    while a<n:
        result.append(a)
        a,b=b,a+b
    return result 
fib100=fib(200)
print(fib100)
```

    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144]


return 语句会从函数内部返回一个值。 不带表达式参数的 return 会返回 None。 函数执行完毕退出也会返回 None。

重要警告： 默认值只会执行一次。这条规则在默认值为可变对象（列表、字典以及大多数类实例）时很重要。比如，下面的函数会存储在后续调用中传递给它的参数:


```python
def f(a, L=[]):
    L.append(a)
    return L
print(f(2))
print(f(3))
print(f('nihao '))
```

    [2]
    [2, 3]
    [2, 3, 'nihao ']



```python
#如果你不想要在后续调用之间共享默认值，你可以这样写这个函数:
def f(a, L=[]):
    if L is not None:
        L=[]
    L.append(a)
    return L
print(f(3))
print(f('Ton'))
```

    [3]
    ['Ton']


### 解包参数列表 

当参数已经在列表或元组中但要为需要单独位置参数的函数调用解包时，会发生相反的情况。例如，内置的 range() 函数需要单独的 start 和 stop 参数。如果它们不能单独使用，可以使用 *-操作符 来编写函数调用以便从列表或元组中解包参数:


```python
print(list(range(3,6)))
```

    [3, 4, 5]



```python
age=[3,6]
print(list(range(*age)))
```

    [3, 4, 5]


### Lambda 表达式

写一个很短的函数可以用 lambda 关键字。

下面是用 def 关键字写函数：



```python
def add(x,y):
    return x+y
add(3,5)
```




    8



下面是用 lambda 关键字写函数：


```python
add=lambda x,y:x+y
add(3,5)
```




    8



lambda 的语法结构如下：

    lambda_expr ::= "lambda" [parameter_list] ":" expression
    注意： lambda 语句中， : 之后有且只能有一个表达式
而这个函数呢，没有名字，所以被称为 “匿名函数”。

作为某函数的返回值


```python
def make_incrementor(n):
    return lambda x: x + n
f = make_incrementor(42)
f(0)
f(1)
```




    43



这个例子乍看起来很令人迷惑。我们先看看 f = make_incrementor(42) 之后， f 究竟是什么东西：


```python
def make_incrementor(n):
    return lambda x: x + n
f = make_incrementor(42)
f
id(make_incrementor)
id(f)
```




    1866230533720



那 f 是什么呢？它是 <function __main__.make_incrementor.<locals>.<lambda>(x)> ：
    
    f = make_incrementor(42) 是将 make_incrementor(42) 的返回值保存到 f 这个变量之中；
    而 make_incrementor() 这个函数接收到 42 这个参数之后，返回了一个函数： lambda x: x + 42 ；
    于是， f 中保存的函数是 lambda x: x + 42 ；
    所以， f(0) 是向这个匿名函数传递了 0 ，而后，它返回的是 0 + 42 。

# 类（这部份比较难点，I believe U can）

面向对象编程是最有效的软件编写方法之一。在面向对象编程中，
你编写表示现实世界中的事物和情景的类，并基于这些类来创建对象。
编写类时，你定义一大类对象都有的通用行为。基于类创建对象时，
每个对象都自动具备这种通用行为，然后可根据需要赋予每个对象独
特的个性。使用面向对象编程可模拟现实情景，其逼真程度达到了令
你惊讶的地步。

理解面向对象编程有助于你像程序员那样看世界，还可以帮助你真正明白自己编写的代
码：不仅是各行代码的作用，还有代码背后更宏大的概念。了解类背后的概念可培养逻辑思
维，让你能够通过编写程序来解决遇到的几乎任何问题。

## 创建和使用类 

使用类几乎可以模拟任何东西。下面来编写一个表示girl friends——她表示的不是特定的GF，而是任何GF。
对于大多数GF，我们都知道些什么呢？首先如果你是一名正常男性，那么的你的对象应该是一名女性，
当然在程序的世界里我们必须要考虑其他的情况在里面，这里按照我这个年龄对这个对象概念的深了解


    如下：
    ① 女的 
    ②物理属型
    ③化学属性
    ④萝卜青菜各有所爱
    扯远了。。。。哈哈哈  不过类（Class）就是这个样子的呀

这个类让Python知道如何创建表示GF的对象。编写这个类后，我们将使用它来创建表示特定Girlfriend的实例


```python
class Girl_friend():
    '''一次模拟对象的小尝试'''
    def __init__(self, name, age):
        """初始化属性name and age"""
        self.name=name
        self.age=age    
    def person(self):
        """不知道了，概念不清"""
        print(self.name.title() + " is very 聪明.")       
    def people(self):
        """where？"""
        print(self.name.title() + " in world")
        
a=Girl_friend("Q",28)
print(a.name)
print(a.person())
print(a.people())
```

    Q
    Q is very 聪明.
    None
    Q in world
    None



```python
#接下来再来写一个吧，描写所computer（class）=========>那就写一个计算机吧
class Computer():
    '''描述一个是什么'''
    #一定要注意这里“__init__"这里左右两边各有2个"_"，不然会报错， \
    #很难找到的，我就在这里栽了跟头好几天
    def __init__(self,si,pr): 
        self.si=si
        self.pr=pr
    def Programe(self):
        '''计算机能干什么'''
        print("它可以帮助人们解决一些技术上面的问题")
    def da(self):
        '''它可以简化人们的工作'''
        print("它可以简化人们的工作")
        
liada=Computer("sa","da")
print(liada.si)
liada.da()
```

    sa
    它可以简化人们的工作


## 模拟实物

模拟较复杂的物件（如电动汽车）时，需要解决一些有趣的问题。
    这让你进入了程序员的另一个境界：解决上述问题时，你从较高的逻辑层面（而不是语法层
面）考虑；你考虑的不是Python，而是如何使用代码来表示实物。到达这种境界后，你经常会发
现，现实世界的建模方法并没有对错之分。有些方法的效率更高，但要找出效率最高的表示法，需要经过一定的实践。只要代码像你希望的那样运行，就说明你做得很好！即便你发现自己不得
不多次尝试使用不同的方法来重写类，也不必气馁；要编写出高效、准确的代码，都得经过这样
的过程。

## 导入类 

随着你不断地给类添加功能，文件可能变得很长，即便你妥善地使用了继承亦如此。为遵循
Python的总体理念，应让文件尽可能整洁。为在这方面提供帮助，Python允许你将类存储在模块
中，然后在主程序中导入所需的模块。

## 导入整个模块 

 你还可以导入整个模块，再使用句点表示法访问需要的类。这种导入方法很简单，代码也易
于阅读。由于创建类实例的代码都包含模块名，因此不会与当前文件使用的任何名称发生冲突。

## 导入模块中的所有类 

要导入模块中的每个类，可使用下面的语法：
from module_name import *
不推荐使用这种导入方式，其原因有二。首先，如果只要看一下文件开头的import语句，就
能清楚地知道程序使用了哪些类，将大有裨益；但这种导入方式没有明确地指出你使用了模块中
的哪些类。这种导入方式还可能引发名称方面的困惑。如果你不小心导入了一个与程序文件中其
他东西同名的类，将引发难以诊断的错误。这里之所以介绍这种导入方式，是因为虽然不推荐使
用这种方式，但你可能会在别人编写的代码中见到它。
需要从一个模块中导入很多类时，最好导入整个模块，并使用module_name.class_name语法
来访问类。这样做时，虽然文件开头并没有列出用到的所有类，但你清楚地知道在程序的哪些地
方使用了导入的模块；你还避免了导入模块中的每个类可能引发的名称冲突。

## 在一个模块中导入另一个模块

有时候，需要将类分散到多个模块中，以免模块太大，或在同一个模块中存储不相关的类。
将类存储在多个模块中时，你可能会发现一个模块中的类依赖于另一个模块中的类。在这种情况
下，可在前一个模块中导入必要的类。

## Python标准库

Python标准库是一组模块，安装的Python都包含它。你现在对类的工作原理已有大致的了解，
可以开始使用其他程序员编写好的模块了。可使用标准库中的任何函数和类，为此只需在程序开
头包含一条简单的import语句。下面来看模块collections中的一个类——OrderedDict。
字典让你能够将信息关联起来，但它们不记录你添加键—值对的顺序。要创建字典并记录其
中的键—值对的添加顺序，可使用模块collections中的OrderedDict类。OrderedDict实例的行为
几乎与字典相同，区别只在于记录了键—值对的添加顺序。

## 类编码风格

你必须熟悉有些与类相关的编码风格问题，在你编写的程序较复杂时尤其如此。
类名应采用驼峰命名法，即将类名中的每个单词的首字母都大写，而不使用下划线。实例名
和模块名都采用小写格式，并在单词之间加上下划线。
对于每个类，都应紧跟在类定义后面包含一个文档字符串。这种文档字符串简要地描述类的
功能，并遵循编写函数的文档字符串时采用的格式约定。每个模块也都应包含一个文档字符串，
对其中的类可用于做什么进行描述。
可使用空行来组织代码，但不要滥用。在类中，可使用一个空行来分隔方法；而在模块中，
可使用两个空行来分隔类。
需要同时导入标准库中的模块和你编写的模块时，先编写导入标准库模块的import语句，再
添加一个空行，然后编写导入你自己编写的模块的import语句。在包含多条import语句的程序中，
这种做法让人更容易明白程序使用的各个模块都来自何方。

最好的 Python 教程，是官方网站上的 The Python Tutorial，读它就够了。
其实Python官方教程写的很好的，李笑来老师建议都英文版的
这一章可以参见官方文档（中文）：https://docs.python.org/zh-cn/3/tutorial/index.html
谢谢！

# 文件和异常

## 从文件中读取数据 

文本文件可存储的数据量多得难以置信：天气数据、交通数据、社会经济数据、文学作品等。
每当需要分析或修改存储在文件中的信息时，读取文件都很有用，对数据分析应用程序来说尤其
如此。例如，你可以编写一个这样的程序：读取一个文本文件的内容，重新设置这些数据的格式
并将其写入文件，让浏览器能够显示这些内容。
要使用文本文件中的信息，首先需要将信息读取到内存中。为此，你可以一次性读取文件的
全部内容，也可以以每次一行的方式逐步读取。

### 读取整个文件 

要读取文件，需要一个包含几行文本的文件。下面首先来创建一个文件，它包含精确到小数
点后30位的圆周率值，且在小数点后每10位处都换行：

将该文件保存到本章程序所在的目录中。
地址：C:\Users\QUESTERYU\.ipynb_checkpoints 根据自己的电脑进行查找
下面的程序打开并读取这个文件，再将其内容显示到屏幕上：
3.1415926535
8979323846
2643383279
保存为text.txt 将该文件保存到本章程序所在的目录中。

```python
with open(r'C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt') as file_object:
    contents = file_object.read()
    print(contents)
```

    3.1415926535
    8979323846
    2643383279


​    

我们先来看看函数open()。要以任何方式使用
文件——哪怕仅仅是打印其内容，都得先打开文件，这样才能访问它。函数open()接受一个参数：
要打开的文件的名称。

在这个示例中，
当前运行的是这个程序，因此Python在这个程序所在的目录中查找text.txt。函数open()
返回一个表示文件的对象。在这里，open('C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt')
返回一个表示文件text.txt的对象；Python将这个对象存储在我们将在后面使用的变量中。

关键字with在不再需要访问文件后将其关闭。在这个程序中，注意到我们调用了open()，但
没有调用close()；你也可以调用open()和close()来打开和关闭文件，但这样做时，如果程序存
在bug，导致close()语句未执行，文件将不会关闭。这看似微不足道，但未妥善地关闭文件可能
会导致数据丢失或受损。如果在程序中过早地调用close()，你会发现需要使用文件时它已关闭
（无法访问），这会导致更多的错误。并非在任何情况下都能轻松确定关闭文件的恰当时机，但通
过使用前面所示的结构，可让Python去确定：你只管打开文件，并在需要时使用它，Python自会
在合适的时候自动将其关闭。
相比于原始文件，该输出唯一不同的地方是末尾多了一个空行。为何会多出这个空行呢？因
为read()到达文件末尾时返回一个空字符串，而将这个空字符串显示出来时就是一个空行。要删
除多出来的空行，可在print语句中使用rstrip()：
为何会出现这些空白行呢？因为在这个文件中，每行的末尾都有一个看不见的换行符，而
print语句也会加上一个换行符，因此每行末尾都有两个换行符：一个来自文件，另一个来自print
语句。

```python
with open(r'C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt') as text:
    text=text.read()
    print(text.rstrip())
```

    3.1415926535
    8979323846
    2643383279


### 文件路径 


```python
#要让Python打开不与程序文件位于同一个目录中的文件，需要提供文件路径，它让Python到系统的特定位置去查找。
#上面的一章调用过文件路径=========>r'C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt'
#就是这个样子的
#在Windows系统中，在文件路径中使用反斜杠（\）而不是斜杠（/）
#绝对路径通常比相对路径更长，因此将其存储在一个变量中，再将该变量传递给open()会有所帮助。

```

刚刚在运行python文件的时候竟然报SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: tr这个错误，其实引起这个错误的原因就是转义的问题。


```python
with open('C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt') as text:
    text=text.read()
    print(text.rstrip())
```


      File "<ipython-input-30-58e0eb71ff5b>", line 1
        with open('C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt') as text:
                 ^
    SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape



原因分析：在windows系统当中读取文件路径可以使用\,但是在python字符串中\有转义的含义，如\t可代表TAB，\n代表换行，所以我们需要采取一些方式使得\不被解读为转义字符。目前有3个解决方案


```python
#1、在路径前面加r，即保持字符原始值的意思。
with open(r'C:\Users\QUESTERYU\.ipynb_checkpoints\text.txt') as text:
    text=text.read()
    print(text.rstrip())
```

    3.1415926535
    8979323846
    2643383279



```python
#2、替换为双反斜杠
with open('C:\\Users\\QUESTERYU\\.ipynb_checkpoints\\text.txt') as text:
    text=text.read()
    print(text.rstrip())
```

    3.1415926535
    8979323846
    2643383279



```python
#3、替换为正斜杠
with open('C:/Users/QUESTERYU/.ipynb_checkpoints/text.txt') as text:
    text=text.read()
    print(text.rstrip())
```

    3.1415926535
    8979323846
    2643383279


也可以将路径设置为变量  如下：


```python
a='C:/Users/QUESTERYU/.ipynb_checkpoints/text.txt'
with open(a)as a:
    a=a.read()
    print(a)
    print(a.rstrip()) #去除尾部的空格
```

    3.1415926535
    8979323846
    2643383279
    
    3.1415926535
    8979323846
    2643383279


### 逐行读取 

读取文件时，常常需要检查其中的每一行：你可能要在文件中查找特定的信息，或者要以
某种方式修改文件中的文本。


```python
a='C:/Users/QUESTERYU/.ipynb_checkpoints/text.txt'
with open(a)as a:
    for i in a:
        print(i.rstrip())
    
```

    3.1415926535
    8979323846
    2643383279


​    

### 创建一个包含文件各行内容的列表


```python
使用关键字with时，open()返回的文件对象只在with代码块内可用。如果要在with代码块外
访问文件的内容，可在with代码块内将文件的各行存储在一个列表中，并在with代码块外使用该
列表：你可以立即处理文件的各个部分，也可推迟到程序后面再处理。
```


```python
#下面的示例在with代码块中将文件pi_digits.txt的各行存储在一个列表中，再在with代码块外打印它们：
a='C:/Users/QUESTERYU/.ipynb_checkpoints/text.txt'
with open(a)as a:
    lines=a.readlines()
    
for line in lines:
    print(line.rstrip())
```

    3.1415926535
    8979323846
    2643383279


​    

处的方法readlines()从文件中读取每一行，并将其存储在一个列表中；接下来，该列表被
存储到变量lines中；在with代码块外，我们依然可以使用这个变量。
我们使用一个简单
的for循环来打印lines中的各行。由于列表lines的每个元素都对应于文件中的一行，因此输出
与文件内容完全一致。

## 使用文件的内容 

 将文件读取到内存中后，就可以以任何方式使用这些数据了。下面以简单的方式使用圆周率
的值。首先，我们将创建一个字符串，它包含文件中存储的所有数字，且没有任何空格：


```python
a='C:/Users/QUESTERYU/.ipynb_checkpoints/text.txt'
with open(a)as a:
    lines=a.readlines()
po='' #新建一个字符串用于储存文件中的字符
pe=''
pc=''
#这里我们复习一下关于字符串的处理 
#详见：2.2.3  删除空白字符串中的空格（rstrip(尾部),lstrip(首部),strip(首尾))
#我们分别打印看效果
for line in lines:
    po+=line.strip()
    pe+=line.rstrip()
    pc+=line.lstrip()
print("strip(首尾)po={},\nrstrip(尾部)pe={},\n\nlstrip(首部)pc={}" \
     .format(po,pe,pc))
print(len(po))
#上面全都是是字符串不能进行运算，如果想要变成数字，就要用int整性，float浮点数
```

    strip(首尾)po=3.141592653589793238462643383279,
    rstrip(尾部)pe=3.1415926535   8979323846   2643383279,
    
    lstrip(首部)pc=3.1415926535   
    8979323846   
    2643383279
    
    32



```python
#我们下载一个百万级的圆周率，看看里面有没有自己的生日
t='C:\\Users\QUESTERYU\\.ipynb_checkpoints\\pi_million.txt'
with open(t) as t:
    lines=t.readlines()
pi=''
for line in lines:
    pi+=line.strip()
boriday=input("please you input you're boriday:")
if boriday in pi:
    print('yes')
else:
    print('No')  
```

### 写入文件

在这个示例中，调用open()时提供了两个实参。第一个实参也是要打开的文件的名称；
第二个实参（'w'）告诉Python，我们要以写入模式打开这个文件。打开文件时，可指定读取模
式（'r'）、写入模式（'w'）、附加模式（'a'）或让你能够读取和写入文件的模式（'r+'）。如果
你省略了模式实参，Python将以默认的只读模式打开文件。
如果你要写入的文件不存在，函数open()将自动创建它。然而，以写入（'w'）模式打开文
件时千万要小心，因为如果指定的文件已经存在，Python将在返回文件对象前清空该文件。


```python
import os   
t='miss.txt'
with open (t,'w') as t:
    t.write("I miss U")
print(os.getcwd())
```

    C:\Users\QUESTERYU



```python
#也可以写入多行字符串 如下：（就上面的代码，换一种方式写一下，实践一下条条大路通罗马
with open ("miss.txt",'w')as t:
    t.write("\n大家好")
    t.write("\nnimasan")
#如果文件存在，以写入（'w'）模式打开文 件时千万要小心，
#因为如果指定的文件已经存在，Python将在返回文件对象前清空该文件。切记！！！切记！！！
```


```python
#接下来我们打印出文本中的字符
with open ("miss.txt",'w')as t:
    t.write("\n大家好")
    t.write("\nnimasan")
#我们再次去读取文件中的字符串（这里还有没有更简单的方法呢？）
#if True，please tell me
with open ('miss.txt','r')as C:
    lines=C.readlines()
for line in lines:
    print(line)
```


​    
    大家好
    
    nimasan



```python
#或者使用如下方法 （这个应该比较简单，如果有更好的优化方法请给我说一哈，让我也进步）
with open ("miss.txt",'r+')as t:
    t.write("\n大家好")
    t.write("\nnimasan")
    a=t.readlines()
for i in a:
    print(i)
```


​    
    大家好
    
    nimasan
    
    大家好
    
    nimasan
    
    大家好
    
    nimasan


### 附加到文件 （附加模式'a')

如果你要给文件添加内容，而不是覆盖原有的内容，可以附加模式打开文件。你以附加模式
打开文件时，Python不会在返回文件对象前清空文件，而你写入到文件的行都将添加到文件末尾。
如果指定的文件不存在，Python将为你创建一个空文件。


```python
#以上面的“miss.txt文件为栗子
with open('miss.txt','a') as re:
    re.write("你好Questeryu\n")
    re.write("yu")
with open('miss.txt','r') as f:
    a=f.readlines()
for i in a:
    print(i)

```


​    
    大家好
    
    nimasan
    
    大家好
    
    nimasan
    
    大家好
    
    nimasan
    
    大家好
    
    nimasan你好Questeryu
    
    yu你好Questeryu
    
    yu


## 异常 

Python使用被称为异常的特殊对象来管理程序执行期间发生的错误。每当发生让Python不知
所措的错误时，它都会创建一个异常对象。如果你编写了处理该异常的代码，程序将继续运行；
如果你未对异常进行处理，程序将停止，并显示一个traceback，其中包含有关异常的报告。
异常是使用try-except代码块处理的。try-except代码块让Python执行指定的操作，同时告
诉Python发生异常时怎么办。使用了try-except代码块时，即便出现异常，程序也将继续运行：
显示你编写的友好的错误消息，而不是令用户迷惑的traceback。

### 处理ZeroDivisionError 异常

导致Python引发异常的简单错误。你可能知道不能将一个数字除以0，但我们
还是让Python这样做吧：


```python
print(33/0)
```


    ---------------------------------------------------------------------------
    
    ZeroDivisionError                         Traceback (most recent call last)
    
    <ipython-input-29-fad870a50e27> in <module>
    ----> 1 print(5/0)


    ZeroDivisionError: division by zero


错误ZeroDivisionError是一个异常对象。Python无法按你的
要求做时，就会创建这种对象。在这种情况下，Python将停止运行程序，并指出引发了哪种异常，
而我们可根据这些信息对程序进行修改。下面我们将告诉Python，发生这种错误时怎么办；这样，
如果再次发生这样的错误，我们就有备无患了。

### 使用try-except 代码块 


```python
try:
    print(33/0)
except ZeroDivisionError:
    print("You can't divide by zero!")
```

    You can't divide by zero!


如果try代码块中的代码运行
起来没有问题，Python将跳过except代码块；如果try代码块中的代码导致了错误，Python将查找
这样的except代码块，并运行其中的代码，即其中指定的错误与引发的错误相同。

如果try-except代码块后面还有其他代码，程序将接着运行，因为已经告诉了Python如何处
理这种错误

## 存储数据 

很多程序都要求用户输入某种信息，程序都把用户提供的信息存储在列表和字典等数据结构中。用户关闭程序时，你
几乎总是要保存他们提供的信息；一种简单的方式是使用模块json来存储数据。

### 使用json.dump()和json.load() 

我们来编写一个存储一组数字的简短程序，再编写一个将这些数字读取到内存中的程序。第
一个程序将使用json.dump()来存储这组数字，而第二个程序将使用json.load()。
函数json.dump()接受两个实参：要存储的数据以及可用于存储数据的文件对象。

 import json
numbers = [2, 3, 5, 7, 11, 13]
test='numbers.json'
#我们指定了要将该数字列表存储到其中的文件的名称。
#通常使用文件扩展名.json来指出文件存储的数据为JSON格式。
#接下来，我们以写入模式打开这个文件，让json能够将数据写入其中。
#我们使用函数json.dump()将数字列表存储到文件numbers.json中。
with open('test','w') as re:
    json.dump(numbers,re)


```python
#下面再编写一个程序，使用json.load()将这个列表读取到内存中：
import json
test='numbers.json'
with open(r"C:\Users\QUESTERYU\test") as t:
    numbers = json.load(t)
print(numbers)
```

    [2, 3, 5, 7, 11, 13]


### 保存和读取用户生成的数据 


```python
import json
name=input('请输入你的名字')
#username='name.json'
with open('user_name','w') as re:
    json.dump(name,re)
    print('you are name is '+name)
```

    请输入你的名字Quester yu
    you are name is Quester yu

以上就是本次4个月的学习心得，后续会再次去完善一次，

最后用乔布斯的话说：**Stay Hungry. Stay Foolish.求知若渴，虚怀若谷**

2019.12.15 于上海





# 随机漫步 


```python
import numpy as np
data = {i : np.random.randn() for i in range(7)}
data
```




    {0, 1, 4, 9, 16, 25, 36}



前两行是Python代码语句；第二条语句创建一个名为data的变量，它引用一个新创建的Python字典。最后一行打印data的值。


```python
b = [1, 2, 3]
b
```


      File "<ipython-input-8-ef1efb243a28>", line 2
        b？
         ^
    SyntaxError: invalid character in identifier




```python

```
