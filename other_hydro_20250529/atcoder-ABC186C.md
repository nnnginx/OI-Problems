## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc186/tasks/abc186_c

高橋君は $ 7 $ が嫌いです。

$ 1 $ 以上 $ N $ 以下の整数のうち、$ 10 $ 進法で表しても $ 8 $ 進法で表しても $ 7 $ を含まないような数はいくつありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを整数で出力せよ。

## 题目大意
给定一个正整数 $n$，求出 $1$ 至 $n$ 中有多少个数满足：该数在十进制下和八进制表示下均不含 $7$。

$1 \leq n \leq 10^5$。

```input1
20
```

```output1
17
```

```input2
100000
```

```output2
30555
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ N $ は整数である。

### Sample Explanation 1

$ 1 $ 以上 $ 20 $ 以下の整数のうち、$ 10 $ 進法で表したときに $ 7 $ を含む数は $ 7,17 $、$ 8 $ 進法で表したときに $ 7 $ を含む数は $ 7,15 $ です。 よって、$ 7,15,17 $ 以外の $ 17 $ 個の数が条件を満たします。

