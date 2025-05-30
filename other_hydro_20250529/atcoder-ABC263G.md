## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc263/tasks/abc263_g

黒板に $ N $ 種類の整数が書かれています。 $ i $ 種類目の整数は $ A_i $ で、書かれている個数は $ B_i $ 個です。

あなたは次の操作を可能な限り繰り返すことができます。

- 黒板に書かれている $ 2 $ 個の整数 $ x,y $ であって、$ x+y $ が素数であるものを選ぶ。 選んだ $ 2 $ 個の整数を黒板から消す。

操作を最大で何回行えるか求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \vdots $ $ A_N $ $ B_N $

## 输出格式
答えを出力せよ。

## 题目大意
有 $n$ 种整数 $a_i$ ，第 $i$ 种有 $b_i$ 个。进行若干次操作，每次在这些数中取出两个，若它们的和为质数，分数加一，操作后把这两个数移去，求最大分数。

```input1
3
3 3
2 4
6 2
```

```output1
3
```

```input2
1
1 4
```

```output2
2
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ A_i\ \leq\ 10^7 $
- $ 1\ \leq\ B_i\ \leq\ 10^9 $
- $ A_i $ は全て異なる
- 入力は全て整数

### Sample Explanation 1

$ 2\ +\ 3\ =\ 5 $ であり、$ 5 $ は素数なので、$ 2 $ と $ 3 $ を選んで消す操作が行えます。また、それ以外の操作は行えません。 $ 2 $ は $ 4 $ 個、 $ 3 $ は $ 3 $ 個あるので、操作を $ 3 $ 回行うことができます。

### Sample Explanation 2

$ 1+\ 1\ =\ 2 $ であり、$ 2 $ は素数なので、$ 1 $ と $ 1 $ を選んで消す操作が行えます。$ 1 $ は $ 4 $ 個あるので、操作を $ 2 $ 回行うことができます。

