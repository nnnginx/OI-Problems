## ��Ŀ����
You are given an undirected weighted graph $G$ with vertices $1, 2, \ldots, n$. Please output the sum of the answers to the following $x$ questions:
- The $i$-th question $(1\le i\le x$): What is the minimum length of path that starts at vertex $1$, ends at vertex $n$, and contains exactly $i$ edges?

For each question, if such a path does not exist, the answer is considered to be $0$. A path may use one edge multiple times. Output the answer modulo $998244353$. 


## �����ʽ
The first line contains one integer $T~(1 \le T\le 2000)$, the number of test cases.

For each test case, the first line contains three integers $n, m, x~(1\le n\le 2000, 0\le m\le 5000, 1\le x\le 10^9)$. Each of the next $m$ lines describes an edge of the graph. Edge $i$ is denoted by three integers $a_i, b_i, w_i$ $(1\le a_i, b_i\le n, 1\le w_i\le 10^9)$, the labels of vertices it connects and its weight. Note that self-loops and parallel edges may exist.

It is guaranteed that the sum of $n$ over all test cases is no more than $2000$ and the sum of $m$ over all test cases is no more than $5000$.

## �����ʽ
For each test case, output one integer modulo $998244353$ denoting the answer.

## ��Ŀ����
### ��Ŀ����

����һ�� $n$ ���� $m$ ���ߵ�����ͼ $G$�����б�Ȩ����Ҫ�ش� $x$ �����⣬���е� $i$ $(1\leqslant i\leqslant x)$ ���������磺

- �ӽ�� $1$ ���������� **ǡ��** $i$ ���ߣ������� $n$ �����·������Ϊ���٣�

����ÿ��ѯ�ʣ���������������·������Ӧ��Ϊ $0$��һ��·������ **���** ����һ���ߡ�

����� $x$ ����������Ӧ�Ĵ�֮�͡�����𰸶� $998244353$ ȡģ��Ľ����

### �����ʽ

��һ�а���һ������ $T$ $(1\leqslant T\leqslant 2000)$����ʾ��������������

����ÿ��������ݣ�

��һ���������� $n,m,x$ $(1\leqslant n\leqslant 2000,0\leqslant m\leqslant 5000,1\leqslant x\leqslant 10^9)$��

������ $m$ �У�ÿ���������� $a_i,b_i,w_i$ $(1\leqslant a_i,b_i\leqslant n,1\leqslant w_i\leqslant 10^9)$���ֱ��ʾ�� $i$ �������ӵ��������ı�ź����Ȩ��ע�� **���ܴ����Ի����ر�**��

��֤���в��������� $n$ ���ܺͲ����� $2000$���� $m$ ���ܺͲ����� $5000$��

### �����ʽ

����ÿ��������ݣ��������������ݶ�Ӧ�Ĵ� $\bmod$ $998244353$ ��Ľ����

```input1
4
3 2 10
1 2 5
2 3 4
3 0 1000000000
3 3 100
1 2 3
1 3 4
2 3 5
4 6 1000000000
1 2 244
1 2 325
1 4 927
3 3 248
2 4 834
3 4 285
```

```output1
125
0
15300
840659991
```

