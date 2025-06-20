# AT_iroha2019_day4_d 揺れる街、増える敵

## 题目描述

在每个 （T） 个城市中，都出现了一个敌人。

出现在第 $(i)$ 个城市的敌人形状像一排方块，原来的方块数是 $(1)$ 或更多，还有 $(L_i)$。 这座城市已经摧毁了超过 $(0)$ 个敌方方格，敌人被摧毁的方格分成了几个部分。 当拥有方格数 $(L)$ 的敌人从最后被 $(i)$ 单元格摧毁时，方格数被分别分成 $(i-1)$ 和 $(L-i)$ 的 $(2)$ 个敌人（但拥有方格数 （0） 的敌人消失了）。

然而，敌人在分裂时变得更加强大。 具体来说，当用 （p_1、p_2、dots、p_n） 将方格数分成 （n） 个部分时，敌人的强度整体变为 （p_1times p_2timesdotstimes p_n）。

目前，在第 （i） 个城市，敌人的实力已经达到 （2^{A_i}） 或更高。 找出出现在 （T） 个城镇中的每个敌人有多少个敌人的原始方块。

## 输入格式

输入以以下形式给出：
```

\(T\)
\(L_1\) \(A_1\)
\(L_2\) \(A_2\)
:
\(L_T\) \(A_T\)
```

## 输出格式

打印 $(T)$ 行，$(i (1 \leqq i \leqq T))$ 行应该是出现在第 $(i)$ 个城市的敌人的答案。

## 输入输出样例 #1

### 输入 #1

```
4
9 3
13 4
11 6
11235813 213455
```

### 输出 #1

```
3
5
0
10702177
```