# AT_arc082_d [ARC082F] Sandglass

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc082/tasks/arc082_d

パーツAとパーツBからなる砂時計があります。これらのパーツにはいくらかの砂が入っています。 砂時計を置くときはパーツAとパーツBのどちらかが上になり、そうでないほうが下になります。

$ 1 $ 秒間に $ 1 $ \[g\] の砂が上にあるパーツから下にあるパーツに落ちます。 ただし、上のパーツにもう砂が残っていない場合は砂は落ちません。

はじめ時刻 $ 0 $ にパーツAが上にあり、$ a $ \[g\] の砂がパーツAに入っていて、$ X-a $ \[g\] の砂がパーツBに入っています(すなわち、合計 $ X $ \[g\] の砂が入っています)。

時刻 $ r_1,r_2,\ ..,\ r_K $ に砂時計をひっくり返します。この操作は瞬間的に行われ、時間はかからないものとします。なお、時刻 $ t $ とは時刻 $ 0 $ の $ t $ 秒後を指します。

クエリが $ Q $ 個与えられます。 各クエリは $ (t_i,a_i) $ の形をしています。 各クエリに対し、$ a=a_i $ だとして、時刻 $ t_i $ にパーツAに入っている砂の量が何gか答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ X $ $ K $ $ r_1 $ $ r_2 $ .. $ r_K $ $ Q $ $ t_1 $ $ a_1 $ $ t_2 $ $ a_2 $ $ : $ $ t_Q $ $ a_Q $

## 输出格式

各クエリの答えを $ 1 $ 行ごとに出力せよ。

## 输入输出样例 #1

### 输入 #1

```
180
3
60 120 180
3
30 90
61 1
180 180
```

### 输出 #1

```
60
1
120
```

## 输入输出样例 #2

### 输入 #2

```
100
1
100000
4
0 100
90 100
100 100
101 100
```

### 输出 #2

```
100
10
0
0
```

## 输入输出样例 #3

### 输入 #3

```
100
5
48 141 231 314 425
7
0 19
50 98
143 30
231 55
342 0
365 100
600 10
```

### 输出 #3

```
19
52
91
10
58
42
100
```

## 说明/提示

### 制約

- $ 1\ <\ =X\ <\ =10^9 $
- $ 1\ <\ =K\ <\ =10^5 $
- $ 1\ <\ =r_1\ <\ r_2\ <\ ..\ <\ r_K\ <\ =10^9 $
- $ 1\ <\ =Q\ <\ =10^5 $
- $ 0\ <\ =t_1\ <\ t_2\ <\ ..\ <\ t_Q\ <\ =10^9 $
- $ 0\ <\ =a_i\ <\ =X\ (1\ <\ =i\ <\ =Q) $
- 入力値はすべて整数

### Sample Explanation 1

$ 1 $ つめのクエリでは、はじめパーツAに $ 90 $ \\\[g\\\] 入っていた砂が $ 30 $ \\\[g\\\] 減り、$ 60 $ \\\[g\\\] になります。 $ 2 $ つめのクエリでは、はじめパーツAに入っていた $ 1 $ \\\[g\\\] の砂がパーツBに落ちた後、$ 59 $ 秒間変化は起こりません。ここで砂時計をひっくり返し、その $ 1 $ 秒後にパーツAに入っている砂の量を聞かれているため、答えは $ 1 $ \\\[g\\\] になります。

### Sample Explanation 2

どのクエリでもはじめにパーツAに入っている砂は $ 100 $ \\\[g\\\] で、砂時計をひっくり返す前の時間での値を聞いています。