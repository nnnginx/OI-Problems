## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc220/tasks/abc220_d

$ 0 $ 以上 $ 9 $ 以下の整数からなる長さ $ N $ の数列 $ A=(A_1,\dots,A_N) $ があり、この順に左から右に並んでいます。

数列の長さが $ 1 $ になるまで、操作 $ F $ または操作 $ G $ を繰り返し行います。

- 操作 $ F $ ：左端の $ 2 $ つの値 ( $ x,y $ とする ) を削除した後、一番左に $ (x+y)\%10 $ を挿入する
- 操作 $ G $ ：左端の $ 2 $ つの値 ( $ x,y $ とする ) を削除した後、一番左に $ (x\times\ y)\%10 $ を挿入する

なお、$ a\%b $ は $ a $ を $ b $ で割った余りを意味します。

$ K=0,1,\dots,9 $ について、以下の問題に答えてください。

> 操作手順としてあり得るものは $ 2^{N-1} $ 通りありますが、このうち最終的に残る値が $ K $ となる操作手順は何通りありますか？  
>  ただし答えは非常に大きくなる可能性があるので、$ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \dots $ $ A_N $

## 输出格式
答えを $ 10 $ 行に出力せよ。  
 ただし、$ i $ 行目には $ K=i-1 $ としたときの答えを出力せよ。

## 题目大意
给定一个数组 $A=(A_1,A_2 \dots A)$，从左到右排列，每个元素都是 $0\sim9$ 中的数字，你可以进行 $n-1$ 次操作使得数组长为 $1$，每次操作为以下两者之一：

+ 删除最左边两个数 $x,y$，在最左端插入 $(x+y) \bmod 10$。
+ 删除最左边两个数 $x,y$，在最左端插入 $(x\times y)\bmod 10$。

    对于 $k$ 从 $0$ 到 $9$，有多少种方式使得最后剩余的数是 $k$？对于每个 $k$ 输出一行答案，对 $998244353$ 取模。

```input1
3
2 7 6
```

```output1
1
0
0
0
2
1
0
0
0
0
```

```input2
5
0 1 2 3 4
```

```output2
6
0
1
1
4
0
1
1
0
2
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 9 $
- 入力は全て整数

### Sample Explanation 1

$ 1 $ 回目に操作 $ F $ 、$ 2 $ 回目に操作 $ F $ を行ったとき：数列は $ (2,7,6)→(9,6)→(5) $ となります。 $ 1 $ 回目に操作 $ F $ 、$ 2 $ 回目に操作 $ G $ を行ったとき：数列は $ (2,7,6)→(9,6)→(4) $ となります。 $ 1 $ 回目に操作 $ G $ 、$ 2 $ 回目に操作 $ F $ を行ったとき：数列は $ (2,7,6)→(4,6)→(0) $ となります。 $ 1 $ 回目に操作 $ G $ 、$ 2 $ 回目に操作 $ G $ を行ったとき：数列は $ (2,7,6)→(4,6)→(4) $ となります。

