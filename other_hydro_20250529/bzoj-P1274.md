给定 $3 \times N$ 个正整数

$A_1,A_2 \dots A_n$

$B_1,B_2 \dots B_n$

$C_1,C_2 \dots C_n$

另给定 $M$ 对正整数 $S_i,T_i$ 对于每一对 $S_i,T_i$，求下列方程组的一组非负实数解

$A_1X_1+A_2X_2+...+A_nX_n=S_i$

$B_1X_1+B_2X_2+...+B_nX_n=T_i$

使得 $C_1X_1+C_2X_2+...+C_nX_n$ 最大


## 输入格式

第一行两个整数代表 $N,M$，

接下来 $N$ 行每行三个正整数 $A_i,B_i,C_i$。

$1\le A_i,B_i,C_i,S_i,T_i \le 10^6$

## 输出格式

输出为 $M$ 行，第 $i$ 行代表 $S_i,T_i$。

如果方程无解输出`IMPOSSIBLE`

否则输出一个实数保留五位小数，代表对应的最大值。

```input1
1 2
100 100 10
3 3
99 100
```

```output1
0.30000
IMPOSSIBLE
```



## 数据范围

$50\%$ 的数据满足 $1 \leq N,M \leq 1000$；

$100\%$ 的数据满足 $1 \leq N \leq 10^5,~1 \leq M \leq 10^4$；

$100\%$ 的数据满足 $1 \leq A_i,B_i,C_i,S_i,T_i \leq 10^6$。

