## ��Ŀ����
Consider a grid pattern with $n$ rows and $m$ columns. There are $(n+1)\times(m+1)$ grid points in total which is the intersections of $n+1$ horizontal lines and $m+1$ vertical lines. We number the horizontal lines from $0$ to $n$ from top to bottom. We number the vertical lines from $0$ to $m$ from left to right. The intersection of horizontal line $i$ and vertical line $j$ is named $(i, j)$ ($0\le i\le n, 0\le j\le m$).

There are some constraints when you travel in the grid world. When you are located at point $(x,y)$, you can choose a destination $(x',y')$ and walk to it along the line segment between $(x, y)$ and $(x', y')$. We call this operation a $\textit{walk}$. A walk is forbidden if there exists another grid point different from $(x, y)$ and $(x', y')$ lying on the line segment between them. You can walk as many times as you want but the directions of two consecutive walks cannot be the same. (Specifically, if you walk from $(x_0, y_0)$ to $(x_1, y_1)$ and then walk from $(x_1, y_1)$ to $(x_2, y_2)$, you must make sure that $(x_0-x_1)(y_1-y_2)\neq (x_1-x_2)(y_0-y_1)$.) The length of a walk from $(x, y)$ to $(x', y')$ is defined as the Euclidean distance between the two endpoints, $\sqrt{(x-x')^2+(y'-y)^2}$.

Starting from $(0,0)$, you are planning to arrive at $(n,m)$ by several walks. Because of the annoying rules, you may need some turning points to achieve your goal. Please find the minimum total length of your walks.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n,m$ ($1\le n,m \le 10^6$) indicating the size of the grid graph.

It is guaranteed that the sum of the values of $\max(n,m)$ over all test cases does not exceed $10^6$.

## �����ʽ
For each test case, output the minimum total length of walks. Your answer will be considered correct if its absolute or relative error does not exceed $10 ^{-9}$.

## ��Ŀ����
### ��Ŀ����

���Ǿ��� $n$ �к� $m$ �е�����ģʽ���ܹ���$��n+1��\times��m+1��$����㣬��$n+1$ˮƽ�ߺ�$m+1$��ֱ�ߵĽ��㡣���ǽ�ˮƽ�ߴ��ϵ��´� $0$ �� $n$ ��š����ǽ���ֱ�ߴ����ұ�Ŵ� $0$ �� $m$��ˮƽ�� $i$ �ʹ�ֱ�� $j$ �Ľ�������Ϊ $(i,j)$($0 \le i \le n�� 0 \le j \le m$)��

��������������������ʱ������һЩ���ơ�����λ�ڵ� $(x,y)$ ʱ��������ѡ��һ��Ŀ�ĵ� $(x',y')$ ������ $(x,y)$ �� $(x',y')$ ֮����߶β��е���Ŀ�ĵء����ǽ��˲�����Ϊ $\textit{walk}$���������֮����߶��ϴ�����һ����ͬ�� $(x,y)$ �� $(x', y')$ ������㣬���ֹ���ߡ������������������ߺܶ�Σ����������β��еķ�������ͬ����������˵������� $(x_0,y_0)$ �� $(x_1, y_1)$��Ȼ��� $(x_1, y_1)$ �� $��x_2�� y_2��$�������ȷ�� $(x_0-x_1)(y_1-y_2) \neq (x_1-x_2)(y_0-y_1)$���� $(x,y)$ �� $(x',y')$ �Ĳ��г��ȶ���Ϊ�����˵�֮���ŷ����þ��� $\sqrt{(x-x')^2+(y'-y)^2}$��

�� $(0,0)$ ��ʼ�����ƻ�ͨ�����β��е��� $(n��m)$�����ڷ��˵Ĺ�����������ҪһЩת�۵���ʵ������Ŀ�ꡣ���ҵ������е���С�ܳ��ȡ�

### �����ʽ

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������
��һ�а����������� $n,m$ ��$1 \le n,m \le 10^6$������ʾ����ͼ�Ĵ�С��

��֤���в��������� $\max(n,m)$ ��ֵ֮�Ͳ����� $10^6$��

```input1
2
2 2
2 3
```

```output1
3.236067977499790
3.605551275463989
```

