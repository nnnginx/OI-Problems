## 题目描述
在 $n$ 行 $m$ 列的方格矩阵中，每个方格都包含一个数字。小明可以从任意方格出发开始移动。每次移动可以移到与当前方格有一条边相邻的方格（即向上、下、左或右方向移动 $1$ 格，且不能移出边界）。除此之外，你移动到的方格中的数字必须比当前方格中的数字更大。

请你帮助小明编程规划移动路径，使路径上经过的所有数字之和最大。

## 输入格式
一行三个正整数 $n,m,s$。

本题方格 $a$ 中的数据根据输入的初始数字 $s$ 按照如下算法生成：

$$
\begin{aligned}
&\text{for } i=1\text{ to } n\\
&\quad\text{for } j=1\text{ to } m\\
&\qquad s\gets(s\times345) \bmod 19997\\
&\qquad a_{i,j}\gets (s\bmod 10)+1\\
&\quad \text{end for}\\
&\text{end for}
\end{aligned}
$$

## 输出格式
所有合法路径中的最大数字和。

```input1
4 5 97
```

```output1
24
```

```input2
40 50 1
```

```output2
47
```

## 提示
### 样例 $\textbf 1$ 解释
样例数据 1 对应的矩阵如下。图中路径数字之和 $4+5+7+8=24$。
$$
\begin{array}{|c|c|c|c|c|}\hline 
9 & 7 & 10 & 10 & 8\\\hline
2 & 9 & 2 & 5 &3\\\hline
2 & 5 & \red5 & \red7 & 7\\\hline
5 & 8 & \red4 & \red8 & 5\\\hline
\end{array}
$$
### 数据范围
$1\le n,m\le 100,1\le s\le 19997$。
> 本题原始满分为 $20\text{pts}$。

