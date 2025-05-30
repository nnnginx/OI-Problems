考虑一个由 $N$ 个编号为 $1 \ldots N$ 的结点组成的网络。每个结点被指定为发送者（sender）、接收者（receiver）或两者均不是。发送者的数量 $S$ 与接收者的数量相等。

这一网络中结点间的连接关系可以用一系列形式为 $i \to j$ 的有向边表示，代表由结点 $i$ 可以路由到结点 $j$。有趣的是，所有的边满足性质 $i \lt j$，除了 $K$ 条满足 $i \gt j$。网络中没有自环（$i \to i$ 形式的边）。

一个「路由方案」的描述由 $S$ 条从发送者到接收者的有向路径组成，其中没有两条路径有相同的起止点。也就是说，这些路径将不同的发送者连接到不同的接收者。一条从发送者 $s$ 到接收者 $r$ 的路径可以用一个结点序列
$$s=v_0 \to v_1 \to v_2 \to \cdots \to v_e=r$$
表示，其中对于所有 $0 \leqslant i \lt e$，有向边 $v_i \to v_i+1$ 均存在。一个结点可能在同一条路径中出现多于一次。

计算使得每条有向边恰好使用一次的路由方案数量。由于答案可能非常大，输出答案对 $10^9+7$ 取模的结果。输入保证存在至少一种路由方案符合条件。

每个输入包含 $T$ 组需要独立求解的测试用例。输入保证所有测试用例的 $N^2$ 之和不超过 $2 \cdot 10^4$。

> - $2 \leqslant N \leqslant 100$
> - $S \geqslant 1$
> - $0 \leqslant K \leqslant 2$
> - $1 \leqslant T \leqslant 20$

## 输入格式

输入的第一行包含 $T$，为测试用例的数量。

每个测试用例的第一行包含整数 $N$ 和 $K$。注意 $S$ 并不会在输入中明确给出。

每个测试用例的第二行包含一个长为 $N$ 的字符串。如果第 $i$ 个结点是发送者，则字符串的第 $i$ 个字符为 `S`，如果第 $i$ 个结点是接收者则为 `R`，如果第 $i$ 个结点两者均不是则为 `.`。字符串中 `R` 的数量等于 `S` 的数量，且至少有一个 `S`。

每个测试用例的以下 $N$ 行每行包含一个长为 $N$ 的 01 字符串。如果从结点 $i$ 到结点 $j$ 存在一条有向边，则第 $i$ 行的第 $j$ 个字符为 $1$，否则为 $0$。由于不存在自环，矩阵的主对角线仅包含 $0$。除此之外，在主对角线以下恰好有 $K$ 个 $1$。

为提高可读性，相邻的测试用例之间用一个空行隔开。

## 输出格式

对每个测试用例，输出每条边使用恰好一次的路由方案的数量，结果对 $10^9+7$ 取模。输入保证对每个测试用例存在至少一种合法的路由方案。

```input1
2

8 0
SS....RR
00100000
00100000
00011000
00000100
00000100
00000011
00000000
00000000

13 0
SSS.RRRSS.RR.
0001000000000
0001000000000
0001000000000
0000111000000
0000000000000
0000000000000
0000000000000
0000000001000
0000000001000
0000000000110
0000000000000
0000000000000
0000000000000
```
```output1
4
12
```

> 对于第一个测试用例，网络中的边为 $1 \to 3,2 \to 3,3 \to 4,3 \to 5,4 \to 6,5 \to 6,6 \to 7,6 \to 8$。
>

> 有四种可能的路由方案：
>

> - $1 \to 3 \to 4 \to 6 \to 7,2 \to 3 \to 5 \to 6 \to 8$
> - $1 \to 3 \to 5 \to 6 \to 7,2 \to 3 \to 4 \to 6 \to 8$
> - $1 \to 3 \to 4 \to 6 \to 8,2 \to 3 \to 5 \to 6 \to 7$
> - $1 \to 3 \to 5 \to 6 \to 8,2 \to 3 \to 4 \to 6 \to 7$
>

> 对于第二个测试用例，网络中的边为 $1 \to 4,2 \to 4,3 \to 4,4 \to 5,4 \to 6,4 \to 7,8 \to 10,9 \to 10,10 \to 11,11 \to 12$。
>

> 一种可能的路由方案由如下路径组成：
>

> - $1 \to 4 \to 5$
> - $2 \to 4 \to 7$
> - $3 \to 4 \to 6$
> - $8 \to 10 \to 12$
> - $9 \to 10 \to 11$
>

> 总的来说，发送者 $\{1,2,3\}$ 可以路由到接收者 $\{5,6,7\}$ 的某个排列，发送者 $\{8,9\}$ 可以路由到接收者 $\{11,12\}$ 的某个排列，得出答案为 $6 \times 2=12$。

```input2
2

5 1
SS.RR
00101
00100
10010
00000
00000

6 2
S....R
001000
000100
010001
000010
001000
000000
```
```output2
3
1
```

> 对于第一个测试用例，网络中的边为 $1 \to 3,1 \to 5,2 \to 3,3 \to 1,3 \to 4$。
>

> 有三种可能的路由方案：
>

> - $1 \to 3 \to 1 \to 5,2 \to 3 \to 4$
> - $1 \to 3 \to 4,2 \to 3 \to 1 \to 5$
> - $1 \to 5,2 \to 3 \to 1 \to 3 \to 4$
>

> 对于第二个测试用例，网络中的边为 $1 \to 3,2 \to 4,3 \to 2,3 \to 6,4 \to 5,5 \to 3$。
> 
> 只有一种可能的路由方案：$1 \to 3 \to 2 \to 4 \to 5 \to 3 \to 6$。

```input3
5

3 2
RS.
010
101
100

4 2
.R.S
0100
0010
1000
0100

4 2
.SR.
0000
0011
0100
0010

5 2
.SSRR
01000
10101
01010
00000
00000

6 2
SS..RR
001010
000010
000010
000010
100101
000000
```
```output3
2
1
2
6
24
```
> 一些额外的小的测试用例。

## 测试点性质

- 测试点 4-5 满足 $N \leqslant 6$。
- 测试点 6-7 满足 $K=0$。
- 测试点 8-12 满足 $K=1$。
- 测试点 13-24 满足 $K=2$。

## 题目提供者

Benjamin Qi