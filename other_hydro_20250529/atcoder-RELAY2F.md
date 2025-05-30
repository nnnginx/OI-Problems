## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf17-relay-open/tasks/relay2_f

東西方向に伸びる細長い森に $ N $ 匹のけものが生息しています。以下では、森の西端から $ p $ メートルの地点を地点 $ p $ と呼びます。西から $ i $ 匹目にいるけもの $ (1\ <\ =\ i\ <\ =\ N) $ は地点 $ x_i $ におり、捕獲すると $ s_i $ 円で売れます。

あなたは整数 $ L, $ $ R $ $ (L\ <\ =\ R) $ を選び、地点 $ L $ から地点 $ R $ までの両端を含む範囲、$ [L,\ R] $ に網を放ちます。すると、その範囲内のけものがすべて捕獲されます。ただし、網に $ R\ -\ L $ 円のコストがかかり、あなたの利益は $ ( $捕獲されたすべてのけもの $ i $ に対する $ s_i $ の合計$ )\ -\ (R\ -\ L) $ 円となります。

網を一度だけ放つとき、得られる最大の利益はいくらでしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ s_1 $ $ x_2 $ $ s_2 $ $ : $ $ x_N $ $ s_N $

## 输出格式
得られる最大の利益が $ X $ 円のとき、$ X $ の値を出力せよ。

## 题目大意
# 题目大意

在东西方向延伸的细长的森林里栖息着 $N$ 只动物。从森林的最左端到 $p$ 米的地点称为地点 $p$ 。若第i头动物到森林最左端的距离为 $x$（1≤i≤N）那么它就在地点 $x_i$ ，若捕获的话你可以以 $s_i$ 日元卖出。

选择两个整数 $L$ 和 $R$（L≤R），那么，从 $L$ 到 $R$ 范围内的动物就会全部被捕获。但是，买网要花费 $R$-$L$日元，所以你的利益=(被捕获的所有的除物i的合计)-($R$-$L$)日元。

若你只放一次网，得到的最大利益是多少呢？

# 输入格式 

$x_1$ $s_1$

$x_2$ $s_2$

$:$

$x_N$ $s_N$

# 输出格式

输出最大利益X

# 数据范围

1 ≤ $N$ ≤ 2 × $10_5$

1 ≤ x1 < x2 < ... < $x_N$ ≤ $10_15$

1 ≤ $s_i$ ≤ $10_9$

所有输入数据皆为整数.

```input1
5
10 20
40 50
60 30
70 40
90 10
```

```output1
90
```

```input2
5
10 2
40 5
60 3
70 4
90 1
```

```output2
5
```

```input3
4
1 100
3 200
999999999999999 150
1000000000000000 150
```

```output3
299
```

## 提示
### 制約

- $ 1\ <\ =\ N\ <\ =\ 2\ ×\ 10^5 $
- $ 1\ <\ =\ x_1\ <\ x_2\ <\ ...\ <\ x_N\ <\ =\ 10^{15} $
- $ 1\ <\ =\ s_i\ <\ =\ 10^9 $
- 入力値はすべて整数である。

### Sample Explanation 1

範囲 $ [L\ =\ 40,\ R\ =\ 70] $ に網を放つと西から $ 2, $ $ 3, $ $ 4 $ 匹目のけものを捕獲でき、$ s_2\ +\ s_3\ +\ s_4\ -\ (R\ -\ L)\ =\ 90 $ 円の利益が得られます。$ 91 $ 円以上の利益を得ることはできません。

### Sample Explanation 2

けものたちは入力例 1 と同じ位置にいますが、彼らの売値が大幅に下がっているため、二匹以上を狙うべきではありません。範囲 $ [L\ =\ 40,\ R\ =\ 40] $ に網を放つことで $ s_2\ -\ (R\ -\ L)\ =\ 5 $ 円の利益が得られ、これが最大です。

