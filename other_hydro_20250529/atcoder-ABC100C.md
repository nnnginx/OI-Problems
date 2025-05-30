## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc100/tasks/abc100_c

AtCoder Beginner Contest 100 の開催にともなって, AtCoder 社では長さ $ N $ の数列 $ a\ = ${$ a_1,\ a_2,\ a_3,\ ...,\ a_N $} が飾られることになった.   
 社員のすぬけ君は, この数列で遊んでみようと思った.

具体的には, 以下の操作をできるだけ多くの回数繰り返そうと思った.

> $ 1\ \leq\ i\ \leq\ N $ を満たす全ての $ i $ に対して, それぞれ「$ a_i $ の値を $ 2 $ で割る」「$ a_i $ の値を $ 3 $ 倍する」のどちらかを行う. ただし, 全ての $ i $ に対して $ 3 $ 倍することはできず, 操作後の $ a_i $ の値は整数でなければならない.

最大で何回の操作が可能か, 求めなさい.

## 输入格式
入力は以下の形式で標準入力から与えられる.

> $ N $ $ a_1 $ $ a_2 $ $ a_3 $ $ ... $ $ a_N $

## 输出格式
すぬけ君が行える最大の操作回数を出力しなさい.

## 题目大意
给定一个长度为 $n$ 的数列 $a$，你可以对它进行以下操作：

对于所有使得 $1\le i\le n$ 的 $i$，将 $a_i$ 乘以 $3$，或者除以 $2$。

注意：

* 如果 $a_i$ 是奇数，那么 $a_i$ 就不能除以 $2$。

* 两种操作都必须使用。

最后输出能操作的次数的最大值。

```input1
3
5 2 4
```

```output1
3
```

```input2
4
631 577 243 199
```

```output2
0
```

```input3
10
2184 2126 1721 1800 1024 2528 3360 1945 1280 1776
```

```output3
39
```

## 提示
### 制約

- $ N $ は $ 1 $ 以上 $ 10\ 000 $ 以下の整数
- $ a_i $ は $ 1 $ 以上 $ 1\ 000\ 000\ 000 $ 以下の整数

### Sample Explanation 1

最初, 数列は $ {5,\ 2,\ 4} $ であるが, 以下のように操作すれば $ 3 $ 回の操作を行うことができる. - 最初に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 3 $ 倍し, $ a_3 $ を $ 2 $ で割る. すると数列は $ {15,\ 6,\ 2} $ となる. - 次に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 2 $ で割り, $ a_3 $ を $ 3 $ 倍する. すると数列は $ {45,\ 3,\ 6} $ となる. - 最後に, $ a_1 $ を $ 3 $ 倍し, $ a_2 $ を $ 3 $ 倍し, $ a_3 $ を $ 2 $ で割る. すると数列は $ {135,\ 9,\ 3} $ となる.

### Sample Explanation 2

全ての要素が奇数なので, 操作はできない. よって答えは $ 0 $ である.

