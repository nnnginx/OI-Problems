## ��Ŀ����
Consider $n$ segments on the number axis, where the left endpoint of the $i$-th segment is $l_i$ and the right endpoint is $r_i$. Each segment has a color where the color of the $i$-th segment is $c_i$ ($0 \le c_i \le 1$). There are two types of colors, where $c_i = 0$ indicates a red segment and $c_i = 1$ indicates a blue segment.

You need to choose some segments (you can also choose no segments at all). If any two chosen segments overlap, then they must have the same color.

Calculate the number of ways to choose segments.

We say segment $i$ overlaps with segment $j$, if there exists a real number $x$ satisfying both $l_i \le x \le r_i$ and $l_j \le x \le r_j$.

We say two ways of choosing segments are different, if there exists an integer $1 \le k \le n$ such that the $k$-th segment is chosen in one of the ways and is not chosen in the other.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$) indicating the number of segments.

For the following $n$ lines, the $i$-th line contains three integers $l_i$, $r_i$ and $c_i$ ($1 \le l_i \le r_i \le 10^9$, $0 \le c_i \le 1$) indicating the left and right endpoints and the color of the $i$-th segment.

It's guaranteed that the sum of $n$ of all test cases will not exceed $5 \times 10^5$.

## �����ʽ
For each test case output one line containing one integer indicating the number of ways to choose segments. As the answer may be large, please output the answer modulo $998244353$.


## ��Ŀ����
**����Ŀ������**

���������ϵ� $n$ ���߶Σ����е� $i$ ���߶ε���˵�Ϊ $l_i$���Ҷ˵�Ϊ $r_i$��ÿһ���߶ζ���Ϳ������ɫ�����е� $i$ ���߶ε���ɫΪ $c_i$��$0 \le c_i \le 1$������ɫ�������֣�$c_i = 0$ ����һ����ɫ���߶Σ��� $c_i = 1$ ����һ����ɫ���߶Ρ�

����Ҫѡ���������߶Σ����Բ�ѡ���κ��߶Σ��������ѡ������������߶����غϣ����������߶ε���ɫ������ͬ��

��ѡ���߶εĲ�ͬ��������

�Ƶ� $i$ ���߶κ͵� $j$ ���߶����غϣ�������һ��ʵ�� $x$ ͬʱ���� $l_i \le x \le r_i$ �� $l_j \le x \le r_j$��

������ѡ���߶εķ����ǲ�ͬ�ģ�������һ������ $1 \le k \le n$������� $k$ ���߶�������һ�������б�ѡ�񣬶�����һ��������û�б�ѡ��

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ������һ������ $n$��$1 \le n \le 10^5$����ʾ�߶ε�������

���ڽ����� $n$ �У��� $i$ �������������� $l_i$��$r_i$ �� $c_i$��$1 \le l_i \le r_i \le 10^9$��$0 \le c_i \le 1$����ʾ�� $i$ ���߶ε����Ҷ˵��Լ���ɫ��

��֤�������� $n$ ֮�Ͳ����� $5 \times 10^5$��

**�������ʽ��**

ÿ���������һ��һ��������ʾѡ���߶εĲ�ͬ�����������ڴ𰸿��ܴܺ��뽫�𰸶� $998244353$ ȡģ�������

**���������͡�**

���ڵ�һ���������ݣ�������ͬʱѡ��� $1$ �͵� $2$ ���߶Σ�Ҳ����ͬʱѡ��� $2$ �͵� $3$ ���߶Σ���Ϊ�������غ�����ɫ��ͬ��

���ڵڶ����������ݣ���Ϊ�� $2$ ���߶���� $1$ �͵� $3$ ���߶ζ����غϣ��������������ѡ���߶Ρ�

```input1
2
3
1 5 0
3 6 1
4 7 0
3
1 5 0
7 9 1
3 6 0
```

```output1
5
8
```

## ��ʾ
For the first sample test case, you cannot choose the $1$-st and the $2$-nd segment, or the $2$-nd and the $3$-rd segment at the same time, because they overlap with each other and have different colors.

For the second sample test case, as the $2$-nd segment does not overlap with the $1$-st and the $3$-rd segment, you can choose them arbitrary.

