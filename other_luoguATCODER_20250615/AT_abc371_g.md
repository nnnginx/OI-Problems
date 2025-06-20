# AT_abc371_g [ABC371G] Lexicographically Smallest Permutation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc371/tasks/abc371_g

$ (1,2,\ldots,N) $ の並べ替え $ P=(P\ _\ 1,P\ _\ 2,\ldots,P\ _\ N),A=(A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N) $ が与えられます。

あなたは、次の操作を $ 0 $ 回以上好きな回数行うことができます。

- $ i=1,2,\ldots,N $ に対して**一斉に** $ A\ _\ i $ を $ A\ _\ {P\ _\ i} $ で置き換える。
 
得られる $ A $ としてありえるもののうち、辞書順で最小のものを出力してください。

 辞書順の大小とは？ 長さ $ N $ の列 $ A=(A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N),B=(B\ _\ 1,B\ _\ 2,\ldots,B\ _\ N) $ について、辞書順で $ A $ が $ B $ より小さいとは、次のことが成り立つことをいいます。

- ある整数 $ i\ (1\leq\ i\leq\ N) $ が存在し、$ A\ _\ i\lt\ B\ _\ i $ が成り立ち、$ 1\leq\ j\lt\ i $ を満たすすべての整数 $ j $ に対して $ A\ _\ j=B\ _\ j $ が成り立つ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ P\ _\ 1 $ $ P\ _\ 2 $ $ \ldots $ $ P\ _\ N $ $ A\ _\ 1 $ $ A\ _\ 2 $ $ \ldots $ $ A\ _\ N $

## 输出格式

$ 0 $ 回以上の操作の結果としてあり得る $ A $ のうち辞書順で最小のものを $ (A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N) $ として、$ A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N $ をこの順に空白を区切りとして $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
3 1 5 6 2 4
4 3 1 6 2 5
```

### 输出 #1

```
1 4 2 5 3 6
```

## 输入输出样例 #2

### 输入 #2

```
8
3 5 8 7 2 6 1 4
1 2 3 4 5 6 7 8
```

### 输出 #2

```
1 2 3 4 5 6 7 8
```

## 输入输出样例 #3

### 输入 #3

```
26
24 14 4 20 15 19 16 11 23 22 12 18 21 3 6 8 26 2 25 7 13 1 5 9 17 10
15 3 10 1 13 19 22 24 20 4 14 23 7 26 25 18 11 6 9 12 2 21 5 16 8 17
```

### 输出 #3

```
4 1 22 18 20 13 14 6 15 11 3 26 2 12 5 23 9 10 25 24 7 17 16 21 19 8
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq2\times10\ ^\ 5 $
- $ 1\leq\ P\ _\ i\leq\ N\ (1\leq\ i\leq\ N) $
- $ P\ _\ i\neq\ P\ _\ j\ (1\leq\ i\lt\ j\leq\ N) $
- $ 1\leq\ A\ _\ i\leq\ N\ (1\leq\ i\leq\ N) $
- $ A\ _\ i\neq\ A\ _\ j\ (1\leq\ i\lt\ j\leq\ N) $
- 入力はすべて整数
 
### Sample Explanation 1

はじめ、$ A=(4,3,1,6,2,5) $ です。 ここから操作を繰り返すと、以下のようになります。 - $ A=(1,4,2,5,3,6) $ となる。 - $ A=(2,1,3,6,4,5) $ となる。 - $ A=(3,2,4,5,1,6) $ となる。 - $ A=(4,3,1,6,2,5) $ となる。 以降、$ 4 $ 回操作を行うたびにもとの $ A $ に戻ります。 よって、このうち辞書順で最小である `1 4 2 5 3 6` を出力してください。

### Sample Explanation 2

$ 1 $ 度も操作をしなくても構いません。