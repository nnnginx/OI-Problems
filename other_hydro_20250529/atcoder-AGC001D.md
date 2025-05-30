## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc001/tasks/agc001_d

高橋君のお母さんは、高橋君の誕生日に数列 $ a,\ b $ をプレゼントしました。 数列 $ a,\ b $ は以下の性質をすべて満たしていたため、高橋君はとても喜びました。

- 数列 $ a $ に含まれる数の総和は $ N $ である。
- 数列 $ b $ に含まれる数の総和は $ N $ である。
- 数列 $ a,\ b $ に含まれる数はすべて正の整数である。
- 以下の条件を $ 2 $ つとも満たす長さ $ N $ の文字列は、必ずすべての文字が同じである。
  - 先頭の $ a_1 $ 文字、続く $ a_2 $ 文字、さらに続く $ a_3 $ 文字 ... はすべて回文である。
  - 先頭の $ b_1 $ 文字、続く $ b_2 $ 文字、さらに続く $ b_3 $ 文字 ... はすべて回文である。

しかしある日、高橋君は数列 $ a,\ b $ を両方ともなくしてしまいました。 幸運なことに、高橋君は数列 $ a $ が長さ $ M $ の数列 $ A $ の並び替えであったことを覚えています。

高橋君のお母さんは高橋君を喜ばせるために、数列 $ a,\ b $ として考えられるものを高橋君にもう一度プレゼントしようと考えました。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ ... $ $ A_M $

## 输出格式
数列 $ a,\ b $ として考えられるものがある場合、数列 $ a $、数列 $ b $ の長さ、数列 $ b $ を順に出力せよ。 ただし、高橋君の勘違いなどの理由で数列 $ a,\ b $ として考えられるものが存在しない場合がある。その場合は代わりに `Impossible` と出力せよ。

## 题目大意
### 题目描述

高桥くん的母亲在高桥生日的时候送了他 $a, b$ 两个数列。因为 $a, b$ 满足了如下的所有性质， 所以他非常高兴：

* $a$ 数列的数字总和是 $N$；
* $b$ 数列的数字总和是 $N$；
* $a, b$ 中包含的数都是正整数； 
* 满足以下两个条件的数列， 所有元素必定是相同的。
  * 最开始的 $a_1$ 个元素, 接下来的 $a_2$ 个元素，更后面的 $a_3$ 个，等等，都是回文；
  * 最开始的 $b_1$ 个元素, 接下来的 $b_2$ 个元素，更后面的 $b_3$ 个，等等，都是回文。

但是有一天，高桥把把数列 $a$ 和 $b$ 都弄丢了， 幸运的是，他知道数列 $a$ 是另一个长度为 $M$ 的序列 $A$ 的排列。

为了让他再一次高兴起来， 他妈妈决定给他另一对数列使其满足如上性质。


### 数据范围

- $1≤N≤10^5$；
- $1≤M≤100$；
- $1≤A_i≤10^5$。

数据保证 $A_i$ 的和是 $N$。

### 输入输出格式：

>**输入格式**
>
>第一行两个整数 $N, M$。
>
>之后一行，第 $i$ 个整数是 $A_i$。
>
>**输出格式**
>
>如果存在解， 输出三行，第一行数列 $a$，第二行 $b$ 的长度，第三行数列 $b$。
>
>否则输出 `Impossible`（大小写敏感！）。

感谢 @ToBiChi 提供翻译。

```input1
3 2
2 1
```

```output1
1 2
1
3
```

```input2
6 1
6
```

```output2
6
3
1 2 3
```

```input3
55 10
1 2 3 4 5 6 7 8 9 10
```

```output3
Impossible
```

## 提示
### 制約

- $ 1≦N≦10^5 $
- $ 1≦M≦100 $
- $ 1≦A_i≦10^5 $
- $ A_i $ の総和は $ N $ である。

