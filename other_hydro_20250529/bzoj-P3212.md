## ��Ŀ����

You have $n$ integers, $A_1, A_2, ... , A_n$. You need to deal with two kinds of operations.

One type of operation is to add some given number to each number in a given interval.

The other is to ask for the sum of numbers in a given interval.

## �����ʽ

The first line contains two numbers $n$ and $q$. $(1 \leq n,q \leq 10^5)$

The second line contains $n$ numbers, the initial values of $A_1, A_2, ... , A_n$. $(-10^9 \leq A_i \leq 10^9)$

Each of the next $q$ lines represents an operation.

* `C a b c` means adding $c$ to each of $A_a, A_{a+1}, ... , A_b$. $(-10^4 \leq c \leq 10^4)$

* `Q a b` means querying the sum of $A_a, A_{a+1}, ... , A_b$.

## �����ʽ

You need to answer all $q$ commands in order. One answer in a line.


```input1
10 5
1 2 3 4 5 6 7 8 9 10
Q 4 4
Q 1 10
Q 2 4
C 3 6 3
Q 2 4
```

```output1
4
55
9
15
```

## ���ݹ�ģ��Լ��

* $1 \leq n,q \leq 10^5$, $-10^9 \leq A_i \leq 10^9$, $-10^4 \leq c \leq 10^4$.

## ��ʾ

The sums may exceed the range of 32-bit integers.