# AT_joi2019ho_c たのしいたのしいたのしい家庭菜園 (Growing Vegetables is Fun 3)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2019ho/tasks/joi2019ho_c

JOI 君は，長年にわたる家庭菜園の経験を生かして，自宅の庭で新たにジョイ草という植物を育てている．庭には東西方向に並んだ $ N $ 個のプランターがあり，西側から順に $ 1 $ から $ N $ までの番号がついている．ジョイ草は全部で $ N $ 株あり，それぞれのプランターに $ 1 $ 株ずつ植えてある．

春になって様子を見に行った JOI 君は，ジョイ草が予想に反して色とりどりの葉を付けていることに気がついた．さらに，ジョイ草が思ったほど生育していないことに気がついた．JOI 君はこれらのことを不思議に思い，本で調べたところ，次のことがわかった：

- ジョイ草には $ 3 $ 種類あり，それぞれ赤，緑，黄の葉を付ける．
- 葉の色が同じジョイ草を近くに置くと，その成長が阻害されてしまう．

そこで，JOI 君は，ジョイ草を並び替えて，葉の色が同じジョイ草が隣り合わないようにすることにした．このとき，JOI 君は隣り合う $ 2 $ つのジョイ草を入れ替えることしかできない．つまり，$ 1 $ 回の操作で JOI 君はプランター $ i $ ($ 1\ \leqq\ i\ \leqq\ N\ -\ 1 $) を任意に $ 1 $ つ選び，プランター $ i $ のジョイ草とプランター $ i\ +\ 1 $ のジョイ草を入れ替えることができる．JOI 君は，できるだけ少ない回数の操作で，葉の色が同じジョイ草が隣り合わないようにしたい．

ジョイ草の数と，それぞれのジョイ草の葉の色が与えられたとき，葉の色が同じジョイ草が隣り合わないように並び替えるために必要な操作回数の最小値を求めるプログラムを作成せよ．

- - - - - -

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $

$ S $ は長さ $ N $ の文字列で，その $ i $ 文字目 ($ 1\ \leqq\ i\ \leqq\ N $) は，プランター $ i $ に植えてあるジョイ草の葉の色が赤ならば `R`，緑ならば `G`，黄ならば `Y` である．

## 输出格式

標準出力に，必要な操作回数の最小値を $ 1 $ 行で出力せよ．ただし，葉の色が同じジョイ草が隣り合わないように並び替えることが不可能ならば，代わりに $ -1 $ を出力せよ．

- - - - - -

## 输入输出样例 #1

### 输入 #1

```
5
RRGYY
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6
RRRRRG
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
20
YYGYYYGGGGRGYYGRGRYG
```

### 输出 #3

```
8
```

## 说明/提示

### 制約

- $ 1\ \leqq\ N\ \leqq\ 400 $．
- $ S $ は長さ $ N $ の文字列である．
- $ S $ の各文字は `R`，`G`，`Y` のいずれかである．

### 小課題

1. ($ 5 $ 点) $ N\ \leqq\ 15 $．
2. ($ 55 $ 点) $ N\ \leqq\ 60 $．
3. ($ 15 $ 点) $ S $ の各文字は `R`，`G` のいずれかである．
4. ($ 25 $ 点) 追加の制約はない．

- - - - - -

### Sample Explanation 1

この入力例では，例えば次のようにすると，葉の色が同じジョイ草が隣り合わないようにすることができる． - まず，プランター $ 3 $ のジョイ草とプランター $ 4 $ のジョイ草を入れ替える． - 次に，プランター $ 2 $ のジョイ草とプランター $ 3 $ のジョイ草を入れ替える． このようにすると，ジョイ草の並びは `RYRGY` のようになる．$ 1 $ 回以下の操作で葉の色が同じジョイ草が隣り合わないようにすることはできないので，$ 2 $ を出力する． - - - - - -

### Sample Explanation 2

この入力例では，どのように操作をしても，葉の色が同じジョイ草が隣り合わないようにすることはできない． - - - - - -