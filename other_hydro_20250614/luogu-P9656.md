## ��Ŀ����
BaoBao the Witch is stuck in a maze with $n$ rows and $n$ columns, where the height of the cell in the $i$-th row and the $j$-th column is $h_{i,j}$. To get out of the maze, BaoBao has to find a path which passes through each cell exactly once. Each time she can only move into the neighboring cell sharing a same edge with the current one. But as we know, BaoBao is super lazy, so every time when she climbs up (that is to say, moving from a cell with a smaller height to another with a larger height) her happiness value will decrease. As her helping hand, your task is to find a valid path so that when moving along the path, the number of times BaoBao climbs up will not be more than the number of times she climbs down.

More formally, you need to find a sequence $(x_1, y_1), (x_2, y_2), \cdots, (x_{n^2}, y_{n^2})$ such that:
- For all $1 \le i \le n^2$, $ 1 \le x_i, y_i \le n$;
- For all $1 \le i, j \le n^2, i \neq j$, $ (x_i, y_i) \neq (x_j, y_j)$;
- For all $2 \le i \le n^2$, $|x_i - x_{i-1}| + |y_i - y_{i-1}| = 1$;
- $\sum\limits_{i=2}^{n^2}{[h_{x_{i-1}, y_{i-1}} < h_{x_i, y_i}]} \le \sum\limits_{i=2}^{n^2}{[h_{x_{i-1}, y_{i-1}} > h_{x_i, y_i}]}$, where $[P]$ equals $1$ when $P$ is true, and equals $0$ when it is false.

Additionally, you discover that the heights in all cells are a permutation of $n^2$, so you just need to output the height of each cell in a valid path.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 100$) indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($2 \le n \le 64$) indicating the size of the maze.

For the following $n$ lines, the $i$-th line contains $n$ integers $h_{i, 1}, h_{i, 2}, \cdots, h_{i,n}$ ($1 \le h_{i, j} \le n^2$) where $h_{i,j}$ indicates the height of the cell in the $i$-th row and the $j$-th column. It's guaranteed that all integers in the input make up a permutation of $n^2$.

## �����ʽ
For each test case output one line containing $n^2$ separated by a space indicating the heights of each cell in a valid path. If there are multiple valid answers you can output any of them. It's easy to prove that an answer always exists.

Please, DO NOT output extra spaces at the end of each line, or your answer may be considered incorrect!

## ��Ŀ����
**����Ŀ������**

����Ů�ױ�����һ�� $n$ �� $n$ �е��Թ��У����е� $i$ �е� $j$ �еĵ�Ԫ��߶�Ϊ $h_{i,j}$��Ҫ�߳��Թ������������ҵ�һ��·������·������ÿ����Ԫ��ǡ��һ�Ρ�ÿ����ֻ���ƶ����뵱ǰ��Ԫ����ߵ����ڵ�Ԫ�񡣵���������֪�������ǳ���������ÿ�������������Ӹ߶Ƚϵ͵ĵ�Ԫ���ƶ����߶Ƚϸߵĵ�Ԫ��ʱ�������Ҹ�ֵ����١���Ϊ���İ��֣�����������ҵ�һ����Ч��·����ʹ������·���ƶ�ʱ�����������Ĵ������������½��Ĵ�����

����ʽ��˵������Ҫ�ҵ�һ������ $(x_1, y_1), (x_2, y_2), \cdots, (x_{n^2}, y_{n^2})$��ʹ�ã�
- �������е� $1 \le i \le n^2$��$ 1 \le x_i, y_i \le n$��
- �������е� $1 \le i, j \le n^2, i \neq j$��$ (x_i, y_i) \neq (x_j, y_j)$��
- �������е� $2 \le i \le n^2$��$|x_i - x_{i-1}| + |y_i - y_{i-1}| = 1$��
- $\sum\limits_{i=2}^{n^2}{[h_{x_{i-1}, y_{i-1}} < h_{x_i, y_i}]} \le \sum\limits_{i=2}^{n^2}{[h_{x_{i-1}, y_{i-1}} > h_{x_i, y_i}]}$������ $[P]$ �� $P$ Ϊ��ʱ���� $1$����Ϊ��ʱ���� $0$��

���⣬�㷢�����е�Ԫ��ĸ߶ȶ��� $n^2$ �����У�������ֻ��Ҫ�����Ч·����ÿ����Ԫ��ĸ߶ȡ�

**�������ʽ��**

�ж����������������ĵ�һ�а���һ������ $T$��$1 \le T \le 100$������ʾ��������������������ÿ������������

��һ�а���һ������ $n$��$2 \le n \le 64$������ʾ�Թ��Ĵ�С��

�������� $n$ �У��� $i$ �а��� $n$ ������ $h_{i, 1}, h_{i, 2}, \cdots, h_{i,n}$��$1 \le h_{i, j} \le n^2$�������� $h_{i,j}$ ��ʾ�� $i$ �е� $j$ �е�Ԫ��ĸ߶ȡ���֤�����е������������� $n^2$ �����С�

**�������ʽ��**

����ÿ���������������һ�У����� $n^2$ ���ɿո�ָ�����������ʾ��Ч·����ÿ����Ԫ��ĸ߶ȡ�����ж����Ч�𰸣��������������κ�һ����������֤�������Ǵ��ڡ�

�벻Ҫ��ÿ�е�ĩβ�������Ŀո񣬷�����Ĵ𰸿��ܻᱻ��Ϊ����ȷ��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
1
2
4 3
2 1
```

```output1
4 3 1 2
```

