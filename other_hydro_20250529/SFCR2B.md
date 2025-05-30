### 题目描述
小 L 有一张 $n$ 个点的**无向图**。

他认为不互质的一对数是有趣的，于是他规定：在这张图上，$u, v$ 两点之间有边，**当且仅当 $u, v$ 不互质**。

现在，他希望在这张图上进行一次游走。

具体地，他希望求出一个**可以是非简单路径的**路径 $P$。

- 为了游览沿途更丰富的风景，他想要让 $P$ 中**本质不同点数**最多。
- 为了游览时不走太多路，他想要让 $P$ 的**总点数**最短。

请你求出一个符合上述条件的路径 $P$。
### 输入格式
一行，一个整数 $n$。
### 输出格式
第一行，一个整数 $|P|$，表示你求出的路径 $P$ 的总点数；

第二行，$|P|$ 个整数 $P_1, P_2, \cdots, P_{|P|}$，依次表示路径 $P$ 上的每个点。

**若有多种最优方案，你可以输出任意一种。**

**若你的方案的本质不同点数与最优方案相同，但总点数多于最优方案，你也可以获得一些分数，详见「评测说明」。**
### 样例 #1
#### 样例输入 #1
```
4
```
#### 样例输出 #1
```
2
2 4
```
### 样例 #2
#### 样例输入 #2
```
6
```
#### 样例输出 #2
```
4
2 4 6 3
```
### 样例 #3
#### 样例输入 #3
```
9
```
#### 样例输出 #3
```
6
8 4 2 6 3 9
```
### 样例 #4
#### 样例输入 #4
```
15
```
#### 样例输出 #4
```
12
2 8 10 5 15 6 9 3 12 4 14 7
```
### 评测说明
**本题开启 Special Judge。**

设最优解中的路径为 $P_0$，你求出的路径为 $P$。

设 $F(P)$ 表示 $P$ 中本质不同点的个数，则：

- 若 $P$ 不合法或 $F(P) < F(P_0)$，你可以得到当前测试点 $0\%$ 的分数。
- 否则，你可以得到当前测试点 $w(|P|, |P_0|)\%$ 的分数，其中 $w(x, y)$ 的定义如下：

$$
w(x, y) = 
\begin{cases}
0 & (x > \lceil 1.07 y \rceil) \\
20 & (\lceil 1.03 y \rceil < x \leq \lceil 1.07 y \rceil) \\
40 & (\lceil 1.01 y \rceil < x \leq \lceil 1.03 y \rceil) \\
60 & (y < x \leq \lceil 1.01 y \rceil) \\
100 & (x \leq y)
\end{cases}
$$
### 数据范围
对于 $20\%$ 的数据，$2 \leq n \leq 10$；

对于 $40\%$ 的数据，$2 \leq n \leq 100$；

对于 $60\%$ 的数据，$2 \leq n \leq 10^3$；

对于 $80\%$ 的数据，$2 \leq n \leq 10^4$；

对于 $100\%$ 的数据，$2 \leq n \leq 10^5$。