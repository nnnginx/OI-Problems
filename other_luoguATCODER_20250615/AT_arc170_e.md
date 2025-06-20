# AT_arc170_e [ARC170E] BDFS

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc170/tasks/arc170_e

整数 $ N,P $ が与えられます．

頂点に $ 1 $ から $ N $ の番号が付いた $ N $ 頂点 $ N $ 辺のグラフがあります．$ i $ 番目の辺は頂点 $ i $ と頂点 $ i+1 $ を双方向に結んでいます．ここで頂点 $ N+1 $ は頂点 $ 1 $ を意味します．

以下のアルゴリズムを行い，長さ $ N $ の数列 $ D=(D_1,D_2,\ldots,D_N) $ を得ます．

- 長さ $ N $ の整数列 $ D $ を $ D=(D_1,\ldots,D_N)=(-1,\ldots,-1) $ で定める．また，数のペアの列 $ Q $ を $ Q=((1,0)) $ で定める．$ Q $ が空でない限り，以下の処理を繰り返す．
  
  
  - $ Q $ の先頭の要素を $ (v,d) $ とする．先頭の要素を削除する．
  - $ D_v\ =\ -1 $ の場合，$ D_v\ :=\ d $ とし，頂点 $ v $ に隣接して $ D_x=-1 $ を満たすような各頂点 $ x $ に対して以下の処理を行う．ただし条件を満たす $ x $ が複数存在する場合，頂点番号の小さい順に処理を行う．
      
      
      1. 確率 $ \frac{P}{100} $ で $ Q $ の**先頭**に $ (x,d+1) $ を追加する．
      2. $ Q $ の先頭への $ (x,d+1) $ の追加を行わなかった場合，$ Q $ の**末尾**に $ (x,d+1) $ を追加する．
 
最終的に得られる $ D $ の要素の総和の期待値を $ \text{mod\ }\ 998244353 $ で求めてください．

$ T $ 個のテストケースが与えられるので，それぞれについて答えてください．

   期待値 $ \text{mod\ }\ 998244353 $ の定義  求める期待値は必ず有理数になることが証明できます． また，この問題の制約下では，その値を既約分数 $ \frac{P}{Q} $ で表したときに $ Q $ が $ 998244353 $ で割り切れないことが保証されます． このとき $ R\times\ Q\ \equiv\ P\pmod{998244353} $ を満たすような $ 0 $ 以上 $ 998244352 $ 以下の整数 $ R $ が一意に定まります．この $ R $ を 答えてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ T $ $ \mathrm{case}_1 $ $ \vdots $ $ \mathrm{case}_T $

各ケースは以下の形式で与えられる．

> $ N $ $ P $

## 输出格式

$ T $ 行出力せよ．$ i $ 行目 $ (1\ \leq\ i\ \leq\ T) $ には， $ i $ 番目のテストケースの答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3
3 50
4 1
1000000000000000000 70
```

### 输出 #1

```
499122179
595552585
760296751
```

## 说明/提示

### 制約

- $ 1\ \leq\ T\ \leq\ 10^4 $
- $ 3\ \leq\ N\ \leq\ 10^{18} $
- $ 1\leq\ P\ \leq\ 99 $
- 入力される数値は全て整数
 
### Sample Explanation 1

$ 1 $ 番目のテストケースでは，例えば以下のようにアルゴリズムは動きます． - はじめ，$ D=(-1,-1,-1),\ Q=((1,0)) $ である．$ Q $ の先頭の要素 $ (1,0) $ を削除する． - $ D_1\ =\ -1 $ なので，$ D_1\ :=\ 0 $ とする．頂点 $ 1 $ に隣接して $ D_x=\ -1 $ を満たすような頂点 $ x $ は $ 2,3 $ が考えられる． - $ Q $ の先頭に $ (2,1) $ を追加する．$ Q $ の末尾に $ (3,1) $ を追加する．$ Q=((2,1),(3,1)) $ となる． - $ Q $ の先頭の要素 $ (2,1) $ を削除する． - $ D_2\ =\ -1 $ なので，$ D_2\ :=\ 1 $ とする．頂点 $ 2 $ に隣接して $ D_x=\ -1 $ を満たすような頂点 $ x $ は $ 3 $ が考えられる． - $ Q $ の先頭に $ (3,2) $ を追加する．$ Q=((3,2),(3,1)) $ となる． - $ Q $ の先頭の要素 $ (3,2) $ を削除する． - $ D_3\ =\ -1 $ なので，$ D_3\ :=\ 2 $ とする．頂点 $ 3 $ に隣接して $ D_x=\ -1 $ を満たすような頂点 $ x $ は存在しないので何もしない． - $ Q $ の先頭の要素 $ (3,1) $ を削除する． - $ D_3\ =2 $ なので何もしない． - $ Q $ が空になったので処理を終了する． この場合，最終的に $ D=(0,1,2) $ が得られます．アルゴリズムが上記の動作をする確率は $ \frac{1}{8} $ であり，$ D $ の要素の総和の期待値は $ \frac{5}{2} $ です．