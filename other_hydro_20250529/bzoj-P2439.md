小 W 很喜欢序列，尤其喜欢 $\texttt W$ 形的和 $\texttt M$ 形的序列。

定义 $\texttt M$ 形的序列为一个长度为 $m$ 的序列 $a$，当且仅当存在 $1<x<y<z<m$，使得 $a_1<a_2<\cdots<a_{x-1}<a_x>a_{x+1}>\cdots>a_{y-1}>a_y<a_{y+1}<\cdots<a_{z-1}<a_z>a_{a_z+1}>\cdots>a_{m-1}>a_m$。

例如，$a=\{1,3,2,4,2\}$ 和 $a=\{1,4,5,1,4,1\}$ 就是 $\texttt M$ 形的，而 $a=\{3,3,3,3,3\}$，$a=\{5,5,4,6,3,8\}$ 和 $a=\{1,1,4,5,1,4\}$ 就不是 $\texttt M$ 形的。

一天他看到了一个长度为N 的整数序列{Ai}，他想通过一些修改把序列变成“M”形的。但这时小 X 过来了，说这个序列是他的，小 W 如果想要修改就要支付一定的费用。每支付一单位的费用，小 W 都可以进行这样的操作：将一段连续的数同时加上 1，即选定i, j 满足1 ≤ i ≤ j ≤ N 并令Ai, Ai+1, ..., Aj均加上1。小 W 想用最小的费用将序列变成“M”形的。但是有个条件：如果他修改成的目标是序列{Bi}满足B1 < ... < Bx > ... > By < ... < Bz > ... > BN，那么必须有Ay= By。现在，他希望你来帮他计算最小费用。