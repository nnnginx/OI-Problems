## ��Ŀ����
Byteasar once decided to start manufacturing necklaces.

He subsequently bought a very long string of colourful coral beads for a bargain price.

Byteasar now also has a machine that, for a given ![](http://main.edu.pl/images/OI17/kor-en-tex.1.png) (![](http://main.edu.pl/images/OI17/kor-en-tex.2.png)), can cut the string    into pieces (or substrings) of ![](http://main.edu.pl/images/OI17/kor-en-tex.3.png) coral beads (i.e., the first piece consists of the beads no.

![](http://main.edu.pl/images/OI17/kor-en-tex.4.png), the second of ![](http://main.edu.pl/images/OI17/kor-en-tex.5.png), etc.).

If the length of the string (measured in coral beads) is not a multiple of ![](http://main.edu.pl/images/OI17/kor-en-tex.6.png),    then the last piece is not used, as it has length smaller than ![](http://main.edu.pl/images/OI17/kor-en-tex.7.png).

From now on we denote the colours of the beads with positive integers.

Byteasar, always praising diversity, wonders how he should choose the number ![](http://main.edu.pl/images/OI17/kor-en-tex.8.png)    in order to get as many different substrings as possible.

The ends of the long string that will be cut are different: there are specific    beginning and ending (rather than two interchangeable endpoints), and the machine    of course starts cutting at the beginning. On the other hand, in the substrings    obtained from cutting the endpoints are interchangeable, and so the substrings    can be reversed. In other words, the substrings ![](http://main.edu.pl/images/OI17/kor-en-tex.9.png) and ![](http://main.edu.pl/images/OI17/kor-en-tex.10.png) are    identical to us. Write a program that determines the optimum value of ![](http://main.edu.pl/images/OI17/kor-en-tex.11.png) for Byteasar.

## �����ʽ
In the first line of the standard input there is an integer ![](http://main.edu.pl/images/OI17/kor-en-tex.37.png)      (![](http://main.edu.pl/images/OI17/kor-en-tex.38.png)) denoting the length of the string to cut.

In the second line there are ![](http://main.edu.pl/images/OI17/kor-en-tex.39.png) positive integers ![](http://main.edu.pl/images/OI17/kor-en-tex.40.png)      (![](http://main.edu.pl/images/OI17/kor-en-tex.41.png)), separated by single spaces, that denote      the colours of successive beads in Byteasar's string.


## �����ʽ
Two integers, separated by a single space, should be printed out to the first line of the standard ouput:

the (maximum) number of different substrings that can be obtained with an optimal choice    of parameter ![](http://main.edu.pl/images/OI17/kor-en-tex.42.png), and the number ![](http://main.edu.pl/images/OI17/kor-en-tex.43.png) of such optimal values of ![](http://main.edu.pl/images/OI17/kor-en-tex.44.png).

The second line should contain ![](http://main.edu.pl/images/OI17/kor-en-tex.45.png) integers separated by single spaces:

the values of parameter ![](http://main.edu.pl/images/OI17/kor-en-tex.46.png) that yield an optimum solution;    these can be given in arbitrary order.

������У���һ�е�һ����Ϊ�����Եõ��Ĳ�ͬ�Ӵ��ĸ������ڶ�����Ϊȡ�����Ž�ʱ�Ĳ�ͬ��k�ĸ������ڶ��а������ɸ�����Ϊȡ�����Ž�ʱ�Ĳ�ͬ��k ���ڶ����еĲ�ͬ��k���԰�����λ�������


## ��Ŀ����
### ����Ŀ������

Byteasar �� $n$ �����ӣ��� $i$ ����ɫΪ $a_i$����һ̨������

Byteasar ����ѡ��һ��ֵ $k$��Ȼ��������� $1\sim k$ ������������� $b_1$��$k+1\sim 2k$ ������������� $b_2$���Դ����ƣ�**��� $n\bmod k$ �����Ӳ���������������Ǳ�����**��

�����������һ�� $k$ ֵ��ʹ���� $\left\lfloor\dfrac{n}{k}\right\rfloor$ ������ $b$ �У����� **��ͬ��** ����������ࡣ

�������Է�ת����ʽ���أ�$b_x$ �� $b_y$ ��ͬ�����ҽ�����������һ�� $i$��ʹ�� $b_{x,i}\ne b_{y,i}$ �� $b_{x,i} \ne b_{y,k-i+1}$��

���� $[1,2,3]$ �� $[3,2,1]$ ����ͬ�ģ��� $[1,2,3]$ �� $[2,3,1]$ �ǲ�ͬ�ġ�

### �������ʽ��

�������У���һ��Ϊ $n$��

�ڶ���Ϊ $n$ ������������ $i$ ������������ $a_i$��

### �������ʽ��

������С�

��һ�������������ֱ����ͬ�����������������Լ���ͬ���������ʱ��$k$ �ĸ�����

�ڶ������ɸ�����������������ʹ��ͬ���������� $k$ ֵ������԰�����˳�������

### ���������͡�

$a$ Ϊ $[1,1,1,2,2,2,3,3,3,1,2,3,3,1,2,2,1,3,3,2,1]$��

- $k=1$ ��ʱ�����ǵõ� $3$ ����ͬ������ $b$��$[1],[2],[3]$��
- $k=2$ ��ʱ�����ǵõ� $6$ ����ͬ��������$[1,1],[1,2],[2,2],[2,3],[3,3],[3,1]$��
- $k=3$ ��ʱ�����ǵõ� $5$ ����ͬ��������$[1,1,1],[2,2,2],[3,3,3],[1,2,3],[3,1,2]$��
- $k=4$ ��ʱ�����ǵõ� $5$ ����ͬ��������$[1,1,1,2],[2,2,3,3],[3,1,2,3],[3,1,2,2],[1,3,3,2]$��

### �����ݷ�Χ��

����ȫ�����ݣ�$1\le n\le2\times 10^5$���� $\forall 1\le i\le n$���� $1\le a_i\le n$��

```input1
21
1 1 1 2 2 2 3 3 3 1 2 3 3 1 2 2 1 3 3 2 1
```

```output1
6 1
2
```

## ��ʾ
$1��n��2\times 10^5$���� $\forall 1\le i\le n$���� $1\le a_i\le n$

