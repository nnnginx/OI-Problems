## 题目描述
[problemUrl]: https://atcoder.jp/contests/diverta2019/tasks/diverta2019_a

すぬけ君は $ 1,2,\ldots,N $ の $ N $ 個の整数を持っています。 すぬけ君はこれらの整数から $ K $ 個の整数を選んで高橋君にあげようと考えています。

連続する $ K $ 個の整数を選ぶ方法は何通りありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
答えを出力せよ。

## 题目大意
Snuke 有 $N$ 个整数：$1,2,\ldots,N$。 他将选择其中的 $K$ 个数，然后将其交给 Takahashi。

有多少种方法可以选择 $K$ 个连续整数？

```input1
3 2
```

```output1
2
```

```input2
13 3
```

```output2
11
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ K\ \leq\ N\ \leq\ 50 $

### Sample Explanation 1

\- 連続する $ 2 $ 個の整数を選ぶ方法は $ (1,2) $ と $ (2,3) $ の $ 2 $ 通りです。

