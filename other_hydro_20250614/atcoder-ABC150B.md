## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc150/tasks/abc150_b

英大文字のみからなる長さ $ N $ の文字列 $ S $ があります。

$ S $ の連続する部分列 (入出力例をご覧ください) として `ABC` がいくつ含まれるかを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
$ S $ が連続する部分列として含む `ABC` の個数を出力せよ。

## 题目大意
**题意翻译**

输入一个长度为 $N$ 的字符串 $S$。

输出 $S$ 中包含多少个连续的 ABC。

```input1
10
ZABCDBABCQ
```

```output1
2
```

```input2
19
THREEONEFOURONEFIVE
```

```output2
0
```

```input3
33
ABCCABCBABCCABACBCBBABCBCBCBCABCB
```

```output3
5
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 50 $
- $ S $ は英大文字のみからなる。

### Sample Explanation 1

$ S $ の $ 2 $ 文字目から $ 4 $ 文字目、および $ 7 $ 文字目から $ 9 $ 文字目の $ 2 $ 箇所の連続する部分列が `ABC` に一致しています。

### Sample Explanation 2

$ S $ は `ABC` に一致する連続する部分列を含みません。

