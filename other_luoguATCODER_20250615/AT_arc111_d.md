# AT_arc111_d [ARC111D] Orientation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc111/tasks/arc111_d

$ N $ 頂点 $ M $ 辺の単純な無向グラフが与えられます。頂点には $ 1,\ \cdots,\ N $ の番号がついています。$ i $ 番目の辺は頂点 $ a_i $, $ b_i $ を繋いでいます。 また、正整数列 $ c_1,\ c_2,\ \cdots,\ c_N $ も与えられます。

このグラフを、次の条件を満たすように有向グラフに変換してください。つまり、各 $ i $ について無向辺 $ (a_i,\ b_i) $ を削除し、有向辺 $ a_i\ \to\ b_i $、$ b_i\ \to\ a_i $ のどちらか $ 1 $ つを張ってください。

- 全ての $ i\ =\ 1,\ 2,\ \cdots,\ N $ について、頂点 $ i $ から(有向辺を好きな回数使うことで)到達可能な頂点数がちょうど $ c_i $ 個。なお、頂点 $ i $ 自身も $ 1 $ 個と数える。

なお、この問題では、**解が存在する**ような入力のみが与えられます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_1 $ $ b_1 $ $ : $ $ a_M $ $ b_M $ $ c_1 $ $ c_2 $ $ ... $ $ c_N $

## 输出格式

$ M $ 行出力せよ。

$ i $ 行目には、$ i $ 番目の辺について $ a_i\ \to\ b_i $ に辺を張りたい場合 `->`、$ a_i\ \gets\ b_i $ に辺を張りたい場合 `<-` を出力せよ。

解が複数存在する場合、どれを出力しても構わない。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 2
2 3
3 1
3 3 3
```

### 输出 #1

```
->
->
->
```

## 输入输出样例 #2

### 输入 #2

```
3 2
1 2
2 3
1 2 3
```

### 输出 #2

```
<-
<-
```

## 输入输出样例 #3

### 输入 #3

```
6 3
1 2
4 3
5 6
1 2 1 2 2 1
```

### 输出 #3

```
<-
->
->
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 0\ \leq\ M\ \leq\ \frac{N(N\ -\ 1)}{2} $
- $ 1\ \leq\ a_i,\ b_i\ \leq\ N $
- 与えられるグラフに自己ループや多重辺は存在しない
- $ 1\ \leq\ c_i\ \leq\ N $
- **必ず題意を満たす解が存在する**

### Sample Explanation 1

長さ $ 3 $ のサイクルでは、どの頂点からも全ての頂点に到達できます。

### Sample Explanation 3

グラフは非連結のこともあります。