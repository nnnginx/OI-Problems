# 描述

给定一个正整数 $k$，有 $k$ 次询问，每次给定三个正整数 $n_i, e_i, d_i$，求两个正整数 $p_i, q_i$， 使$n_i = p_i ×q_i,e_i ×d_i = (p_i −1)(q_i −1)+1$。

# 输入格式

从文件 decode.in 中读入数据。 
第一行一个正整数 $k$，表示有 $k$ 次询问。 
接下来 $k$ 行，第 $i$ 行三个正整数 $n_i, d_i, e_i$。

# 输出格式

输出到文件 decode.out 中。

输出 $k$ 行，每行两个正整数 $p_i, q_i$ 表示答案。 

为使输出统一，你应当保证 $p_i ≤ q_i$。 

如果无解，请输出 ==NO==。

```input1
10
770 77 5
633 1 211
545 1 499
683 3 227
858 3 257
723 37 13
572 26 11
867 17 17
829 3 263
528 4 109
```
```output1
2 385
NO
NO
NO
11 78
3 241
2 286
NO
NO
6 88
```

# 样例 2
见选手目录下的 decode/decode2.in 与 decode/decode2.ans。

# 样例 3
见选手目录下的 decode/decode3.in 与 decode/decode3.ans。

# 样例 4
见选手目录下的 decode/decode4.in 与 decode/decode4.ans。

# 数据范围

以下记 $m = n − e × d + 2$。
保证对于100%的数据，$1 ≤ k ≤ 10^5$，对于任意的$1 ≤ i ≤ k，1 ≤ n_i ≤ 10^{18},1 ≤ e_i ×d_i ≤10^{18}$,$1≤m≤10^9$。
![](./5151/file/tmp1031-1.jpg)

[测试样例 decode.zip](./5151/file/decode.zip)