## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc146/tasks/arc146_f

$ (1,2,\dots,N) $ の順列 $ P $ を用意して、次の操作を行います。

> $ N $ 枚のカードがあります。これらのカードには $ 1 $ から $ N $ の番号がついてます。カード $ i $ には $ P_i $ が書かれています。
> 
> 整数 $ X=1 $ があります。はじめ PCT 君は何も持っていません。PCT 君は以下の操作を $ i=1,2,\dots,N $ の順で行います。
> 
> - カード $ i $ を手に入れる。その後、$ X $ が書かれたカードを持っている限り以下の行動を繰り返す。
> - $ X $ の書かれているカードを食べ、$ X $ を $ 1 $ 増やす。
> 
> - 現在持っているカードの枚数が $ M $ 枚以上の場合、持っているカードを全て捨てて操作を終了する。これ以降も操作は行わない。

ここで、以下のように順列 $ P $ のスコアを定義します。

- カードが捨てられて操作が終わった場合、$ P $ のスコアを $ 0 $ とする。
- カードが捨てられずに操作が最後まで行われた場合、$ P $ のスコアを $ \prod_{i=1}^{N-1} $ $ (i $ 回目の操作終了時に PCT 君が持っているカードの枚数 $ ) $ とする。

$ P $ としてあり得るものは $ N! $ 通りありますが、そのすべてに対してスコアの総和を $ 998244353 $ で割ったあまりを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
答えを出力せよ。

## 题目大意
#### 题目描述

有一个长为 $N$ 的排列 $P$ 。

在接下来的 $N$ 天里，为了救她的朋友， $\mathsf{linyue}$ 会参加一个仪式，在第 $i$ 天的行动如下所示：

> 首先，$\mathsf{linyue}$ 会参加这一天的祭祀，然后获得编号为 $P_i$ 的诅咒。
>
> 然后，$\mathsf{linyue}$ 会净化自己身上的诅咒。只要所有编号小于某个诅咒的诅咒都被 $\mathsf{linyue}$ 获得过，那么这个诅咒就会被净化。（特别地，$1$ 号诅咒总是能被净化）
>
> 最后，如果此时 $\mathsf{linyue}$ 身上有不少于 $M$ 种不同的诅咒，那么这个仪式会立刻结束。

这个仪式的贡献是前 $N-1$ 天里每一天结束时 $\mathsf{linyue}$ 身上未净化的诅咒的数量之积。当然，如果仪式中止，贡献就是 $0$。

理论上在第 $N$ 天，$\mathsf{linyue}$ 会获得并净化所有 $N$ 种诅咒，她的朋友也能恢复健康，这样一切都能恢复如初！当然，这需要仪式能有足够的贡献。仪式的贡献只和排列 $P$ 有关，所以 $\mathsf{linyue}$ 希望你能对于所有 $N!$ 种排列 $P$，求仪式的贡献和。

#### 数据范围

$2 ≤ N ≤ 2 × 10^5$
 
$2 ≤ M ≤ N$

#### 样例解释

对于第 $1$ 组样例，$N=3,M=2$。唯一一个可以让仪式有贡献的 $P$ 是 $(3,1,2)$。此时，$\mathsf{linyue}$ 会在第一天获得 $3$ 号诅咒，在第二天获得并净化 $1$ 号诅咒，因此有 $1$ 的贡献。对于其他的排列，如果 $P_3=1$，那么就会导致她在第二天结束时有 $2$ 种诅咒而中止仪式，否则就会导致在前两天里有一天结束时身上未净化诅咒数量为 $0$ 而使得乘积为 $0$。

translated by 隔壁泞2的如心

```input1
3 2
```

```output1
1
```

```input2
3 3
```

```output2
5
```

```input3
146146 146
```

```output3
103537573
```

## 提示
### 制約

- $ 2\ \le\ N\ \le\ 2\ \times\ 10^5 $
- $ 2\ \le\ M\ \le\ N $
- 入力は全て整数である。

### Sample Explanation 1

$ P=(3,1,2) $ の場合、以下のように操作が行われます。 - $ 1 $ 回目の操作 - PCT 君がカード $ 1 $ を手に入れる。 - 現在持っているカードの枚数は $ 1 $ 枚なので、操作を続行する。 - $ 2 $ 回目の操作 - PCT 君がカード $ 2 $ を手に入れる。 - カード $ 2 $ を食べ、$ X $ を $ 2 $ にする。 - 現在持っているカードの枚数は $ 1 $ 枚なので、操作を続行する。 - $ 3 $ 回目の操作 - PCT 君がカード $ 3 $ を手に入れる。 - カード $ 1,3 $ を食べ、$ X $ を $ 4 $ にする。 - 現在持っているカードの枚数は $ 0 $ 枚なので、操作を続行する。 操作が最後まで行われたため、$ (3,1,2) $ のスコアは $ 1\ \times\ 1\ =\ 1 $ です。 $ (3,1,2) $ 以外にスコアが $ 1 $ 以上になる順列は存在しないため、解は $ 1 $ です。

