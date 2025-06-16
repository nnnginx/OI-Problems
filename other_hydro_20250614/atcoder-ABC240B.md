## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc240/tasks/abc240_b

長さ $ N $ の正整数列 $ a\ =\ (a_1,\ a_2,\ \dots,\ a_N) $ には何種類の整数が現れますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ \ldots $ $ a_N $

## 输出格式
答えを出力せよ。

## 题目大意
给你一个正整数序列，求里面出现了几种正整数

```input1
6
1 4 1 2 2 1
```

```output1
3
```

```input2
1
1
```

```output2
1
```

```input3
11
3 1 4 1 5 9 2 6 5 3 5
```

```output3
7
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ a_i\ \leq\ 10^9\ \,\ (1\ \leq\ i\ \leq\ N) $
- 入力は全て整数

### Sample Explanation 1

$ 1,\ 2,\ 4 $ の $ 3 $ 種類の整数が現れます。

