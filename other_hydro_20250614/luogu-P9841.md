## ��Ŀ����
Every traveler knows that they'll be rewarded with a treasure box after solving the puzzles in Inazuma, but few know that these puzzles are designed by Yae Miko, the Guuji of the Grand Narukami Shrine, to test whether the traveler is strong enough to save her friend Raiden Shogun and people of Inazuma.

![](https://cdn.luogu.com.cn/upload/image_hosting/p50zu2m6.png)

After a traveler passes the test Yae will have to reset the puzzles to the initial state. But this time she has some troubles and even doubts that whether some of them are already broken.

Yae's puzzle can be considered as a weighted undirected complete graph $G$ before resetting. We also denote the initial state as another weighted undirected complete graph $H$. Both $G$ and $H$ have exactly $n$ vertices, and these vertices are labeled from $1$ to $n$.

To reset graph $G$ to $H$ Yae can perform the following operation any number of times:
- First select four distinct vertices $a$, $b$, $c$, $d$ and an integer $x$. Note that she can select a different set of $a$, $b$, $c$, $d$ and $x$ each time.
- Let $(i, j)$ be the edge between vertices $i$ and $j$. Increase the weight of $(a, b)$, $(a, c)$ and $(a, d)$ by $x$ and also decrease the weight of $(b, c)$, $(b, d)$ and $(c, d)$ by $x$.

Please help Yae determine whether she can change graph $G$ to graph $H$. If yes you also shall tell her the detailed steps.

## �����ʽ
There is only one test case in each test file.

The first line of the input contains an integer $n$ ($4 \leq n \leq 100$) indicating the number of vertices in graph $G$ and $H$.

For the following $(n - 1)$ lines, the $i$-th line contains $(n - i)$ integers $w_{i, i + 1}, w_{i, i + 2}, \cdots, w_{i, n}$ ($-100 \le w_{i, j} \le 100$) where $w_{i, j}$ indicates the weight of the edge connecting vertices $i$ and $j$ in graph $G$.

For the following $(n - 1)$ lines, the $i$-th line contains $(n - i)$ integers $v_{i, i + 1}, v_{i, i + 2}, \cdots, v_{i, n}$ ($-100 \le v_{i, j} \le 100$) where $v_{i, j}$ indicates the weight of the edge connecting vertices $i$ and $j$ in graph $H$.

## �����ʽ
If Yae cannot change $G$ to $H$, output `-1`.

Otherwise first output an integer $m$ ($0 \le m \le 10^5$) in one line indicating the number of operations Yae needs.

For the following $m$ lines, output five integers $a_i$, $b_i$, $c_i$, $d_i$ and $x_i$ in the $i$-th line separated by a space, indicating that for the $i$-th operation Yae choose vertices $a_i$, $b_i$, $c_i$, $d_i$ and integer $x_i$. Note that $a_i$, $b_i$, $c_i$, $d_i$ must be distinct and $-10^9 \le x_i \le 10^9$.

It can be proved that if graph $G$ can be changed to graph $H$ there exists a solution with no more than $10^5$ operations.

Note that you don't have to minimize $m$. If there are multiple solutions, output any of them.

## ��Ŀ����
����һ�� $n$ ����Ĵ�Ȩ��ȫͼ $G$����������Զ����ͼ������ $10^5$ �����²�����ʹ������һ�Ŵ�Ȩ��ȫͼ $H$��
- ѡȡ�ĸ��� $a,b,c,d$ ��Ȩֵ $x$��ʹ�ñ� $(a,b),(a,c),(a,d)$ ���� $x$���� $(b,c),(b,d),(c,d)$ ��ȥ $x$��

����һ�鷽�����ж��޽⡣  
$4\le n\le 100$����Ȩ�� $-100\sim 100$ ֮�䡣

```input1
4
0 1 1
0 0
1
1 0 0
1 1
0

```

```output1
1
2 1 3 4 1

```

```input2
4
3 3 3
0 0
0
0 0 0
3 3
3

```

```output2
1
1 2 3 4 -3

```

```input3
5
-12 15 -12 1
37 14 7
7 9
-11
12 5 1 13
-1 -4 -7
-5 -9
18

```

```output3
-1

```

