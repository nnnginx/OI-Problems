# AT_abc272_h [ABC272Ex] Flipping Coins 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc272/tasks/abc272_h

$ 0,1,\ldots,N-1 $ の番号がついた $ N $ 枚のコインが並べられています。はじめ、全てのコインは表を向いています。また、 $ 0 $ 以上 $ N-1 $ 以下の整数からなる長さ $ N $ の数列 $ A $ が与えられます。

すぬけ君は $ (1,\ldots,N) $ を並び替えて得られる順列 $ p=(p_1,p_2,\ldots,p_N) $ を等確率で $ 1 $ つ選び $ N $ 回操作を行います。 $ i\ (1\leq\ i\ \leq\ N) $ 回目の操作では以下の処理が行われます。

- コイン $ (i-1)\ \bmod\ N $、コイン$ (i-1+1\ )\ \bmod\ N $、$ \ldots $、コイン $ (i\ -1+\ A_{p_i})\ \bmod\ N $ の $ (A_{p_i}+1) $ 枚のコインを全てひっくり返す。

$ N $ 回の操作の後、表向きのコインの枚数を $ k $ としてすぬけ君はお母さんから $ k $ 円もらえます。

すぬけ君が得られるお金の期待値を $ \text{mod\ }\ 998244353 $ で求めてください。

期待値 $ \text{mod\ }\ 998244353 $ の定義この問題で求める期待値は必ず有理数になることが証明できます。 また、この問題の制約下では、求める期待値を既約分数 $ \frac{y}{x} $ で表したときに $ x $ が $ 998244353 $ で割り切れないことが保証されます。

このとき $ xz\ \equiv\ y\ \pmod{998244353} $ を満たすような $ 0 $ 以上 $ 998244352 $ 以下の整数 $ z $ が一意に定まります。この $ z $ を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
0 1
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
4
3 1 1 2
```

### 输出 #2

```
665496237
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\leq\ 2\times\ 10^5 $
- $ 0\leq\ A_i\ \leq\ N-1 $
- 入力は全て整数

### Sample Explanation 1

$ p $ としてありうるのは $ (1,2) $ と $ (2,1) $ です。 - $ p $ として $ (1,2) $ が選ばれたとき $ 1 $ 回目の操作ではコイン $ 0 $ をひっくり返します。 $ 2 $ 回目の操作ではコイン $ 1 $ とコイン $ 0 $ をひっくり返します。最終的に表向きのコインはコイン $ 0 $ の $ 1 $ 枚なので、$ 1 $ 円もらえます。 - $ p $ として $ (2,1) $ が選ばれたとき $ 1 $ 回目の操作ではコイン $ 0 $ とコイン $ 1 $ をひっくり返します。 $ 2 $ 回目の操作ではコイン $ 1 $ をひっくり返します。最終的に表向きのコインはコイン $ 1 $ の $ 1 $ 枚なので、$ 1 $ 円もらえます。 以上より、得られるお金の期待値は $ 1 $ 円 です。

### Sample Explanation 2

期待値を $ \text{mod\ }\ 998244353 $ で出力してください。