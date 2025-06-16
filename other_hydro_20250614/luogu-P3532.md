## ��Ŀ����
We consider the distance between positive integers in this problem, defined as follows.

A single operation consists in either multiplying a given number by a prime number1    or dividing it by a prime number (if it does divide without a remainder).

The distance between the numbers ![](http://main.edu.pl/images/OI19/odl-en-tex.1.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.2.png), denoted ![](http://main.edu.pl/images/OI19/odl-en-tex.3.png), is the minimum number of operations    it takes to transform the number ![](http://main.edu.pl/images/OI19/odl-en-tex.4.png) into the number ![](http://main.edu.pl/images/OI19/odl-en-tex.5.png).

For example, ![](http://main.edu.pl/images/OI19/odl-en-tex.6.png).

Observe that the function ![](http://main.edu.pl/images/OI19/odl-en-tex.7.png) is indeed a distance function - for any positive integers ![](http://main.edu.pl/images/OI19/odl-en-tex.8.png), ![](http://main.edu.pl/images/OI19/odl-en-tex.9.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.10.png) the following hold:

the distance between a number and itself is 0: ![](http://main.edu.pl/images/OI19/odl-en-tex.11.png),                  the distance from ![](http://main.edu.pl/images/OI19/odl-en-tex.12.png) to ![](http://main.edu.pl/images/OI19/odl-en-tex.13.png) is the same as from ![](http://main.edu.pl/images/OI19/odl-en-tex.14.png) to ![](http://main.edu.pl/images/OI19/odl-en-tex.15.png): ![](http://main.edu.pl/images/OI19/odl-en-tex.16.png), and                  the triangle inequality holds: ![](http://main.edu.pl/images/OI19/odl-en-tex.17.png).

A sequence of ![](http://main.edu.pl/images/OI19/odl-en-tex.18.png) positive integers, ![](http://main.edu.pl/images/OI19/odl-en-tex.19.png), is given.

For each number ![](http://main.edu.pl/images/OI19/odl-en-tex.20.png) we have to determine ![](http://main.edu.pl/images/OI19/odl-en-tex.21.png) such that ![](http://main.edu.pl/images/OI19/odl-en-tex.22.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.23.png) is minimal.

## �����ʽ
In the first line of standard input there is a single integer ![](http://main.edu.pl/images/OI19/odl-en-tex.24.png) (![](http://main.edu.pl/images/OI19/odl-en-tex.25.png)).

In the following ![](http://main.edu.pl/images/OI19/odl-en-tex.26.png) lines the numbers ![](http://main.edu.pl/images/OI19/odl-en-tex.27.png) (![](http://main.edu.pl/images/OI19/odl-en-tex.28.png)) are given,      one per line.

In tests worth 30% of total point it additionally holds that ![](http://main.edu.pl/images/OI19/odl-en-tex.29.png).


## �����ʽ
Your program should print exactly ![](http://main.edu.pl/images/OI19/odl-en-tex.30.png) lines to the standard output, a single integer in each line.

The ![](http://main.edu.pl/images/OI19/odl-en-tex.31.png)-th line should give the minimum ![](http://main.edu.pl/images/OI19/odl-en-tex.32.png) such that: ![](http://main.edu.pl/images/OI19/odl-en-tex.33.png), ![](http://main.edu.pl/images/OI19/odl-en-tex.34.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.35.png) is minimal.


## ��Ŀ����
### ��Ŀ����
**���� POI 2012 Stage 1. ��[Distance](https://szkopul.edu.pl/problemset/problem/Phel_x2Ny30OUh7z1RhCtzEG/site/?key=statement)��**

����һ�Ρ�������Ϊ��һ�����������Ի����һ�����������庯�� $d(a,b)$ ��ʾ�� $a$ �������ɴΡ���������� $b$ ����Ҫ����С�������������磬$d(69,42)=3$.

$d$ ��Ȼ��һ�����뺯���������������ʣ�
* $d(a,a) = 0$
* $d(a,b) = d(b,a)$
* $d(a,b) + d(b,c) \ge d(a,c)$

���� $n$ �������� $a_1, a_2, \ldots, a_n$����ÿ�� $a_i (1 \le i \le n)$���� $j$ ʹ�� $j \neq i$ �� $d(a_i,a_j)$ ��С������ж������������ $j$��Ӧ�����С���Ǹ���

### �����ʽ

��һ��һ�������� $n (2 \le n \le 100,000)$.

�ڶ��� $n$ �������� $a_1, a_2, \ldots, a_n (1 \le a_i \le 1\ 000\ 000)$.

### �����ʽ

��� $n$ �У�ÿ��һ����������ʾʹ $j \neq i$ �� $d(a_i,a_j)$ ��С�� $j$.

### ���ݷ�Χ

���� $30\%$ �������� $n \le 1000$.

�������������� $2 \le n \le 10^5,1 \le a_i \le 10^6$.

���������� [LibreOJ](https://loj.ac/p/2690)��

```input1
6
1
2
3
4
5
6
```

```output1
2
1
1
2
1
2
```

