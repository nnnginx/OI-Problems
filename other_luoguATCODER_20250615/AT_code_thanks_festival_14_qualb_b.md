# AT_code_thanks_festival_14_qualb_b 電卓ゲーム

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-thanks-festival-2014-b-open/tasks/code_thanks_festival_14_qualb_b

あなたが持っている電卓には、足し算(+)と掛け算(×)の、$ 2 $ つの演算子が存在します。

あなたには、 $ 3 $ つの数字 $ A,B,C $ が与えられます。 これらの数字を電卓に、「$ A $ → $ 演算子 $ → $ B $ → $ 演算子 $ → $ C $」の順番で入力します。

たとえば、$ (A,B,C)=(1,2,3) $ のとき、最初の演算を足し算、次の演算の演算を掛け算とすることを考えます。 この場合、入力は「$ 1 $ → $ + $ → $ 2 $ → $ × $ → $ 3 $」であり、計算結果は $ 9 $ です。電卓は順番に演算を行うため、演算子の優先順位は無視して左から計算します。

あなたは、各数字の間に入れる演算をうまく定めて最大値を得る一人遊びを行うことにしました。 各数字の間に入れる演算をうまく選ぶことによって得られる計算結果の最大値を求めて下さい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $

- $ 1 $ 行目には、数字 $ A\ (0\ ≦\ A\ ≦\ 9) $ が与えられる。
- $ 2 $ 行目には、数字 $ B\ (0\ ≦\ B\ ≦\ 9) $ が与えられる。
- $ 3 $ 行目には、数字 $ C\ (0\ ≦\ C\ ≦\ 9) $ が与えられる。

## 输出格式

$ 1 $ 行目に、計算結果の最大値を出力せよ。末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
1
2
3
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
1
0
9
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
2
3
4
```

### 输出 #3

```
24
```

## 输入输出样例 #4

### 输入 #4

```
9
9
0
```

### 输出 #4

```
81
```

## 说明/提示

### Sample Explanation 1

問題文で言及したケースです。 - 「$ 1 $ → $ + $ → $ 2 $ → $ + $ → $ 3 $」を計算すると $ 6 $ が得られます。 - 「$ 1 $ → $ + $ → $ 2 $ → $ × $ → $ 3 $」を計算すると $ 9 $ が得られます。 - 「$ 1 $ → $ × $ → $ 2 $ → $ + $ → $ 3 $」を計算すると $ 5 $ が得られます。 - 「$ 1 $ → $ × $ → $ 2 $ → $ × $ → $ 3 $」を計算すると $ 6 $ が得られます。 したがって、最大値の $ 9 $ を出力すれば良いです。

### Sample Explanation 2

「$ 1 $ → $ + $ → $ 0 $ → $ + $ → $ 9 $」を計算すると $ 10 $ が得られ、これが最大値である。

### Sample Explanation 3

「$ 2 $ → $ × $ → $ 3 $ → $ × $ → $ 4 $」を計算すると $ 24 $ が得られ、これが最大値である。

### Sample Explanation 4

「$ 9 $ → $ × $ → $ 9 $ → $ + $ → $ 0 $」を計算すると $ 81 $ が得られ、これが最大値である。