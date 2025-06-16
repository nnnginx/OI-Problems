## ��Ŀ����
There is a sequence of length $n$. At the beginning, all elements in the sequence equal to $0$. There are also $m$ operations, where the $i$-th operation will change the value of the $l_i$-th element in the sequence to $x_i$, and also change the value of the $r_i$-th element in the sequence to $y_i$. Each operation must be performed exactly once.

Find the optimal order to perform the operations, so that after all operations, the sum of all elements in the sequence is maximized.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($2 \leq n, m \leq 5 \times 10^5$) indicating the length of the sequence and the number of operations.

For the following $m$ lines, the $i$-th line contains four integers $l_i$, $x_i$, $r_i$ and $y_i$ ($1 \leq l_i<r_i \leq n$, $1 \leq x_i,y_i \leq 2$) indicating the $i$-th operation.

It's guaranteed that neither the sum of $n$ nor the sum of $m$ of all test cases will exceed $5 \times 10^5$.

## �����ʽ
For each test case, first output one line containing one integer, indicating the maximum sum of all elements in the sequence after all operations. Then output another line containing $m$ integers $a_1, a_2, \cdots, a_m$ separated by a space, indicating the optimal order to perform the operations, where $a_i$ is the index of the $i$-th operation to be performed. Each integer from $1$ to $m$ (both inclusive) must appear exactly once. If there are multiple valid answers, you can output any of them.

## ��Ŀ����
**����Ŀ������**

��һ������Ϊ $n$ �����У�һ��ʼ�����е�����Ԫ�ؾ�Ϊ $0$�����⻹�� $m$ �����������е� $i$ �������Ὣ�����е� $l_i$ ��Ԫ�ص�ֵ��Ϊ $x_i$���Լ��������е� $r_i$ ��Ԫ�ص�ֵ��Ϊ $y_i$��ÿ����������ǡ��ִ��һ�Ρ�

��ִ�в���������˳��ʹ�����в���ִ����ɺ�����������Ԫ��֮�����

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ�������������� $n$ �� $m$��$2 \leq n, m \leq 5 \times 10^5$����ʾ���еĳ��ȺͲ����ĸ�����

���ڽ����� $m$ �У��� $i$ �������ĸ����� $l_i$��$x_i$��$r_i$ �� $y_i$��$1 \leq l_i<r_i \leq n$��$1 \leq x_i,y_i \leq 2$����ʾ�� $i$ ��������

��֤�������� $n$ ֮���� $m$ ֮�;������� $5 \times 10^5$��

**�������ʽ��**

ÿ�������������һ��һ����������ʾִ�в���������Ԫ�ص����͡����������һ�� $m$ ���ɵ����ո�ָ������� $a_1, a_2, \cdots, a_m$ ��ʾִ�в���������˳������ $a_i$ ��ʾ�� $i$ ��ִ�еĲ����ı�š��� $1$ �� $m$ ��ÿ�������������ˣ�����ǡ�ó���һ�Ρ����ж��ֺϷ��𰸣��������������һ�֡�

**���������͡�**

���ڵ�һ���������ݣ��� $4, 1, 3, 2$ ��˳��ִ�в��������б�Ϊ $\{2, 2, 2, 1\}$��Ԫ��֮��Ϊ $7$��

���ڵڶ����������ݣ��� $2, 1$ ��˳��ִ�в��������б�Ϊ $\{2, 0, 2, 1\}$��Ԫ��֮��Ϊ $5$��

```input1
2
4 4
1 1 2 2
3 2 4 1
1 2 3 2
2 1 4 1
4 2
3 2 4 1
1 2 3 1
```

```output1
7
4 1 3 2
5
2 1
```

## ��ʾ
For the first sample test case, after performing operations $4, 1, 3, 2$ in order, the sequence becomes $\{2, 2, 2, 1\}$. The sum of all elements is $7$.

For the second sample test case, after performing operations $2, 1$ in order, the sequence becomes $\{2, 0, 2, 1\}$. The sum of all elements is $5$.

