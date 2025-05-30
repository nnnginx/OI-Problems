## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc139/tasks/arc139_b

整数 $ P=0 $ があります。以下の $ 3 $ 種類の操作を任意の回数選んで行うことで $ P=N $ とするとき、コストの総和の最小値を求めてください。

- $ P $ を $ 1 $ 増やす。この操作はコストが $ X $ かかる。
- $ P $ を $ A $ 増やす。この操作はコストが $ Y $ かかる。
- $ P $ を $ B $ 増やす。この操作はコストが $ Z $ かかる。

$ T $ 個のテストケースが与えられるので、それぞれについて答えを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_T $

各テストケースは以下の形式で与えられます。

> $ N\ A\ B\ X\ Y\ Z $

## 输出格式
$ T $ 行出力してください。$ i $ 行目には、$ \mathrm{case}_i $ に対する答えを出力してください。

## 题目大意
给你一个数字 $N$ ，现在希望你用三个数字 $1,A,B$ 拼出 $N$

但是使用一次 $1$ 要花掉 $X$ 元，用一次 $A$ 花掉$Y$ 元，用一次 $B$ 花掉 $Z$ 元

请你求出最小的花费

本题有多组数据。第一行输入数据组数 $T~(1\leqslant T\leqslant 100)$ 。接下来行每行输入六个整数，$N,A,B,X,Y,Z$ （均小于 $10^9$ ）

输出时每行一个数，表示最小花费

```input1
5
10 3 5 2 3 6
10 3 5 1 1000000000 1000000000
139 2 139 1 1 1
139 1 1 1 1 1
139 7 10 3845 26982 30923
```

```output1
11
10
1
139
436604
```

## 提示
### 制約

- $ 1\ \le\ T\ \le\ 100 $
- $ 1\ \le\ N,A,B,X,Y,Z\ \le\ 10^9 $
- 入力は全て整数である。

### Sample Explanation 1

$ 1 $ 個目のテストケースでは、例えば以下のようにするとコスト $ 11 $ で $ P=10 $ とでき、これが最適です。 - $ P $ を $ 3 $ 増やす。$ P=3 $ となる。コストが $ 3 $ かかる。 - $ P $ を $ 1 $ 増やす。$ P=4 $ となる。コストが $ 2 $ かかる。 - $ P $ を $ 3 $ 増やす。$ P=7 $ となる。コストが $ 3 $ かかる。 - $ P $ を $ 3 $ 増やす。$ P=10 $ となる。コストが $ 3 $ かかる。

