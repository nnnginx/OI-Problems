## ��Ŀ����
This task is a harder version of task Monotonicity from the third stage of 17th Polish OI. It wasn't used in the contest itself.

For an integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.1.png) we define its monotonicity scheme as the sequence    ![](http://main.edu.pl/images/OI17/mot-en-tex.2.png) of symbols ![](http://main.edu.pl/images/OI17/mot-en-tex.3.png), ![](http://main.edu.pl/images/OI17/mot-en-tex.4.png) or ![](http://main.edu.pl/images/OI17/mot-en-tex.5.png).

The symbol ![](http://main.edu.pl/images/OI17/mot-en-tex.6.png) represents the relation between ![](http://main.edu.pl/images/OI17/mot-en-tex.7.png) and ![](http://main.edu.pl/images/OI17/mot-en-tex.8.png).

For example, the monotonicity scheme of the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.9.png) is ![](http://main.edu.pl/images/OI17/mot-en-tex.10.png).

We say that an integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.11.png) with monotonicity scheme    ![](http://main.edu.pl/images/OI17/mot-en-tex.12.png), realizes another monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.13.png)    if for every ![](http://main.edu.pl/images/OI17/mot-en-tex.14.png) it holds that ![](http://main.edu.pl/images/OI17/mot-en-tex.15.png).

In other words, the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.16.png) can be obtained by repeating the sequence    ![](http://main.edu.pl/images/OI17/mot-en-tex.17.png) and removing appropriate suffix from that repetition.

For example, the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.18.png) realizes each and every one of the following schemes:

![](http://main.edu.pl/images/OI17/mot-en-tex.19.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.20.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.21.png)           ![](http://main.edu.pl/images/OI17/mot-en-tex.22.png)                  as well as many others.

An integer sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.23.png) and a monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.24.png) are given.

Your task is to find the longest subsequence ![](http://main.edu.pl/images/OI17/mot-en-tex.25.png) (![](http://main.edu.pl/images/OI17/mot-en-tex.26.png))    of the former that realizes the latter.

## �����ʽ
The first line of the standard input holds two integers ![](http://main.edu.pl/images/OI17/mot-en-tex.27.png) and ![](http://main.edu.pl/images/OI17/mot-en-tex.28.png) (![](http://main.edu.pl/images/OI17/mot-en-tex.29.png), ![](http://main.edu.pl/images/OI17/mot-en-tex.30.png)),    separated by a single space, denoting the lengths of the sequences ![](http://main.edu.pl/images/OI17/mot-en-tex.31.png) and monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.32.png) respectively.

The second input line gives the sequence ![](http://main.edu.pl/images/OI17/mot-en-tex.33.png), i.e, it holds ![](http://main.edu.pl/images/OI17/mot-en-tex.34.png) integers ![](http://main.edu.pl/images/OI17/mot-en-tex.35.png) separated by single spaces (![](http://main.edu.pl/images/OI17/mot-en-tex.36.png)).

Finally, the third lines gives the monotonicity scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.37.png), i.e., it holds ![](http://main.edu.pl/images/OI17/mot-en-tex.38.png) s��


## �����ʽ
In the first line of the standard output your program should print out a single integer ![](http://main.edu.pl/images/OI17/mot-en-tex.40.png),    the maximum length of a subsequence of ![](http://main.edu.pl/images/OI17/mot-en-tex.41.png) that realizes the scheme ![](http://main.edu.pl/images/OI17/mot-en-tex.42.png).

In the second line it should print out any such subsequence ![](http://main.edu.pl/images/OI17/mot-en-tex.43.png), separating its elements by single spaces.


## ��Ŀ����
### ��Ŀ����

���������� POI 2010 �����׶ε�[������](https://www.luogu.com.cn/problem/P3541)һ��ļ�ǿ�棬����û�����Ǵα����б�ʹ�á�

**���� POI 2010 ��[Monotonicity 2](https://szkopul.edu.pl/problemset/problem/0_pcwjQ6no8LDss0IWNLbb2_/site/?key=statement)��**

����һ���������� $a_1, a_2, ..., a_n$�����Ƕ����䡰��������"Ϊһ���� $<$��$>$ �� $=$ ��ɵķ������� $s_1, s_2, ... s_{n-1}$�����з��� $s_i$ ��ʾ $a_i$ �� $a_{i+1}$ ֮��Ĺ�ϵ�����磬���� $2, 4, 3, 3, 5, 3$ �ĵ�������Ϊ $<, >, =, <, >$��

������������ $b_1, b_2, ..., b_{n+1}$ �Լ��䵥������ $s_1, s_2, ..., s_n$������������� $s_1', s_2', ..., s_k'$ ��������� $1 \le i \le n$ �� $s_i = s_{((i - 1) \bmod n) + 1}'$�����Ǿ�˵���� $s_1, s_2, ..., s_n$ ��ʵ�֡������� $s_1', s_2', ..., s_k'$��Ҳ����˵������ $s_1, s_2, ..., s_n$ ����ͨ���ظ���� $s_1', s_2', ..., s_k'$ ���в�ɾ��һ����׺�õ������磬�������� $2, 4, 3, 3, 5, 3$ ����ʵ�������·������У�
* $<, >, =$
* $<, >, =, <, >$
* $<, >, =, <, >, <, <, =$
* $<, >, =, <, >, =, >, >$

����һ���������� $a_1, a_2, ..., a_n$ �Լ�һ���������� $s_1, s_2, ..., s_k$�����ԭ����������������� $a_{i_1}, a_{i_2}, ..., a_{i_m} (1 \le i_1 \lt i_2 \lt ... \lt i_m \le n)$ ʹ��ǰ�ߵĵ�������ʵ�ֺ��ߵķ������С�

### �����ʽ

��һ�а����ÿո�ָ����������� $n,k$���ֱ��ʾ�������� $(a_i)$ �ĳ��Ⱥ͵������� $(s_j)$ �ĳ��ȡ�

�ڶ��а����ÿո�ָ��� $n$ ����������ʾ���� $a_i$.

�����а����ÿո�ָ��� $k$ �����ţ���ʾ�������� $s_j$.

### �����ʽ

��һ�����һ������ $m$����ʾ���� $a_1, a_2, ..., a_n$ ����ġ�ʵ�֡��˵������� $s_1, s_2, ..., s_n$ �������С�

�ڶ����������һ�������������� $a_{i_1}, a_{i_2}, ..., a_{i_n}$��Ԫ��֮���ÿո�ָ���

### ���ݷ�Χ

���� $100\%$ �����ݣ� $1 \le n \le 500000,1 \le k \le 500000 , 1 \le a_i \le 1000000 , s_j \in \{<, >, =\}$ ��

��л [����](https://www.luogu.com.cn/discuss/67056) �ṩ�� SPJ������������ [LibreOJ](https://loj.ac/p/3009)��

```input1
7 3
2 4 3 1 3 5 3
< > =
```

```output1
6
2 4 3 3 5 3
```

