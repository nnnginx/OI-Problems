## ��Ŀ����
Prof. Pang is given a fixed sequence $a_1, \ldots, a_n$ and $m$ queries.

Each query is specified by two integers $l$ and $r$ satisfying $1\le l\le r\le n$. For each query, you should answer the number of pairs of integers $(i, j)$ such that $l\le i\le j\le r$ and the number of distinct integers in $a_i, \ldots, a_j$ is odd.

## �����ʽ
The first line contains a single integer $n$ ($1\le n\le 5\times 10^5$).

The next line contains $n$ integers $a_1, \ldots, a_n$ ($1\le a_i\le n$ for all $1\le i\le n$) separated by single spaces.

The next line contains a single integer $m$ ($1\le m\le 5\times 10^5$).

Each of the next $m$ lines contains two integers $l$ and $r$ ($1\le l\le r\le n$) separated by a single space denoting a query.

## �����ʽ
For each query, output one line containing the answer to that query.

```input1
5
1 2 3 2 1
5
1 5
2 4
1 3
2 5
4 4
```

```output1
10
3
4
6
1
```

```input2
5
2 3 5 1 5
5
2 3
1 1
1 3
2 5
2 4
```

```output2
2
1
4
6
4
```

```input3
10
2 8 5 1 10 5 9 9 3 5
10
6 8
1 2
3 5
5 7
1 7
3 9
4 9
1 4
3 7
2 5
```

```output3
4
2
4
4
16
16
12
6
9
6
```

