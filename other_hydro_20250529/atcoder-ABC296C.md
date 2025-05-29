## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc296/tasks/abc296_c

長さ $ N $ の数列 $ A=(A_1,\ldots,A_N) $ が与えられます。

$ 1\leq\ i,j\ \leq\ N $ である組 $ (i,j) $ であって、$ A_i-A_j=X $ となるものが存在するかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式
$ 1\leq\ i,j\ \leq\ N $ である組 $ (i,j) $ であって、$ A_i-A_j=X $ となるものが存在するとき `Yes`、存在しないとき `No` と出力せよ。

## 题目大意
有一个长度为 $n$ 的数组 $a$，给定一个数 $x$，确定是否存在一组 $(i,j)$ 满足 $a_i-a_j=x$。

Translated by @[Zealous_YH](https://www.luogu.com.cn/user/399150)

```input1
6 5
3 1 4 1 5 9
```

```output1
Yes
```

```input2
6 -4
-2 -7 -1 -8 -2 -8
```

```output2
No
```

```input3
2 0
141421356 17320508
```

```output3
Yes
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ -10^9\ \leq\ A_i\ \leq\ 10^9 $
- $ -10^9\ \leq\ X\ \leq\ 10^9 $
- 入力は全て整数である
 
### Sample Explanation 1

$ A_6-A_3=9-4=5 $ です。

### Sample Explanation 2

$ A_i-A_j=-4 $ となる組 $ (i,j) $ は存在しません。

### Sample Explanation 3

$ A_1-A_1=0 $ です。

