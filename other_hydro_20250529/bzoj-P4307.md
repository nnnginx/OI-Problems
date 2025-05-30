## 题目描述

Maishroom 在全国各地开设了 OI 辅导班，比如四川班等等。

Maishroom 的辅导班有两种讲师，也就是助教（主要是机房里其他小伙伴）和教师（主要是 Maishroom 自己）。当一个助教去打 vp 的时候，显然他就不能授课了，不过没有关系，因为只是助教。

当一个教师 A（例如 Maishroom）去打（看）vp（片）的时候，他需要找另一个讲师 B 来代替自己的授课。如果 B 也是教师，他也需要另一个讲师 C 来代替自己，依次类推。

现在我们需要知道：

- 有多少个讲师不能去打 vp。

- 有多少对讲师 $(A,B)$，单独地，每个人都可以去打 vp，然而不能一起打（开）vp（黑）。

## 输入格式

第一行两个整数 $n,k$，分别表示辅导班里的讲师数与教师数。

约定：编号 $1$ 到 $k$ 的为教师，编号 $k+1$ 到 $n$ 的为助教。

以下 $k$ 行，表示各个教师可以被哪些讲师替代。

第 $i+1$ 行，第一个整数 $d_i$，代表可代替教师 $i$ 的讲师数，之后 $d_i$ 个整数为其编号。

## 输出格式

一行，两个整数。分别代表两问的答案。

```input1
7 5
2 6 7
1 7
2 2 7
1 5
1 4
```

```output1
2 3
```

## 样例解释

教师 $4, 5$ 不能去打 vp。因为剩下一个人不能做两个人的事。

当教师 $2, 3$ 开黑的时候，讲师 $7$ 不可能同时顶替他们两个人。

事实上，$(2, 3), (2, 7), (3, 7)$ 都满足，可以单独 vp，不能一起开黑。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq k\leq n\leq 5\times 10^3$，$1\leq m\leq 2\times 10^4$。

