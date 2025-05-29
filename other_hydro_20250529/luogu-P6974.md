## ��Ŀ����
Garrison and Anderson are working in a company named ��Adjustment Office��. In competing companies workers change the reality, in this company they try to predict the future.

They are given a big square board $n\times n$. Initially in each cell $(x, y)$ of this board the value of $x + y$ is written $(1\leq x, y\leq n$). They know that in the future there will be two types of queries on the board:
- ��R $r$�� �� sum up all values in row $r$, print the result and set all values in row $r$ to zero;
- ��C $c$�� �� sum up all values in column $c$, print the result and set all values in column $c$ to zero.

They have predicted what queries and results there will be. They need to ensure that they have correctly predicted the results. Help them by computing the results of the queries.


## �����ʽ
The first line of the input contains two integers $n$ and $q$ $(1\leq n\leq10^6$, $1\leq q\leq10^5$) �� the size of the square and the number of queries.

Each of the next $q$ lines contains the description of the query. Each query is either ��R $r$�� $(1\leq r\leq n$) or ��C $c$�� $(1\leq c\leq n$).

## �����ʽ
The output file shall contain $q$ lines. The $i$ - th line shall contain one integer �� the result of the $i$ - th query. 

## ��Ŀ����
��һ����СΪ $n\times n$ �ľ���ÿ��λ�õ�ֵΪ��λ�õ�����+������

�������� $q$ �β�����

- $R\ m$������� $m$ �е��ܺͲ�������ȥ��
- $C\ m$������� $m$ �е��ܺͲ�������ȥ��

$1\leqslant n\leqslant 10^6$��$1\leqslant q\leqslant 10^5$��$1\leqslant m\leqslant n$��

Translated by Eason_AC  
2020.11.19

```input1
3 7
R 2
C 3
R 2
R 1
C 2
C 1
R 3

```

```output1
12
10
0
5
5
4
0

```

## ��ʾ
Time limit: 1 s, Memory limit: 256 MB. 



