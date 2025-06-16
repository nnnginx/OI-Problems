## ��Ŀ����
You are given an $n \times m$ grid. Some of the cells are obstacles, the others are empty. Choose a non-negative integer $k$ and color all empty cells with $k+1$ colors $0, 1, 2, \ldots k$. You can not color two cells in the same row or same column with the same **non-zero** color. 

You are given two non-negative integers $c$ and $d$. For a coloring plan, define $z$ as the number of the cells with color $0$. Define the cost of the plan is $ck+dz$.

Find the minimum cost.

## �����ʽ
The first line contains four integers $n$, $m$ ($1\leq n, m\leq 250$), $c$ and $d$ ($0\leq c, d\leq 10 ^ 9$).

The $i$-th line of the next $n$ lines contains a string of $m$ characters. The $j$-th character is `*` if the cell in the $i$-th row and the $j$-th column is an obstacle. The $j$-th character is `.` if the cell in the $i$-th row and the $j$-th column is empty.

## �����ʽ
Output a line with a single number, representing the answer.

## ��Ŀ����
### ��Ŀ����

����һ�� $n\times m$ ������һЩ�������ϰ������������ǿյġ�ѡ��һ���Ǹ����� $k$������ $k + 1$ ����ɫ $0, 1, \ldots, k$ ���ո���Ⱦɫ��������ͬһ�л�ͬһ�е��������ӱ�Ⱦ������ͬ�� **����** ��ɫ��

���������Ǹ����� $c, d$������һ��Ⱦɫ���������� $z$ ��ʾȾ����ɫ $0$ �ĸ�����������÷����Ĵ���Ϊ $ck + dz$��

�����С���ۡ�

$1\leq n, m \leq 250$��$0\leq c, d\leq 10 ^ 9$��

### �����ʽ

��һ���ĸ����� $n, m, c, d$��

������ $n$ �У�ÿ��һ������Ϊ $m$ ���ַ������ַ����ĵ� $j$ ���ַ�Ϊ `*` ��ʾ�� $i$ �е� $j$ �еĸ���Ϊ�ϰ���Ϊ `.` ��ʾΪ�ա�

### �����ʽ

���һ��һ��������ʾ�𰸡�



```input1
3 4 2 1
.***
*..*
**..

```

```output1
4

```

```input2
3 4 1 2
.***
*..*
**..

```

```output2
2
```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem B.

**Author**: csy2005.

