## ��Ŀ����
Given an integer sequence $a_1, a_2, \cdots, a_n$ of length $n$, we construct an undirected graph $G$ from the sequence. More precisely, for all $1 \le i < j \le n$, if $i - j = a_i - a_j$, there will be an undirected edge in $G$ connecting vertices $i$ and $j$. The weight of the edge is $(a_i + a_j)$.

Find a matching of $G$ so that the sum of weight of all edges in the matching is maximized, and output this maximized sum.

Recall that a matching of an undirected graph means that we choose some edges from the graph such that any two edges have no common vertices. Specifically, not choosing any edge is also a matching.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($2 \le n \le 10^5$) indicating the length of the sequence.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($-10^9 \le a_i \le 10^9$) indicating the sequence.

It's guaranteed that the sum of $n$ of all test cases will not exceed $5 \times 10^5$.

## �����ʽ
For each test case output one line containing one integer indicating the maximum sum of weight of all edges in a matching.

## ��Ŀ����
**����Ŀ������**

��������Ϊ $n$ ���������� $a_1, a_2, \cdots, a_n$�����ǽ��Ӹ������й����һ������ͼ $G$��������˵���������� $1 \le i < j \le n$���� $i - j = a_i - a_j$���� $G$ �н�����һ�����ӽڵ� $i$ �� $j$ ������ߣ����ȨΪ $(a_i + a_j)$��

�� $G$ ��һ��ƥ�䣬ʹ�ø�ƥ�������бߵı�Ȩ֮����󣬲��������Ȩ֮�͡�

����䣺����ͼ��ƥ�䣬ָ���ǴӸ�����ͼ��ѡ��һЩ�ߣ�ʹ�����������߶�û�й����Ľڵ㡣�ر�أ���ѡ�κα�Ҳ��һ��ƥ�䡣

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ������һ������ $n$��$2 \le n \le 10^5$����ʾ���еĳ��ȡ�

�ڶ������� $n$ ������ $a_1, a_2, \cdots, a_n$��$-10^9 \le a_i \le 10^9$����ʾ���С�

��֤���������� $n$ ֮�Ͳ����� $5 \times 10^5$��

**�������ʽ��**

ÿ���������һ��һ����������ʾƥ�������Ȩ֮�͡�

**���������͡�**

���ڵ�һ���������ݣ����ŷ�����ѡ�����ӽڵ� $3$ �� $5$���ڵ� $4$ �� $7$���Լ��ڵ� $8$ �� $9$ �������ߣ���Ȩ֮��Ϊ $(5 + 7) + (6 + 9) + (1 + 2) = 30$��

���ڵڶ����������ݣ�����ÿ���ߵı�Ȩ���Ǹ������������ƥ�䲻Ӧ��ѡ���καߣ���Ϊ $0$��

���ڵ������������ݣ�����ͼ�в������καߣ���˴�Ϊ $0$��

```input1
3
9
3 -5 5 6 7 -1 9 1 2
3
-5 -4 -3
3
1 10 100

```

```output1
30
0
0

```

## ��ʾ
For the first sample test case, the optimal choice is to choose the three edges connecting vertex $3$ and $5$, vertex $4$ and $7$, and finally vertex $8$ and $9$. The sum of weight is $(5 + 7) + (6 + 9) + (1 + 2) = 30$.

For the second sample test case, as all edges have negative weights, the optimal matching should not choose any edge. The answer is $0$.

For the third sample test case, as there is no edge in the graph, the answer is $0$.

