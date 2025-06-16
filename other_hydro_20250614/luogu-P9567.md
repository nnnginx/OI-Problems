## ��Ŀ����
Given a grid with $n$ rows and $n$ columns, there is exactly one black cell in the grid and all other cells are white. Let $(i, j)$ be the cell on the $i$-th row and the $j$-th column, this black cell is located at $(b_i, b_j)$.

You need to cover all white cells with some L-shapes, so that each white cell is covered by exactly one L-shape and the only black cell is not covered by any L-shape. L-shapes must not exceed the boundary of the grid.

More formally, an L-shape in the grid is uniquely determined by four integers $(r, c, h, w)$, where $(r, c)$ determines the turning point of the L-shape, and $h$ and $w$ determine the direction and lengths of the two arms of the L-shape. The four integers must satisfy $1 \le r, c \le n$, $1 \le r + h \le n$, $1 \le c + w \le n$, $h \ne 0$, $w \ne 0$.

- If $h < 0$, then all cells $(i, c)$ satisfying $r + h \le i \le r$ belong to this L-shape; Otherwise if $h > 0$, all cells $(i, c)$ satisfying $r \le i \le r + h$ belong to this L-shape.
- If $w < 0$, then all cells $(r, j)$ satisfying $c + w \le j \le c$ belong to this L-shape; Otherwise if $w > 0$, all cells $(r, j)$ satisfying $c \le j \le c + w$ belong to this L-shape.

The following image illustrates some L-shapes.

![](https://cdn.luogu.com.cn/upload/image_hosting/s4jgji61.png)

## �����ʽ
There is only one test case in each test file.

The first line contains three integers $n$, $b_i$ and $b_j$ ($1 \le n \le 10^3$, $1 \le b_i, b_j \le n$) indicating the size of the grid and the position of the black cell.

## �����ʽ
If a valid answer exists first output `Yes` in the first line, then in the second line output an integer $k$ ($0 \leq k \leq \frac{n^2-1}{3}$) indicating the number of L-shapes to cover white cells. Then output $k$ lines where the $i$-th line contains four integers $r_i$, $c_i$, $h_i$, $w_i$ separated by a space indicating that the $i$-th L-shape is uniquely determined by $(r_i, c_i, h_i, w_i)$. If there are multiple valid answers you can print any of them.

If there is no valid answer, just output `No` in one line.

## ��Ŀ����
**����Ŀ������**

����һ�� $n$ �� $n$ �е����������а���ǡ��һ����ɫ�������෽���Ϊ��ɫ���� $(i, j)$ ��ʾλ�ڵ� $i$ �е� $j$ �еĸ��ӣ������ɫ����λ�� $(b_i, b_j)$��

����Ҫ������ L �θ������а�ɫ���ӣ�ʹ��ÿ����ɫ���Ӷ�ǡ�ñ�һ�� L �������ǣ�ͬʱΨһ�ĺ�ɫ�����ܱ��κ� L �θ��ǡ�L �β��ܳ�������ı߽硣

����ʽ�أ������е�һ�� L �����ĸ����� $(r, c, h, w)$ Ψһȷ�������� $(r, c)$ ȷ���� L �ε�ת�۵㣬$h$ �� $w$ ȷ���� L �����۵ķ���ͳ��ȡ��ĸ��������� $1 \le r, c \le n$��$1 \le r + h \le n$��$1 \le c + w \le n$��$h \ne 0$��$w \ne 0$��

- �� $h < 0$������������ $r + h \le i \le r$ �ĸ��� $(i, c)$ �����ڸ� L �Σ������� $h > 0$������������ $r \le i \le r + h$ �ĸ��� $(i, c)$ �����ڸ� L �Ρ�
- �� $w < 0$������������ $c + w \le j \le c$ �ĸ��� $(r, j)$ �����ڸ� L �Σ������� $w > 0$������������ $c \le j \le c + w$ �ĸ��� $(r, j)$ �����ڸ� L �Ρ�

��ͼչʾ�˼��� L �Ρ�

![](https://cdn.luogu.com.cn/upload/image_hosting/s4jgji61.png)

**�������ʽ��**

ÿ�������ļ�����һ��������ݡ�

��һ�������������� $n$��$b_i$��$b_j$��$1 \le n \le 10^3$��$1 \le b_i, b_j \le n$����ʾ����Ĵ�С�Լ���ɫ���ӵ�λ�á�

**�������ʽ��**

������ڷ���Ҫ��ĸ��Ƿ������������һ�� `Yes`���������ڵڶ������һ������ $k$��$0 \leq k \leq \frac{n^2-1}{3}$����ʾ���ǰ�ɫ���ӵ� L ����������������� $k$ �У��� $i$ ������ĸ��ɵ����ո�ָ������� $r_i$��$c_i$��$h_i$ �� $w_i$����ʾ�� $i$ �� L ���� $(r_i, c_i, h_i, w_i)$ Ψһȷ��������ж��ֺϷ��𰸣��������������һ�֡�

��������ڷ���Ҫ��ĸ��Ƿ���������Ҫ���һ�� `No`��

**���������͡�**

��һ����������չʾ���¡�

![](https://cdn.luogu.com.cn/upload/image_hosting/nbrr3gun.png)

```input1
5 3 4

```

```output1
Yes
6
5 1 -1 3
1 2 1 3
3 1 -2 1
4 3 -1 -1
4 5 1 -1
2 5 1 -2

```

```input2
1 1 1

```

```output2
Yes
0

```

## ��ʾ
We illustrate the first sample test case as follows.

![](https://cdn.luogu.com.cn/upload/image_hosting/nbrr3gun.png)

