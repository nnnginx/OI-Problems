农夫约翰合牛国（The United Cows of Farmer John，UCFJ）将要选派一个代表队参加国际牛学奥林匹克（International bOvine olympIad，IOI）。

有 $N$ 头奶牛参加了代表队选拔。她们站成一行，奶牛 $i$ 的品种为 $b_i$。

代表队将会由包含至少三头奶牛的连续区间组成——也就是说，对于满足 $1 \leqslant l \lt r \leqslant N$ 且 $r−l \geqslant 2$ 的奶牛 $l \ldots r$。选定区间内的三头奶牛将会被指定为领队。出于法律原因，最边上的两头奶牛必须是领队。此外，为了避免种内冲突，每一名领队都必须与代表队的其他成员（包括领队）品种不同。

请帮助 UCFJ 求出（由于纳税原因）他们可以选派参加 IOI 的代表队的方法数。如果两个代表队拥有不同的成员或不同的领队，则被认为是不同的。

> - $1 \leqslant N \leqslant 2 \cdot 10^5$

## 输入格式

输入的第一行包含 $N$。

第二行包含 $N$ 个整数 $b_1,b_2,\ldots,b_N$，均在范围 $[1,N]$ 之间。

## 输出格式

输出可能的代表队的数量。

注意这个问题涉及到的整数大小可能需要使用 64 位整数型存储（例如，C/C++ 中的 `long long`）。


```input1
7
1 2 3 4 3 2 5
```
```output1
9
```

> 每一代表队对应以下的一组领队：
>

> $$(1,2,3),(1,2,4),(1,3,4),(1,4,7),(2,3,4),(4,5,6),(4,5,7),(4,6,7),(5,6,7).$$

## 测试点性质

- 测试点 1-2 满足 $N \leqslant 50$。

- 测试点 3-4 满足 $N \leqslant 500$。

- 测试点 5-8 满足 $N \leqslant 5000$。

- 测试点 9-20 没有额外限制。


## 题目提供者

Benjamin Qi