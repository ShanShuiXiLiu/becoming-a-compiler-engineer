# 编译技术入门与实战

## Cooper 教授 L20SDT-2 评注

上一课slides将搭车构建AST的原理介绍清楚了。
L20 开始是更加具体的构建。

### 0

SDT一共有3个slides，这是第二个。

### 1 - 7

复习L19的内容。注意里面有些不明白的地方的话，可以从 Cooper 教授的 Parsing-4 开始看，开始进入 handler 和 LR 部分。

### 8

比较重要的计算思维的理解。
也可以类比设计模式里面的算法模版。

将【计算】附着于【语法】上
Parser 决定了计算被执行的时间点和次序
可以做很多事情。

corollary - Bing dictionary
    US['kɔrə.leri]UK[kə'rɒləri]
    n.必然的结果（或结论）
    网络推论；系；系定理

### 9

这里需要稍微发挥一下想象力：想象自己根据已经被具像化为自动机和栈的语法解析器（Parser）构建出来一个树结构的AST。
类似于抄作业，将概念上的语法产生式，誊抄到数据结构中的二叉树（有可能N叉，等价的）。

一个例子：看懂了就会做之前的编程作业了。
注意 $$ 的类型

### 10 - 19

极好的演示，构建AST

### 20 - 28

即使没有看过ILOC也没关系，只要有RISC概念就能看懂。

提到了 NextRegister，咔咔，开始硬核起来了

e·mit /əˈmit/

p26页，回忆下 IR 中的三地址码形式，隐含变量形式。

### 29

Cooper 大佬说了啥？
大佬说啥就是啥，记下来

### 30

引出两个经典优化。

主要的思想是进行任务的拆解。不要把所有要做的事情放在一个算法模版里（不好弄）。

### 31

先知道就行，真实世界很复杂的

### 32

ST = 符号表

lowering 不太好翻译

蓝字部分我也不理解，欢迎弹幕补充经验

### 33

字面理解好就OK。

### 34

符号表。先声明再使用的约定。

### 35 - 40

有意思的例子。
提问：LL或lR会有影响么？ Int a 和 a: int 有差别么？