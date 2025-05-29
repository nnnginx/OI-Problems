## 题目描述
Chilling capybaras celebrate Capybara Cozy Carnival. Chairman capybara cuts convex cake. Cake contains $n$ colorful corners. Countless colors comprise $k$ choices. Creating $m$ continuous crossing-free corner-to-corner cuts, chairman cuts cake chunks, catering $m + 1$ comrades. Curiously, consecutive cake chunks corners contain contrasting colors. 

Calculate cake corners color combinations, considering cuts conditions.

In other words, you are given a cake in the shape of a regular $n$-sided polygon and $m$ non-intersecting diagonal cuts, which divide it into $m + 1$ slices.

Calculate the number of ways to color each corner of the original cake with one of the $k$ colors, such that no two neighboring corners of the resulting slices have the same color. Two corners are considered neighboring if they are either consecutive in the original cake, or they are the endpoints of the same cut. It is not necessary to use all the colors. As the number of ways might be large, find it modulo $998\,244\,353$.

## 输入格式
Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.

The first line of each test case contains three integers $n$, $m$, and $k$, denoting the number of cake corners, the number of cuts, and the number of available colors ($3 \le n \le 10^9$; $0 \le m \le 2\cdot 10^5$; $2 \le k \le 10^6$).

The $i$-th of the following $m$ lines contains two integers $u_i$ and $v_i$, denoting the corners connected by the $i$-th cut ($1 \le u_i < v_i \le n$). No two cuts may coincide or intersect except at the ends of the cuts. All cuts are straight, going strictly inside the cake.

It is guaranteed that the sum of $m$ over all test cases does not exceed $2\cdot 10^5$.

## 输出格式
For each test case, print the number of ways to color the cake corners such that no two neighboring corners have the same color, modulo $998\,244\,353$. Remember that you don't have to use all the colors.

```input1
4
4 1 3
1 3
5 0 2
9 4 3
1 3
1 6
4 6
6 8
3 0 1001
```

```output1
6
0
54
1754647
```

