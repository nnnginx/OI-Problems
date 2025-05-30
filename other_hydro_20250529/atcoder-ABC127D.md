## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc127/tasks/abc127_d

$ N $ 枚のカードがあり、$ i $ 番目のカードには整数 $ A_i $ が書かれています。

あなたは、$ j\ =\ 1,\ 2,\ ...,\ M $ について順に以下の操作を $ 1 $ 回ずつ行います。

操作: カードを $ B_j $ 枚まで選ぶ($ 0 $ 枚でもよい)。選んだカードに書かれている整数をそれぞれ $ C_j $ に書き換える。

$ M $ 回の操作終了後に $ N $ 枚のカードに書かれた整数の合計の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $ $ B_1 $ $ C_1 $ $ B_2 $ $ C_2 $ $ \vdots $ $ B_M $ $ C_M $

## 输出格式
$ M $ 回の操作終了後に $ N $ 枚のカードに書かれた整数の合計の最大値を出力せよ。

## 题目大意
### 题目描述
有一个长度为 $n$ 的序列 $A_{1},A_{2},\cdots,A_{n} $

你可以对这个序列依次进行 $m$ 次操作，第 $ i$ 次操作中，你可以选择至多 $B_{i}$ 个数（可以一个都不选），然后将这些数变成 $C_{i}$

问进行这 $m$ 次操作后，这个序列所有元素之和可能的最大值是多少

### 输入格式
第一行两个整数 $n,m$

第二行 $n$ 个整数，表示序列 $A$

接下来 $m$ 行，每行两个整数 $B_{i},C_{i}$ ，表示一次操作

### 输出格式
一行一个整数，表示答案

### 数据范围与提示
$1 \le n,m \le 10^5,1 \le A_{i},C{i} \le 10^9,1 \le B_{i} \le n$

```input1
3 2
5 1 4
2 3
1 5
```

```output1
14
```

```input2
10 3
1 8 5 7 100 4 52 33 13 5
3 10
4 30
1 4
```

```output2
338
```

```input3
3 2
100 100 100
3 99
3 99
```

```output3
300
```

```input4
11 3
1 1 1 1 1 1 1 1 1 1 1
3 1000000000
4 1000000000
3 1000000000
```

```output4
10000000001
```

## 提示
### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ A_i,\ C_i\ \leq\ 10^9 $
- $ 1\ \leq\ B_i\ \leq\ N $

### Sample Explanation 1

$ 2 $ 番目のカードに書かれた整数を $ 5 $ に書き換えることで、$ 3 $ 枚のカードに書かれた整数の合計が $ 5\ +\ 5\ +\ 4\ =\ 14 $ となり、このときが最大です。

### Sample Explanation 4

出力が $ 32 $ bit 整数型に収まらない場合があります。

