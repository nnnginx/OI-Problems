# AT_arc124_e [ARC124E] Pass to Next

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc124/tasks/arc124_e

$ 1,\ 2,\ \ldots,\ N $ の番号がついた人が円環状に並んでいます。

$ 1\ \leq\ i\ \leq\ N-1 $ を満たす人 $ i $ の右隣に人 $ i+1 $ がおり、人 $ N $ の右隣には人 $ 1 $ がいます。

人 $ i $ ははじめ、$ a_i $ 個のボールを持っています。

以下の処理を一度だけ行います。

- それぞれの人が現在持っているボールのうちいくつかを選ぶ($ 0 $ 個でもよい)
- その後、選んだボールを全て右隣の人に **同時に** 渡す。
- 長さ $ N $ の数列を作る。数列の $ i $ 番目の要素は人 $ i $ が現在持っているボールの個数と等しい値である。

処理の結果できる数列としてありうるものの集合を $ S $ とします。 たとえば、$ a=(1,1,1) $ のとき $ S=\ \{(0,1,2),(0,2,1),(1,0,2),(1,1,1),(1,2,0),(2,0,1),(2,1,0)\ \} $ です。

$ \sum_{x\ \in\ S}\ \prod_{i=1}^{N}\ x_i $ を $ 998244353 $ で割ったあまりを計算してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_{1} $ $ a_{2} $ $ \cdots $ $ a_{N} $

## 输出格式

$ \sum_{x\ \in\ S}\ \prod_{i=1}^{N}\ x_i $ を $ 998244353 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 1 1
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
3
2 1 1
```

### 输出 #2

```
6
```

## 输入输出样例 #3

### 输入 #3

```
20
5644 493 8410 8455 7843 9140 3812 2801 3725 6361 2307 1522 1177 844 654 6489 3875 3920 7832 5768
```

### 输出 #3

```
864609205
```

## 说明/提示

### 制約

- 与えられる入力は全て整数
- $ 3\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ a_i\ \leq\ 10^9 $

### Sample Explanation 1

\- $ S=\ \{(0,1,2),(0,2,1),(1,0,2),(1,1,1),(1,2,0),(2,0,1),(2,1,0)\ \} $ です。 - $ \sum_{x\ \in\ S}\ \prod_{i=1}^{N}\ x_i $ は $ 1 $ です。

### Sample Explanation 3

\- $ 998244353 $ で割ったあまりを求めるのを忘れずに。