## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_b

 **FizzBuzz列**  $ a_1,a_2,... $ を次のように定めます。

- $ i $ が $ 3 $ でも $ 5 $ でも割り切れるなら、$ a_i=\text{FizzBuzz} $
- そうではなく $ i $ が $ 3 $ で割り切れるなら、$ a_i=\text{Fizz} $
- そうではなく $ i $ が $ 5 $ で割り切れるなら、$ a_i=\text{Buzz} $
- そうではないなら、$ a_i=i $

FizzBuzz列の $ N $ 項目までに含まれる数の和を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
FizzBuzz列の $ N $ 項目までに含まれる数の和を出力せよ。

## 题目大意
求 $1$ 到 $n$ 这 $n$ 个数中既不是 $3$ 的倍数也不是 $5$ 的倍数的数之和，其中 $n$ 为正整数。

```input1
15
```

```output1
60
```

```input2
1000000
```

```output2
266666333332
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^6 $

### Sample Explanation 1

FizzBuzz列の $ 15 $ 項目までは次の通りです。 $ 1,2,\text{Fizz},4,\text{Buzz},\text{Fizz},7,8,\text{Fizz},\text{Buzz},11,\text{Fizz},13,14,\text{FizzBuzz} $ $ 15 $ 項目までには $ 1,2,4,7,8,11,13,14 $ が含まれ、これらの和は $ 60 $ です。

### Sample Explanation 2

オーバーフローに注意してください。

