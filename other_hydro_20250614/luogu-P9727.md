## ��Ŀ����
Given an $n \times m$ matrix, you need to fill it with $0$ and $1$, such that:

- There cannot be **four** consecutive horizontal or vertical cells filled with the same number.
- The cells filled with $1$ form a connected area. (Two cells are adjacent if they share an edge. A group of cells is said to be connected if for every pair of cells it is possible to find a path connecting the two cells which lies completely within the group, and which only travels from one cell to an adjacent cell in each step.)

Please construct a matrix satisfying the conditions above and has as many $1$s as possible. Output the maximum number of $1$s, and the matrix.

## �����ʽ
The first line contains an integer $T~(1\leq T\leq 10^3)$ -- the number of test cases.

For each test case, the first line contains two integers $n, m~(2\leq n, m\leq 10^3)$.

### It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10^6$.

## �����ʽ
For each test case, output the maximum number of $1$s in the first line. Then output the matrix in the following $n$ lines. If there are multiple solution, output any.

## ��Ŀ����
**����Ŀ������**

����һ�� $n \times m$ ��������Ҫ�� $0$ �� $1$ �������ʹ����������������

- ������**�ĸ�**������ˮƽ��ֱ��Ԫ��������ͬ�����֡�
- ���� $1$ �ĵ�Ԫ���γ�һ����ͨ���򡣣�������ǹ���һ���ߣ���������Ԫ�������ڵġ��������ÿ�Ե�Ԫ�񣬿����ҵ�һ����ȫλ�ڸ������ڵ�����������Ԫ���·��������ÿһ��ֻ�ܴ�һ����Ԫ���ƶ������ڵĵ�Ԫ����һ�鵥Ԫ�񱻳�Ϊ��ͨ�ġ���

�빹��һ���������������Ҿ��о����ܶ�� $1$ �ľ������ $1$ ����������Լ��þ���

**�������ʽ��**

��һ�а���һ������ $T~(1\leq T\leq 10^3)$����ʾ����������������

����ÿ��������������һ�а����������� $n, m~(2\leq n, m\leq 10^3)$��

��֤���в��������� $n\cdot m$ ���ܺͲ����� $10^6$��

**�������ʽ��**

����ÿ�����������������һ���� $1$ �����������Ȼ���ڽ������� $n$ ���������������ж��ֽ�����������������һ����

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
3
2 2
3 4
3 8

```

```output1
4
11
11
9
1110
1110
1110
18
11101110
10111011
11011011

```

