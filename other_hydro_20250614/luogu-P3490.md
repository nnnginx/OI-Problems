## ��Ŀ����
The following task is a significantly harder version of task Words from the third stage of 16th Polish OI. It wasn't used in the contest itself, but is an extension for those who solved "Words" and want more. :-)    Let ![](http://main.edu.pl/images/OI16/fib-en-tex.1.png) be a function acting on strings composed of the digits 0    and 1.

The function ![](http://main.edu.pl/images/OI16/fib-en-tex.2.png) transforms the string ![](http://main.edu.pl/images/OI16/fib-en-tex.3.png) by replacing (independently    and concurrently) every digit 0 with 1 and every digit    1 with the string ![](http://main.edu.pl/images/OI16/fib-en-tex.4.png).

For example ![](http://main.edu.pl/images/OI16/fib-en-tex.5.png), ![](http://main.edu.pl/images/OI16/fib-en-tex.6.png)    (i.e. ![](http://main.edu.pl/images/OI16/fib-en-tex.7.png) assigns an empty string to the empty string).

Note that ![](http://main.edu.pl/images/OI16/fib-en-tex.8.png) is an injection, or a one-to-one function.

By ![](http://main.edu.pl/images/OI16/fib-en-tex.9.png) we denote the function ![](http://main.edu.pl/images/OI16/fib-en-tex.10.png) composed with itself ![](http://main.edu.pl/images/OI16/fib-en-tex.11.png) times.

In particular, ![](http://main.edu.pl/images/OI16/fib-en-tex.12.png) is the identity function ![](http://main.edu.pl/images/OI16/fib-en-tex.13.png).

We are interested in the strings of the form ![](http://main.edu.pl/images/OI16/fib-en-tex.14.png)    for ![](http://main.edu.pl/images/OI16/fib-en-tex.15.png) This sequence begins with the following strings:

![](http://main.edu.pl/images/OI16/fib-en-tex.16.png), ![](http://main.edu.pl/images/OI16/fib-en-tex.17.png), ![](http://main.edu.pl/images/OI16/fib-en-tex.18.png), ![](http://main.edu.pl/images/OI16/fib-en-tex.19.png),    ![](http://main.edu.pl/images/OI16/fib-en-tex.20.png), ![](http://main.edu.pl/images/OI16/fib-en-tex.21.png).

We call the string ![](http://main.edu.pl/images/OI16/fib-en-tex.22.png) a substring of the string ![](http://main.edu.pl/images/OI16/fib-en-tex.23.png) if it occurs    in ![](http://main.edu.pl/images/OI16/fib-en-tex.24.png) as  a contiguous (i.e. one-block) subsequence.

A sequence of integers ![](http://main.edu.pl/images/OI16/fib-en-tex.25.png) is given.

Your task is to check whether a string of the form    ![](http://main.edu.pl/images/OI16/fib-en-tex.26.png)    is a substring of ![](http://main.edu.pl/images/OI16/fib-en-tex.27.png) for some ![](http://main.edu.pl/images/OI16/fib-en-tex.28.png), and if it is,    you shuold find minimal such ![](http://main.edu.pl/images/OI16/fib-en-tex.29.png).


## �����ʽ
The first line of the standard input contains a single integer ![](http://main.edu.pl/images/OI16/fib-en-tex.30.png),      ![](http://main.edu.pl/images/OI16/fib-en-tex.31.png).

The second line of standard input holds ![](http://main.edu.pl/images/OI16/fib-en-tex.32.png) non-negative integers      ![](http://main.edu.pl/images/OI16/fib-en-tex.33.png)(![](http://main.edu.pl/images/OI16/fib-en-tex.34.png)), separated by single spaces.


## �����ʽ
Your programme should print out ![](http://main.edu.pl/images/OI16/fib-en-tex.35.png) lines to the standard output,     one for each test unit.

Your programm should print to standard output minimal non-negative integer ![](http://main.edu.pl/images/OI16/fib-en-tex.36.png),     such that ![](http://main.edu.pl/images/OI16/fib-en-tex.37.png) is a substring of      ![](http://main.edu.pl/images/OI16/fib-en-tex.38.png), or NIE (no in Polish) if such ![](http://main.edu.pl/images/OI16/fib-en-tex.39.png) doesn't exist.


## ��Ŀ����
## ��Ŀ����
����������ǵ�16�첨���ﾺ�������׶ε����񡰵��ʡ���һ�����Ե��Ѷ���ǿ�汾������û���ڱ�����ʹ�ã���������Щ����ˡ����ʡ�������˵������һ����չ :) ��

����  $h$ ������������  $0$ ��  $1$ ��ɵ��ַ�������ͨ����ÿһ������  $0$ �滻Ϊ  $1$����ÿһ������  $1$ �滻Ϊ�ַ���  $10$ ��������ͬʱ�ر任�ַ���  $w$��

���磺

 $$h(``1001")=``101110"$$
 $$h(``\ ")=``\ "$$

�����������ѿ��ַ�����ֵ�����ַ�����

ע�⣬ $h$ ��һ��һ��һ�ĺ�����

������  $h^k$ ��ʾ����  $h$ ʹ��  $k$ �Ρ�

�ر�ģ� $h^0(w)=w$�� 

���Ƕ�  $k = 0, 1, 2, ...$ ��  $h^k(``0")$ ��ʽ���ַ�������Ȥ���������Ϊ:

 $$ ``0", ``1", ``10", ``101", ``10110", ``10110101", \ldots $$

����ַ���  $x$ ��  $y$ ����һ�������ģ���һ���飩�Ӵ����֣����Ǿͳ�  $x$ Ϊ�ַ���  $y$ ���Ӵ�����������  $k_1, k_2, k_3, ..., k_n $ �����С���������Ǽ�����һЩ  $m$ ��˵�� $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ ��ʽ���ַ����Ƿ���  $h^m(``0")$ ���Ӵ�������У���Ӧ���ҵ���С��  $m$�� 

## ��������
����ĵ�һ�а���һ������  $n$�� $1 \leq n \leq 1000000$������ĵڶ��а���  $n$ ���Ǹ�����  $k_1, k_2, k_3, ..., k_n $���õ����ո�ָ���

## �������
���ĳ���Ӧ�����  $t$ �У�ÿ���������һ�С���ĳ���Ӧ���������С�Ǹ�����  $m$��ʹ  $h^{k_1}(``0") \cdot h^{k_2}(``0") \cdot \ldots \cdot h^{k_n}(``0") $ ��  $h^m(``0")$ ���Ӵ������������  $m$������� `NIE`���������е� _no_ ����

_Translated By in\_young\_ren_ 

```input1
2
1 2

```

```output1
4

```

