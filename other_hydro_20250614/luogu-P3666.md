## ��Ŀ����
Bessie has invented a new programming language, but since there is no compiler yet, she needs your help to actually run her programs.


COWBASIC is a simple, elegant language. It has two key features: addition and MOO loops. Bessie has devised a clever solution to overflow: all addition is done modulo $10^9+7$. But Bessie's real achievement is the MOO loop, which runs a block of code a fixed number of times. MOO loops and addition can, of course, be nested.


Given a COWBASIC program, please help Bessie determine what number it returns.


## �����ʽ
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

## �����ʽ
Output a single positive integer, giving the value of the RETURNed variable.


## ��Ŀ����
### ��Ŀ����

Bessie ������һ���µı�����ԣ������ڻ�û�б�����������Ҫ��İ�����ʵ���������ĳ���

COWBASIC ��һ�ּ򵥶����ŵ����ԡ����������ؼ����ԣ��ӷ��� MOO ѭ����Bessie �����һ������Ľ��������������������еļӷ�������ģ $10^9+7$ �½��еġ��� Bessie �������ɾ��� MOO ѭ���������Թ̶�����������һ�δ��롣��Ȼ��MOO ѭ���ͼӷ�����Ƕ�ס�

����һ�� COWBASIC ��������� Bessie ȷ�������ص����֡�

### �����ʽ

�㽫���һ����� 100 �е� COWBASIC ����ÿ����� 350 ���ַ���һ�� COWBASIC ������һ������б�

���������͵���䣺

```cpp
<variable> = <expression>

<literal> MOO {
<list of statements>
}

RETURN <variable>
```

���������͵ı��ʽ��

```cpp
<literal>

<variable>

( <expression> ) + ( <expression> )
```

��������һ�����Ϊ 100,000 ����������

������һ������� 10 ��СдӢ����ĸ��ɵ��ַ�����

��֤�ڶ���֮ǰ����ʹ�û� RETURN �κα�������֤ RETURN ǡ�÷���һ�Σ������ڳ�������һ�С�

### �����ʽ

���һ������������ʾ RETURN �ı�����ֵ��

### ˵��/��ʾ

����

�� 20% �Ĳ��������У�MOO ѭ������Ƕ�ס�

������ 20% �Ĳ��������У�����ֻ��һ��������MOO ѭ������Ƕ�ס�

��ʣ��Ĳ��������У�û�н�һ�������ơ�

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

## ��ʾ
Scoring

In 20 percent of all test cases - MOO loops are not nested.

In another 20 percent of all test cases - The program only has 1 variable. MOO loops can be nested.

In the remaining test cases, there are no further restrictions.

