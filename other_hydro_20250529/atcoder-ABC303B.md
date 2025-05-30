## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc303/tasks/abc303_b

$ 1,2,\ldots,N $ と番号づけられた $ N $ 人が $ M $ 回、一列に並んで集合写真を撮りました。$ i $ 番目の撮影で左から $ j $ 番目に並んだ人の番号は $ a_{i,j} $ です。

ある二人組は $ M $ 回の撮影で一度も連続して並ばなかった場合、不仲である可能性があります。

不仲である可能性がある二人組の個数を求めてください。なお、人 $ x $ と人 $ y $ からなる二人組と人 $ y $ と人 $ x $ からなる二人組は区別しません。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_{1,1} $ $ \ldots $ $ a_{1,N} $ $ \vdots $ $ a_{M,1} $ $ \ldots $ $ a_{M,N} $

## 输出格式
答えを出力せよ。

## 题目大意
### 题目描述
有 $n$ 个人拍了 $m$ 张照片，第 $i$ 张照片中从左往右数的第 $j$ 个人编号为 $a_{i,j}$，所有照片都是 $n$ 个人的合影。

若两个人在 $m$ 张照片中没有一张是站在相邻位置的，那么说这两个人是一对不开心的人，交换顺序也算同一对，允许一个人在多对不开心的人中出现。

需要求出这 $n$ 个人中，有多少对不开心的人。

### 输入格式
第一行输入两个整数 $n~(2\le n\le 50)$ 和 $m~(1\le m\le 50)$，表示人数和照片数。
第 $2\sim m+1$ 行输入一个 $m$ 行 $n$ 列的矩阵 $a$，表示 $m$ 张照片每张照片中人们的排列顺序。
### 输出格式
输出一个整数，表示不开心的人的对数。

Translated by [Special_Tony](https://www.luogu.com.cn/user/571147) .

```input1
4 2
1 2 3 4
4 3 1 2
```

```output1
2
```

```input2
3 3
1 2 3
3 1 2
1 2 3
```

```output2
0
```

```input3
10 10
4 10 7 2 8 3 9 1 6 5
3 6 2 9 1 8 10 7 4 5
9 3 4 5 7 10 1 8 2 6
7 3 1 8 4 9 5 6 2 10
5 2 1 4 10 7 9 8 3 6
5 8 1 6 9 3 2 4 7 10
8 10 3 4 5 7 2 9 6 1
3 10 2 7 8 5 1 4 9 6
10 6 1 5 4 2 3 8 9 7
4 5 9 1 8 2 7 6 3 10
```

```output3
6
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 50 $
- $ 1\ \leq\ M\ \leq\ 50 $
- $ 1\ \leq\ a_{i,j}\ \leq\ N $
- $ a_{i,1},\ldots,a_{i,N} $ には $ 1,\ldots,N $ が $ 1 $ 回ずつ現れる
- 入力はすべて整数
 
### Sample Explanation 1

人 $ 1 $ と人 $ 4 $ からなる二人組と、人 $ 2 $ と人 $ 4 $ からなる二人組がそれぞれ不仲である可能性があります。

