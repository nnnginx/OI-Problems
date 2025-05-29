## ��Ŀ����
Little Bytie loves to play with colorful chains.

He already has quite an impressive collection, and some of them he likes    more than the others.

Each chain consists of a certain number of colorful links.

Byteasar has noticed that Bytie's sense of aesthetics is very precise.

It turns out that Bytie finds a contiguous fragment of a chain nice if    it contains exactly    ![](http://main.edu.pl/images/OI20/lan-en-tex.1.png) links of color ![](http://main.edu.pl/images/OI20/lan-en-tex.2.png) links of color ![](http://main.edu.pl/images/OI20/lan-en-tex.3.png) links of color ![](http://main.edu.pl/images/OI20/lan-en-tex.4.png),    and moreover it contains no links of other colors.

A chain's appeal is its number of (contiguous) fragments that are nice.

By trial and error, Byteasar has determined the values ![](http://main.edu.pl/images/OI20/lan-en-tex.5.png) and ![](http://main.edu.pl/images/OI20/lan-en-tex.6.png).

Now he would like to buy a new chain, and therefore asks you to write a program to aid him in shopping.

����һ������Ϊ $n$ ������ $a$ �� $m$ ��������ÿ�������а����� $c_i$ ��ֵ $l_i$����Ҫ���ҳ����������������Ӵ��������������

 + �����д��ڼ� $c_i$ �ģ�Ҫ���Ӵ��� $c_i$ ǡ�ó��� $l_i$ �Ρ�

 + �����в����ڼ� $c_i$ �ģ�Ҫ���Ӵ��в����� $c_i$��

������ $n$ �� $m$�������� $m$ �������� $l_i$��Ȼ������ $m$ �������� $c_i$��������� $a_i$��

## �����ʽ
The first line of the standard input gives two integers, ![](http://main.edu.pl/images/OI20/lan-en-tex.7.png) and ![](http://main.edu.pl/images/OI20/lan-en-tex.8.png)      (![](http://main.edu.pl/images/OI20/lan-en-tex.9.png)), separated by a single space.

These are the length of the chain and the length of a nice fragment's description.

The second line gives ![](http://main.edu.pl/images/OI20/lan-en-tex.10.png) integers, ![](http://main.edu.pl/images/OI20/lan-en-tex.11.png) (![](http://main.edu.pl/images/OI20/lan-en-tex.12.png)),      separated by single spaces.

The third line gives ![](http://main.edu.pl/images/OI20/lan-en-tex.13.png) integers, ![](http://main.edu.pl/images/OI20/lan-en-tex.14.png)      (![](http://main.edu.pl/images/OI20/lan-en-tex.15.png), ![](http://main.edu.pl/images/OI20/lan-en-tex.16.png) for ![](http://main.edu.pl/images/OI20/lan-en-tex.17.png)), also separated by single spaces.

The sequences ![](http://main.edu.pl/images/OI20/lan-en-tex.18.png) and ![](http://main.edu.pl/images/OI20/lan-en-tex.19.png) define a nice fragment of a chain - it has to contain exactly ![](http://main.edu.pl/images/OI20/lan-en-tex.20.png) links of color ![](http://main.edu.pl/images/OI20/lan-en-tex.21.png).

The fourth line gives ![](http://main.edu.pl/images/OI20/lan-en-tex.22.png) integers, ![](http://main.edu.pl/images/OI20/lan-en-tex.23.png) (![](http://main.edu.pl/images/OI20/lan-en-tex.24.png)),      separated by single spaces, that are the colors of successive links of      the chain.

In tests worth 50% of total points the constraint ![](http://main.edu.pl/images/OI20/lan-en-tex.25.png) holds in addition.


## �����ʽ
Your program is to print a single integer, the number of nice contiguous    fragments in the chain, to the first and only line of the standard output.


```input1
7 3
2 1 1
1 2 3
4 2 1 3 1 2 5

```

```output1
2

```

## ��ʾ


### ���ݷ�Χ��

���� $100\%$ �����ݣ�$1\leq m\leq n \leq 10^6$��$1\leq a_i,b_i,c_i\leq n$��

