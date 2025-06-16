## 题目描述
Bessie has invented a new programming language, but since there is no compiler yet, she needs your help to actually run her programs.


COWBASIC is a simple, elegant language. It has two key features: addition and MOO loops. Bessie has devised a clever solution to overflow: all addition is done modulo $10^9+7$. But Bessie's real achievement is the MOO loop, which runs a block of code a fixed number of times. MOO loops and addition can, of course, be nested.


Given a COWBASIC program, please help Bessie determine what number it returns.


## 输入格式
You are given a COWBASIC program at most 100 lines long, with each line being at most 350 characters long. A COWBASIC program is a list of statements.

There are three types of statements:

```cpp
<variable> = <expression>

<literal> MOO {
<list of statements>
}

RETURN <variable>
```

There are three types of expressions:

```cpp
<literal>

<variable>

( <expression> ) + ( <expression> )
```

A literal is a positive integer at most 100,000.

A variable is a string of at most 10 lowercase English letters.

It is guaranteed that no variable will be used or RETURNed before it is defined. It is guaranteed that RETURN will happen exactly once, on the last line of the program.

## 输出格式
Output a single positive integer, giving the value of the RETURNed variable.


## 题目大意
### 题目描述

Bessie 发明了一种新的编程语言，但由于还没有编译器，她需要你的帮助来实际运行她的程序。

COWBASIC 是一种简单而优雅的语言。它有两个关键特性：加法和 MOO 循环。Bessie 设计了一个巧妙的解决方案来处理溢出：所有的加法都是在模 $10^9+7$ 下进行的。但 Bessie 的真正成就是 MOO 循环，它可以固定次数地运行一段代码。当然，MOO 循环和加法可以嵌套。

给定一个 COWBASIC 程序，请帮助 Bessie 确定它返回的数字。

### 输入格式

你将获得一个最多 100 行的 COWBASIC 程序，每行最多 350 个字符。一个 COWBASIC 程序是一个语句列表。

有三种类型的语句：

```cpp
<variable> = <expression>

<literal> MOO {
<list of statements>
}

RETURN <variable>
```

有三种类型的表达式：

```cpp
<literal>

<variable>

( <expression> ) + ( <expression> )
```

字面量是一个最多为 100,000 的正整数。

变量是一个最多由 10 个小写英文字母组成的字符串。

保证在定义之前不会使用或 RETURN 任何变量。保证 RETURN 恰好发生一次，并且在程序的最后一行。

### 输出格式

输出一个正整数，表示 RETURN 的变量的值。

### 说明/提示

评分

在 20% 的测试用例中，MOO 循环不会嵌套。

在另外 20% 的测试用例中，程序只有一个变量。MOO 循环可以嵌套。

在剩余的测试用例中，没有进一步的限制。

```input1
x = 1
10 MOO {
x = ( x ) + ( x )
}
RETURN x
```

```output1
1024
```

```input2
n = 1
nsq = 1
100000 MOO {
100000 MOO {
nsq = ( nsq ) + ( ( n ) + ( ( n ) + ( 1 ) ) )
n = ( n ) + ( 1 )
}
}
RETURN nsq
```

```output2
4761
```

## 提示
Scoring

In 20 percent of all test cases - MOO loops are not nested.

In another 20 percent of all test cases - The program only has 1 variable. MOO loops can be nested.

In the remaining test cases, there are no further restrictions.

