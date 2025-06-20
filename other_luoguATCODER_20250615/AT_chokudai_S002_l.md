# AT_chokudai_S002_l 長方形 β

## 题目描述

[problemUrl]: https://atcoder.jp/contests/chokudai_S002/tasks/chokudai_S002_l

$ N $ 個の長方形があり、長方形 $ i $ の幅と高さはそれぞれ $ A_i,\ B_i $ です。

すぬけ君はこれらの長方形の中からいくつかを選んで順番に重ねることで $ 1 $ つの模様を作ろうとしています。 このとき、$ j\ (2\ \leq\ j) $ 番目に配置する長方形は以下の条件を満たすようにしなければなりません。

- $ j-1 $ 番目に配置した長方形の内部に完全に含まれる。
- $ j-1 $ 番目に配置した長方形と辺どうしが接してはならない。
- 各辺は $ j-1 $ 番目に配置した長方形のいずれかの辺と平行になっていなければならない。

なお、長方形を配置する際は**幅と高さを入れ替えても構いません**。また、長方形を配置する順番は長方形の番号に関係なく自由に決めることができます。

すぬけ君は最大でいくつの長方形が重なった模様を作ることができるでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ : $ $ A_N $ $ B_N $

## 输出格式

すぬけ君が重ねることのできる長方形の個数の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
3 4
1 5
5 5
3 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3
1000000000 1000000000
1000000000 1000000000
1000000000 1
```

### 输出 #2

```
1
```

## 说明/提示

### 制約

入力は以下の条件を満たす。

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i,B_i\ \leq\ 10^9 $
- 入力される値は全て整数

### Sample Explanation 1

長方形 $ 3 $、長方形 $ 1 $、長方形 $ 4 $ をこの順で図のように配置すると $ 3 $ つの長方形を重ねることができます。 長方形の幅と高さを入れ替えても構わない点に注意してください。 !\[d1833dc2257ec22da947ab7e7c018515.png\](https://img.atcoder.jp/chokudai\_S002/d1833dc2257ec22da947ab7e7c018515.png)

### Sample Explanation 2

辺どうしが接してはいけない点に注意してください。