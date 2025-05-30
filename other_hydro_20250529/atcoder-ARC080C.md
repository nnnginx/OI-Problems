## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc080/tasks/arc080_c

$ N $ を正の偶数とします。

$ (1,\ 2,\ ...,\ N) $ の順列 $ p\ =\ (p_1,\ p_2,\ ...,\ p_N) $ があります。 すぬけ君は、次の手続きによって $ (1,\ 2,\ ...,\ N) $ の順列 $ q $ を作ろうとしています。

まず、空の数列 $ q $ を用意します。 $ p $ が空になるまで、次の操作を繰り返します。

- $ p $ の隣り合う $ 2 $ つの要素を選び、順に $ x $, $ y $ とする。 $ x $, $ y $ を $ p $ から取り除き (このとき、$ p $ は $ 2 $ だけ短くなる)、$ x $, $ y $ をこの順のまま $ q $ の先頭へ追加する。

$ p $ が空になったとき、$ q $ は $ (1,\ 2,\ ...,\ N) $ の順列になっています。

辞書順で最小の $ q $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ p_1 $ $ p_2 $ $ ... $ $ p_N $

## 输出格式
辞書順で最小の $ q $ を空白区切りで出力せよ。

## 题目大意
给定正偶数 $N$。

给定 $N$ 元排列 $p = (p_1, p_2, ..., p_N)$. Snuke 打算根据下述步骤构造一个 $N$ 元排列 $q$。

首先，令 $q$ 为空。接下来，执行下述操作直到 $p$ 为空。

- 选择 $p$ 中两个相邻元素 ,按原顺序设它们是 $x$ 和 $y$. 从 $p$ 中移除 $x$ 和 $y$，将它们按顺序接在 $q$ 的前面。

试求可能的形成的 $q$ 中，字典序最小的排列。

```input1
4
3 2 4 1
```

```output1
3 1 2 4
```

```input2
2
1 2
```

```output2
1 2
```

```input3
8
4 6 3 2 8 5 7 1
```

```output3
3 1 2 7 4 6 8 5
```

## 提示
### 制約

- $ N $ は偶数である。
- $ 2\ <\ =\ N\ <\ =\ 2\ ×\ 10^5 $
- $ p $ は $ (1,\ 2,\ ...,\ N) $ の順列である。

### Sample Explanation 1

次の順に操作を行えばよいです。 $ p $ $ q $ $ (3,\ 2,\ 4,\ 1) $ $ () $ ↓ ↓ $ (3,\ 1) $ $ (2,\ 4) $ ↓ ↓ $ () $ $ (3,\ 1,\ 2,\ 4) $

### Sample Explanation 3

次の順に操作を行えばよいです。 $ p $ $ q $ $ (4,\ 6,\ 3,\ 2,\ 8,\ 5,\ 7,\ 1) $ $ () $ ↓ ↓ $ (4,\ 6,\ 3,\ 2,\ 7,\ 1) $ $ (8,\ 5) $ ↓ ↓ $ (3,\ 2,\ 7,\ 1) $ $ (4,\ 6,\ 8,\ 5) $ ↓ ↓ $ (3,\ 1) $ $ (2,\ 7,\ 4,\ 6,\ 8,\ 5) $ ↓ ↓ $ () $ $ (3,\ 1,\ 2,\ 7,\ 4,\ 6,\ 8,\ 5) $

