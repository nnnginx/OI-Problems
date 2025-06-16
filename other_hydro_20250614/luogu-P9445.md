## ��Ŀ����
The International Center for the Preservation of Ceramics (ICPC) is searching for motifs in some ancient mosaics. According to the ICPC's definition, a $\textit{mosaic}$ is a rectangular grid where each grid square contains a colored tile. A $\textit{motif}$ is similar to a mosaic but some of the grid squares can be empty. Figure G.1 shows an example motif and mosaic.

The rows of an $r_q \times c_q$ mosaic are numbered $1$ to $r_q$ from top to bottom, and the columns are numbered $1$ to $c_q$ from left to right.

A contiguous rectangular subgrid of the mosaic matches the motif if every tile of the motif matches the color of the corresponding tile of the subgrid. Formally, an $r_p \times c_p$ motif appears in an $r_q \times c_q$ mosaic at position ($r$, $c$) if for all $1 \leq i \leq r_p$, $1 \leq j \leq c_p$, the tile ($r+i-1$, $c+j-1$) exists in the mosaic and either the square ($i$, $j$) in the motif is empty or the tile at ($i$, $j$) in the motif has the same color as the tile at ($r+i-1$, $c+j-1$) in the mosaic.

Given the full motif and mosaic, find all occurrences of the motif in the mosaic.

![](https://cdn.luogu.com.cn/upload/image_hosting/0n7urywk.png)

Figure G.1: Motif (left) and mosaic (right) of Sample Input 1.

## �����ʽ
The first line of input contains two integers $r_p$ and $c_p$, where $r_p$ and $c_p$ ($1 \leq r_p, c_p \leq 1000$) are the number of rows and columns in the motif. Then $r_p$ lines follow, each with $c_p$ integers in the range $[0, 100]$, denoting the color of the motif at that position. A value of $0$ denotes an empty square.

The next line of input contains two integers $r_q$ and $c_q$ where $r_q$ and $c_q$ ($1 \leq r_q, c_q \leq 1000$) are the number of rows and columns in the mosaic. Then $r_q$ lines follow, each with $c_q$ integers in the range $[1, 100]$, denoting the color of the mosaic at that position.

## �����ʽ
On the first line, output $k$, the total number of matches. Then output $k$ lines, each of the form $r c$ where $r$ is the row and $c$ is the column of the top left tile of the match. Sort matches by increasing $r$, breaking ties by increasing $c$.

## ��Ŀ����
#### ��Ҫ����
������������, ���еڶ�����������Ԫ�ط� $0$.

�����һ�������ڵڶ��������е����� $(l, r)$ �������֡�, ���ҽ�������һ�ַ�ʽ�����޸ĵ�һ����������Ϊ $0$ ��Ԫ�غ�, ��һ����������Ͻ��ڵڶ�������Ķ�Ӧλ������Ϊ $(l, r)$ ʱ������ڶ��������һ������ȫ�غ�.

���һ�������ڵڶ������������С����֡���λ�ú��ܡ����֡�������

#### �����ʽ
��һ��, �������� $r_p, c_p$, ��ʾ��һ�����������������.

������ $r_p$ ��, ÿ�� $c_p$ ������, ������һ������.

������һ��, �������� $r_q, c_q$, ��ʾ�ڶ������������������.

������ $r_q$ �У�ÿ�� $c_q$ ������, �����ڶ�������.

#### �����ʽ
��һ��, һ������ $k$, ��ʾ�����֡����ܴ���.

������ $k$ ��, ÿ���������� $x, y$, ��ʾÿһ�Ρ����֡�������. ����ж��, ���� $x$ Ϊ��һ�ؼ���, $y$ Ϊ�ڶ��ؼ�����������������

```input1
2 2
1 0
0 1
3 4
1 2 1 2
2 1 1 1
2 2 1 3

```

```output1
3
1 1
1 3
2 2

```

