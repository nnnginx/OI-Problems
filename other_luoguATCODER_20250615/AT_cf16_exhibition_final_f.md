# AT_cf16_exhibition_final_f Intervals

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf16-exhibition-final/tasks/cf16_exhibition_final_f

すぬけ君は $ N $ 個の区間を誕生日プレゼントとしてもらいました。 $ i $ 番目の区間は $ [-L_i,\ R_i] $ でした。 $ L_i $ と $ R_i $ は正であることが保証されています。 つまり、原点は必ず各区間の内側にあります。

すぬけ君は区間が重なっているのが嫌いなので、いくつかの区間を動かすことにしました。 任意の正整数 $ d $ に対し、$ d $ ドル払うと一つの区間を選んでそれを距離 $ d $ 動かすことができます。 つまり、選んだ区間が $ [a,\ b] $ のとき、それを $ [a+d,\ b+d] $ または $ [a-d,\ b-d] $ にすることができます。

すぬけ君は、このタイプの操作を任意の回数できます。 すべての操作の後、どの二つの区間も交わっていてはいけません (境界が接していることは許されます)。 正確には、任意の二つの区間に対し、その共通部分の長さが 0 になっている必要があります。

目的を達成するのに必要な最小のコストを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ L_1 $ $ R_1 $ : $ L_N $ $ R_N $

## 输出格式

目的を達成するのに必要な最小のコストを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
2 7
2 5
4 1
7 5
```

### 输出 #1

```
22
```

## 输入输出样例 #2

### 输入 #2

```
20
97 2
75 25
82 84
17 56
32 2
28 37
57 39
18 11
79 6
40 68
68 16
40 63
93 49
91 10
55 68
31 80
57 18
34 28
76 55
21 80
```

### 输出 #2

```
7337
```

## 说明/提示

### 制約

- $ 1\ <\ =\ N\ <\ =\ 5000 $
- $ 1\ <\ =\ L_i,\ R_i\ <\ =\ 10^9 $
- 入力される値は全て整数である。

### Sample Explanation 1

一つの最適な方法は以下の通りです: - 区間 $ [-2,\ 7] $ を $ [6,\ 15] $ に $ 8 $ ドルで動かす - 区間 $ [-2,\ 5] $ を $ [-1,\ 6] $ に $ 1 $ ドルで動かす - 区間 $ [-4,\ 1] $ を $ [-6,\ -1] $ に $ 2 $ ドルで動かす - 区間 $ [-7,\ 5] $ を $ [-18,\ -6] $ に $ 11 $ ドルで動かす コストの合計は $ 8\ +\ 1\ +\ 2\ +\ 11\ =\ 22 $ ドルとなります。