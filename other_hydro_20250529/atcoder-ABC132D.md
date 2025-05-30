## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc132/tasks/abc132_d

$ K $ 個の青いボールと $ N-K $ 個の赤いボールがあります。同じ色のボールは区別が不可能です。すぬけ君と高橋君はこれらのボールで遊んでいます。

まず、すぬけ君が、$ N $ 個のボールを左から右に一列に並べます。

次に、高橋君は、これらのうち $ K $ 個の青いボールのみを回収します。高橋君は、$ 1 $ 回の操作で連続して並ぶ青いボールを何個でも回収することができます。高橋君は、常に $ K $ 個の青いボールを回収するのにかかる操作の回数が最小になるように行動します。

$ K $ 個の青いボールを回収するために高橋君がちょうど $ i $ 回操作をする必要があるボールの並べ方は何通りあるでしょうか。 $ 1\ <\ =\ i\ <\ =\ K $ をみたす $ i $ それぞれについて答えを計算し、 $ 10^9+7 $ で割った余りを答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
$ i $ 行目 ($ 1\ <\ =\ i\ <\ =\ K $) に高橋君がちょうど $ i $ 回操作をする必要があるボールの並べ方の総数を $ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
### 题目描述
有 $K$ 个蓝球和 $N-K$ 个红球。同一颜色的球是完全相同的。Snuke 和 Takahashi 在玩这些球。

首先，Snuke 将把 $N$ 个球从左到右排成一排。

然后，Takahashi 将收走 $K$ 个蓝球。在一次操作中，他可以收走连续的一个区间的蓝球。他将以最少的操作数收走所有蓝球。

Snuke 有多少种排列这 $N$ 个球的方法，使得 Takahashi 至少操作 $i$ 次才能收走所有的 $K$ 个蓝球？对于每个 $i$（$1\le i\le K$）计算排列数对 $10^9+7$ 取模的结果。

------------

### 输入格式
从标准输入读取数据，输入格式如下：

$N\ K$

------------

### 输出格式
输出 $K$ 行。第 $i$ 行（$1\le i\le K$）表示有多少种排列这 $N$ 个球的方法，使得 Takahashi 至少操作 $i$ 次才能收走所有的 $K$ 个蓝球，对 $10^9+7$ 取模。

------------

### 说明/提示
#### 样例解释 1
有三种方法来排列球，使得 Takahashi 至少操作 $1$ 次：$(B, B, B, R, R)$，$(R, B, B, B, R)$ 和 $(R, R, B, B, B)$。（$R$ 和 $B$ 分别代表红色和蓝色）。

有六种方法来排列球，使得 Takahashi 至少操作 $2$ 次：$(B, B, R, B, R)$，$(B, B, R, R, B)$，$(R, B, B, R, B)$，$(R, B, B, R, B)$，$(B, R, B, B, R)$，和 $(B, R, R, B, B)$。

有一种方法来排列球，使得 Takahashi 至少操作 $3$ 次：$(B, R, B, R, B)$。

#### 样例解释 2
务必输出对 $10^9+7$ 的排列数。

```input1
5 3
```

```output1
3
6
1
```

```input2
2000 3
```

```output2
1998
3990006
327341989
```

## 提示
### 制約

- $ 1\ <\ =\ K\ <\ =\ N\ <\ =\ 2000 $

### Sample Explanation 1

高橋君がちょうど $ 1 $ 回操作をする必要があるボールの並べ方は (青, 青, 青, 赤, 赤), (赤, 青, 青, 青, 赤), (赤, 赤, 青, 青, 青) の $ 3 $ 通りです。 高橋君がちょうど $ 2 $ 回操作をする必要があるボールの並べ方は (青, 青, 赤, 青, 赤), (青, 青, 赤, 赤, 青), (赤, 青, 青, 赤, 青), (赤, 青, 赤, 青, 青), (青, 赤, 青, 青, 赤), (青, 赤, 赤, 青, 青) の $ 6 $ 通りです。 高橋君がちょうど $ 3 $ 回操作をする必要があるボールの並べ方は (青, 赤, 青, 赤, 青) のみの $ 1 $ 通りです。

### Sample Explanation 2

並べ方の総数を $ 10^9+7 $ で割った余りを出力することに注意してください。

