## ���ⷭ��

쳲���������һ�����������������$F(0)=1$��$F(1)=1$��$F(i)=F(i-1)+F(i-2)$ $(2 \le i)$��ǰ�������������� $1, 1, 2, 3, 5, 8, \ldots$

ΰ��ļ����ѧ�� Byteazar ������һ���Ƿ��ļ���������е�����쳲�������ʾ��

��һ������ $b_1, b_2, \ldots , b_n$ ��ʾ���� $F(1) \times b_1+b_2 \times F(2)+ \ldots +b_n \times F(n)$����ʹ�� $F(0)$ ����

���ҵ��ǣ������ı�ʾ������ȷ������ͬ�����ֿ����в�ͬ�ı�ʾ������ $42$ ���Ա�ʾΪ $(0,0,0,0,1,0,0,1)$��$(0,0,0,0,1,1,1,0)$ �� $(1,1,0,1,0,1,1)$������ Byteazar ����һ�����ƣ�

- ��� $n>1$����ô$b_n=1$�������ֵı�ʾ������ǰ���㡣

- ��� $b_i=1$����ô $b_{i+1}=0$�������ֵı�ʾ���������������������������֡�

���������Ľ���� Byteazar ����Ϊ��Ҫ�ѣ����������������~��

����Ҫдһ������

��ȡ�����������ı�ʾ�����㲢���׼���д����͵ı�ʾ��

�����ʽ��

����ĵ�һ������һ����������Ϊ $x$ ��쳲�������ʾ�ĳ��ȣ��������������� $x$ ��쳲�������ʾ��

�ڶ��еĵ�һ������Ҳ��һ����������Ϊ $y$ ��쳲�������ʾ�ĳ��ȣ��������������� $y$ ��쳲�������ʾ��

�����ʽ�����ֻ��һ�г���Ӧд��$x+y$ �ĺ͵�쳲�������ʾ������������������ͬ���������һ�������� $n$ ����ʾ $x+y$ �ĺ͵�쳲�������ʾ�ĳ��ȣ�Ȼ������� $x+y$ �ĺ͵�쳲�������ʾ��

$1\leq n \leq 10^6$

## ��Ŀ����

Fibonacci numbers are an integer sequence defined in the following way: $Fib_0=1$, $Fib_1=1$, $Fib_i=Fib_{i-1}+Fib_{i-2}$ (for $i\ge 2$). The first few numbers in this sequence are: ($1,1,2,3,5,8,\cdots$).

The great computer scientist Byteazar is constructing an unusual computer, in which numbers are represented in Fibonacci system i.e. a bit string $(b_1,b_2,\cdots,b_n)$ denotes the number $b_1\cdot Fib_1+b_2\cdot Fib_2+\cdots+b_n\cdot Fib_n$. (Note that we do not use $Fib_0$.) Unfortunately, such a representation is ambiguous i.e. the same number can have different representations. The number $42$, for instance, can be written as: $(0,0,0,0,1,0,0,1)$, $(0,0,0,0,1,1,1,0)$ or $(1,1,0,1,0,1,1)$. For this very reason, Byteazar has limited himself to only using representations satisfying the following conditions:

if $n>1$, then $b_n=1$, i.e. the representation of a number does not contain leading zeros.

if $b_i=1$, then $b_{i+1}=0$ (for $i=1,\cdots,n-1$), i.e. the representation of a number does not contain two (or more) consecutive ones.

The construction of the computer has proved more demanding than Byteazar supposed. He has difficulties implementing addition. Help him!

TaskWrite a programme which:

reads from the standard input the representations of two positive integers,calculates and writes to the standard output the representation of their sum.

## �����ʽ

The input contains the Fibonacci representations (satisfying the aforementioned conditions) of two positive integers $x$ and $y$ - one in the first, the other in the second line. Each of these representations is in the form of a sequence of non-negative integers, separated by single spaces. The first number in the line denotes the length of the representation $n$, $1\le n\le 10^6$. It is followed by $n$ zeros and/or ones.

����ĵ�һ������һ����������Ϊ $x$ ��쳲�������ʾ�ĳ��ȣ��������������� $x$ ��쳲�������ʾ��

�ڶ��еĵ�һ������Ҳ��һ����������Ϊ $y$ ��쳲�������ʾ�ĳ��ȣ��������������� $y$ ��쳲�������ʾ��

## �����ʽ

In the first and only line of the output your programme should write the Fibonacci representation (satisfying the aforementioned conditions) of the sum $x+y$. The representation should be in the form of a sequence of non-negative integers, separated by single spaces, as it has been described in the Input section. The first number in the line denotes the length of the representation $n$, $1\le n\le 10^6$. It is followed by $n$ zeros and/or ones.

���ֻ��һ�г���Ӧд�� $x+y$ �ĺ͵�쳲�������ʾ������������������ͬ���������һ�������� $n$����ʾ $x+y$ �ĺ͵�쳲�������ʾ�ĳ��ȣ�Ȼ������� $x+y$ �ĺ͵�쳲�������ʾ��

��֤������������ݳ��ȶ������� $10^6$ Ҳ��С�� $1$;

## ��������
```plain
4 0 1 0 1
5 0 1 0 0 1
```


## �������
```plain
6 1 0 1 0 0 1
```