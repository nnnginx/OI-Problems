# AT_code_formula_2014_final_b 3歩進んで2歩下がる

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-formula-2014-final/tasks/code_formula_2014_final_b

高橋君は、奇数日目に $ 3 $ 歩前に進み、偶数日目に $ 2 $ 歩後ろに下がります。

$ 1 $ 歩の距離は、前に進むときも、後ろに下がるときも、同じ距離です。

$ 1 $ 日目から $ n $ 日目の間に、高橋君が何歩分前に進んだかを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ n $

- $ 1 $ 行目には、日数を表す整数 $ n\ (1\ ≦\ n\ ≦\ 10^{15}) $ が与えられる。

## 输出格式

高橋君が何歩分前に進んだかを $ 1 $ 行で出力せよ。出力の末尾には改行をいれること。

## 输入输出样例 #1

### 输入 #1

```
6
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
999999999999999
```

### 输出 #2

```
500000000000002
```

## 说明/提示

### Sample Explanation 1

高橋君は、$ 1 $, $ 3 $, $ 5 $ 日目に $ 3 $ 歩進み、$ 2 $, $ 4 $, $ 6 $ 日目に $ 2 $ 歩戻ります。 よって、$ 3-2+3-2+3-2=3 $ 歩分、前に進みます。

### Sample Explanation 2

高橋君は、どれだけ長い期間でも、 $ 3 $ 歩進んで $ 2 $ 歩戻り続けます。