## 题目描述
Paimon just puts $(n+1)$ distinct points on the plane, one of which is a special point $O=(0,0)$, and denote the group of remaining points as $\mathbb{S}$.

We call a point set $\mathbb{U}$ $\textit{strict convex set}$, if and only if $|\mathbb{U}| \ge 3$ and all the points from $\mathbb{U}$ lie exactly on the convex hull built from $\mathbb{U}$, with no three points lying on the same line.

You should divide $\mathbb{S}$ into two sets $\mathbb{A}$ and $\mathbb{B}$ so that:
- $\mathbb{A} \cap \mathbb{B}=\emptyset$.
- $\mathbb{A} \cup \mathbb{B}=\mathbb{S}$.
- $|\mathbb{A}| \ge 2, |\mathbb{B}| \ge 2$.
- The point set $\mathbb{A} \cup \{O\}$ is a $\textit{strict convex set}$, and denote its convex hull as $C_{\mathbb{A} \cup \{O\}}$.
- The point set $\mathbb{B} \cup \{O\}$ is a $\textit{strict convex set}$, and denote its convex hull as $C_{\mathbb{B} \cup \{O\}}$.
- The outlines(edges) of $C_{\mathbb{A} \cup \{O\}}$ and $C_{\mathbb{B} \cup \{O\}}$ only intersect at point $O$. That is, only one point $O$ satisfies that it lies both on the outlines of $C_{\mathbb{A} \cup \{O\}}$ and $C_{\mathbb{B} \cup \{O\}}$.

Please help Paimon to maximize the sum of the perimeters of these two convex hulls. That is, find a valid division $\mathbb{A}$ and $\mathbb{B}$ which maximizes $(L(C_{\mathbb{A} \cup \{O\}}) + L(C_{\mathbb{B} \cup \{O\}}))$, where $L(\text{polygon})$ means the perimeter of that polygon.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains one integer $n$ ($4 \le n \le 5 \times 10^5$) indicating the number of points in $\mathbb{S}$.

For the following $n$ lines, the $i$-th line contains two integers $x_i$ and $y_i$ ($-10^9 \le x_i, y_i \le 10^9$, $(x_i, y_i) \ne (0, 0)$) indicating the location of the $i$-th point in $\mathbb{S}$.

It's guaranteed that the points given in the same test case are pairwise different. However, there may be three points lying on the same line.

It's also guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.

## 输出格式
For each test case output one line containing a number indicating the maximum total perimeter. If there does not exist a valid division output `0` instead.

Your answer will be accepted if the relative or absolute error is less than $10^{-6}$.

## 题目大意
## 题目描述

派蒙在平面上放置了$n+1$个互异的点，其中有一特殊点$O=(0,0)$，并记其余点为$\mathbb{S}$。

我们称一个点集 $\mathbb{U}$ 为$\textit{strict convex set}$，当且仅当点集中点的个数大于等于3（$|\mathbb{U}| \ge 3$）且$\mathbb{U}$中的所有点位于$\mathbb{U}$构成的凸包上，且任意三点不共线。


你需要将$\mathbb{S}$划分为两个集合 $\mathbb{A}$ 和$\mathbb{B}$，使其满足
- $\mathbb{A} \cap \mathbb{B}=\emptyset$.
- $\mathbb{A} \cup \mathbb{B}=\mathbb{S}$.
- $|\mathbb{A}| \ge 2, |\mathbb{B}| \ge 2$.

- 点集 $\mathbb{A} \cup \{O\}$ 是 $\textit{strict convex set}$，并记它的凸包为$C_{\mathbb{A} \cup \{O\}}$。
- 点集 $\mathbb{B} \cup \{O\}$是 $\textit{strict convex set}$，并记它的凸包为 $C_{\mathbb{B} \cup \{O\}}$。
- $C_{\mathbb{A} \cup \{O\}}$和 $C_{\mathbb{B} \cup \{O\}}$ 的轮廓 仅在 $O$相交。 这也就是说，仅有点$O$既在$C_{\mathbb{A} \cup \{O\}}$的轮廓上，又在$C_{\mathbb{B} \cup \{O\}}$的轮廓上。
  
请协助派蒙计算出这两个凸包周长之和的最大值。
这也就是说，找到一个合法的划分方案$\mathbb{A}$ 和 $\mathbb{B}$，使得 $(L(C_{\mathbb{A} \cup \{O\}}) + L(C_{\mathbb{B} \cup \{O\}}))$最大，其中$L(\text{polygon})$代表多边形的周长。 

## 输入格式

多组测试数据，第一行给出数据组数 $T$。

第一行给出一个整数 $n$ ($4 \le n \le 5 \times 10^5$) ，表示 $\mathbb{S}$ 中点的个数。

接下来$n$行，第$i$行 包含两个整数 $x_i$ 和 $y_i$ ($-10^9 \le x_i, y_i \le 10^9$, $(x_i, y_i) \ne (0, 0)$) 表示 $\mathbb{S}$ 中第 $i$个点的坐标。

保证同一组测试数据中的点互异，但可能存在三点共线。

保证 所有测试数据中$n$之和不超过 $10^6$.

## 输出格式

每组测试数据单起一行输出一个整数，表示两个凸包的周长之和的最大值。如不存在合法的划分方案，输出`0`。
与标准答案的相对或绝对误差小于 $10^{-6}$的答案会被视作正确答案。

```input1
3
4
0 3
3 0
2 3
3 2
5
4 0
5 -5
-4 -2
1 -2
-5 -2
4
0 1
1 0
0 2
1 1

```

```output1
17.2111025509
36.6326947621
0.0000000000

```

## 提示
A valid division (left) and an invalid division (right) of the first sample test case are shown below.

![](https://cdn.luogu.com.cn/upload/image_hosting/v17tmtdh.png)

