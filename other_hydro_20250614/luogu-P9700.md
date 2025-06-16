## ��Ŀ����
$\textit{Peg Solitaire}$ is a single-player boardgame on a chessboard with $n$ rows and $m$ columns. Each cell of the chessboard either is empty, or contains a chesspiece. Initially, there are $k$ chesspieces on the chessboard.

During the game, the player can choose a chesspiece, jump it over an adjacent chesspiece into an empty cell, and finally remove the chesspiece which is jumped over. More precisely, let $(i, j)$ be the cell on the $i$-th row and the $j$-th column, the player can perform operations of the following four types.

![](https://cdn.luogu.com.cn/upload/image_hosting/ugauif68.png)

Given the initial state of the chessboard, the player can perform the operations any number of times (including zero times). Calculate the minimum possible number of chesspieces remaining on the chessboard.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 20$) indicating the number of test cases. For each test case:

The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 6$, $1 \le k \le \min(6, n \times m)$) indicating the number of rows and columns of the chessboard and the initial number of chesspieces.

For the following $k$ lines, the $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n$, $1 \le y_i \le m$) indicating that there is a chesspiece in the cell on the $x_i$-th row and the $y_i$-th column at the beginning. Except from these $k$ cells, all other cells are empty at the beginning. The positions of these $k$ cells contain no duplicate.

## �����ʽ
For each test case output one line containing one integer indicating the minimum possible number of chesspieces remaining on the chessboard.


## ��Ŀ����
**����Ŀ������**

``������ʯ``��һ�ֵ������Ρ���Ϸ�� $n$ �� $m$ �е������Ͻ��У������ϵ�ÿһ��Ҫô�ǿո�Ҫô��һö���ӡ�һ��ʼ�������Ϲ��� $k$ ö���ӡ�

����Ϸ�У���ҿ���ѡ��һö���ӣ����������������ӵ��ո��ϣ����Ƴ������������ӡ�������˵���� $(i, j)$ ��ʾλ�ڵ� $i$ �е� $j$ �еĸ��ӣ���ҿ���ִ���������ֲ�����

![](https://cdn.luogu.com.cn/upload/image_hosting/pgosoztu.png)

����һ����ʼ�����̣��󾭹�����β�����������Σ�֮��������������ʣ�༸ö���ӡ�

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$��$1 \le T \le 20$����ʾ������������������ÿ��������ݣ�

��һ�������������� $n$��$m$ �� $k$��$1 \le n, m \le 6$��$1 \le k \le \min(6, n \times m)$����ʾ���̵������������ͳ�ʼ���ӵ�������

���ڽ����� $k$ �У��� $i$ �������������� $x_i$ �� $y_i$��$1 \le x_i \le n$��$1 \le y_i \le m$����ʾһ��ʼ�� $x_i$ �е� $y_i$ �еĸ�������һö���ӡ������� $k$ ������֮�⣬��������һ��ʼ���ǿո��� $k$ �����ӵ�λ�ò����ظ���

**�������ʽ��**

ÿ���������һ��һ����������ʾ��������β�����������Σ�֮��������������ʣ�༸ö���ӡ�

**���������͡�**

��һ���������ݽ������¡�

![](https://cdn.luogu.com.cn/upload/image_hosting/aragowha.png)

���ڵڶ����������ݣ����ڳ�ʼ���̲����ڿո�����޷������κβ�����

���ڵ������������ݣ��������̲�����������޷������κβ�����

```input1
3
3 4 5
2 2
1 2
1 4
3 4
1 1
1 3 3
1 1
1 2
1 3
2 1 1
2 1
```

```output1
2
3
1
```

## ��ʾ
The first sample test case is explained as follows.

![](https://cdn.luogu.com.cn/upload/image_hosting/aragowha.png)

For the second sample test case, as the chessboard does not contain empty cell at the beginning, the player cannot perform any operation.

For the third sample test case, as the chessboard has less than three cells, the player cannot perform any operation.


