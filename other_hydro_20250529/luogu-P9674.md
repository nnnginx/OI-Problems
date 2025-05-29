## ��Ŀ����
Prof. Pang has a multi-set of intervals $S=\{[l_i,r_i]\}$($l_i<r_i$).

Prof. Pang will perform the following operation for $|S|-1$ times:

- Select two intervals $[a,b]$ and $[c,d]$ from $S$, and then choose two integers $x,y$ satisfying $x\in [a,b], y\in [c,d], x<y$. After that, delete $[a,b]$ and $[c,d]$ from $S$, and add $[x,y]$ to $S$.

It's easy to find that $S$ contains exactly one interval after the operations, and Prof. Pang will get the interval as a gift.

Now Prof. Pang wants you to calculate how many different intervals he can get.

## �����ʽ
The first line contains one integer $T~$($1\le T \le 10^4$), the number of test cases.

For each test case, the first line contains one integer $n~$($1\le n\le 10^5$) --- the size of $S$. Each of the following $n$ lines contains two integers $l_i$ and $r_i~$($1\le l_i<r_i\le 10^9$), describing the $i$-th interval in $S$.

It is guaranteed that the sum of $n$ over all test cases is no more than $10^5$.

## �����ʽ
For each test case, output one line containing the answer to Prof. Pang's question.

## ��Ŀ����
������һ��Ԫ��ȫΪ������Ŀ��ؼ� $S=\{[l_i,r_i]\}$($l_i<r_i$)��

��������ִ�����²��� $n-1$ �Σ�
- �� $S$ ��ѡ������������ $[a,b]$ �� $[c,d]$����ѡ���������� $x,y$ ���� $x\in [a,b], y\in [c,d], x<y$��Ȼ��� $S$ ��ɾȥ $[a,b]$ �� $[c,d]$������ $[x,y]$ ��ӽ� $S$��

��Ȼ���� $S$ �����ҽ���һ�����䡣����������֪�������Ի�ö��ٲ�ͬ�����䡣

```input1
4
1
1 1000000000
2
1 1000000000
1 1000000000
4
1 2
3 4
5 6
7 8
4
1 3
2 4
5 8
6 7
```

```output1
1
499999999500000000
26
28
```

