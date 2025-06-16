## 题目描述

Bessie has invented a new programming language, but since there is no compiler yet, she needs your help to actually run her programs.

COWBASIC is a simple, elegant language. It has two key features: addition and MOO loops. Bessie has devised a clever solution to overflow: all addition is done modulo $10^9+7$. But Bessie&#039;s real achievement is the MOO loop, which runs a block of code a fixed number of times. MOO loops and addition can, of course, be nested.

Given a COWBASIC program, please help Bessie determine what number it returns.

## 输入格式

You are given a COWBASIC program at most $100$ lines long, with each line being at most $350$ characters long. A COWBASIC program is a list of statements.

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


## 数据规模与约定

In $20$ percent of all test cases - MOO loops are not nested.  
In another $20$ percent of all test cases - The program only has $1$ variable. MOO loops can be nested.  
In the remaining test cases, there are no further restrictions.

$20\%$ 数据：MOO 循环不嵌套；  
另外 $20\%$ 数据：程序只有一个变量，MOO 循环可嵌套；  
对于 $100\%$ 的数据，程序最长 $100$ 行，每行最长 $350$ 字符。  
感谢@psk2016 提供的翻译。

## 题目来源

Platinum
