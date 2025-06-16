## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc059/tasks/abc059_a

英小文字からなる $ 3 $ つの単語 $ s_1 $, $ s_2 $, $ s_3 $ が空白区切りで与えられるので、単語の先頭の文字をつなげ、大文字にした略語を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s_1 $ $ s_2 $ $ s_3 $

## 输出格式
答えを出力せよ。

## 题目大意
输入三个由小写英文字母组成的字符串，以大写字母的方式输出它们的首字母。

```input1
atcoder beginner contest
```

```output1
ABC
```

```input2
resident register number
```

```output2
RRN
```

```input3
k nearest neighbor
```

```output3
KNN
```

```input4
async layered coding
```

```output4
ALC
```

## 提示
### 制約

- $ s_1 $, $ s_2 $, $ s_3 $ は英小文字からなる。
- $ 1\ ≦|s_i|≦\ 10\ (1≦i≦3) $

### Sample Explanation 1

`atcoder` `beginner` `contest` の先頭の文字はそれぞれ`a` `b` `c`なので、`ABC`が答えになります。

