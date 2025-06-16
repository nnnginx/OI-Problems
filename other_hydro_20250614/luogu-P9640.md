## ��Ŀ����
Let $m(x)$ be the $\textit{mode}$ of the digits in decimal representation of positive integer $x$. The mode is the largest value that occurs most frequently in the sequence. For example, $m(15532)=5$, $m(25252)=2$, $m(103000)=0$, $m(364364)=6$, $m(114514)=1$, $m(889464)=8$.

Given a positive integer $n$, DreamGrid would like to know the value of $(\sum\limits_{x=1}^{n} m(x)) \bmod (10^9+7)$.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains a positive integer $n$ ($1 \le n < 10^{50}$) without leading zeros.

It's guaranteed that the sum of $|n|$ of all test cases will not exceed $50$, where $|n|$ indicates the number of digits of $n$ in decimal representation.

## �����ʽ
For each test case output one line containing one integer, indicating the value of $(\sum\limits_{x=1}^{n} m(x)) \bmod (10^9+7)$.

## ��Ŀ����
�� $m(x)$ �������� $x$ ��ʮ�����е� $mode$��$mode$ �� $x$ ����Ƶ�����ֵ����ֵ������ $m(15532)=5,m(25252)=2,m(103000)=0,m(364364)=6,m(114514)=1,m(889464)=8$��

����һ�������� $n$��DreamGrid ϣ��֪�� $(\sum\limits_{x=1}^n m(x)) \mod (10^9+7)$ ��ֵ��

```input1
5
9
99
999
99999
999999
```

```output1
45
615
6570
597600
5689830
```

