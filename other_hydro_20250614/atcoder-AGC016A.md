## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc016/tasks/agc016_a

すぬけ君は、次のルールに従い、長さ $ N $ の文字列 $ t $ を長さ $ N\ -\ 1 $ の文字列 $ t' $ へ変えることができます。

- 各 $ i $ ($ 1\ <\ =\ i\ <\ =\ N\ -\ 1 $) について、$ t' $ の $ i $ 文字目は $ t $ の $ i $, $ i\ +\ 1 $ 文字目のどちらかである。

英小文字のみからなる文字列 $ s $ があります。 すぬけ君の目標は、$ s $ に上記の操作を繰り返し行い、$ s $ が単一の文字のみからなるようにすることです。 目標を達成するために必要な操作回数の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
目標を達成するために必要な操作回数の最小値を出力せよ。

## 题目大意
给出一个字符串，每次操作可以使得字符串缩短一位，新的字符串的第i位可以是原字符串的第i或者第i+1位。
问使得整个字符串全相同最少的操作次数

```input1
serval
```

```output1
3
```

```input2
jackal
```

```output2
2
```

```input3
zzz
```

```output3
0
```

```input4
whbrjpjyhsrywlqjxdbrbaomnw
```

```output4
8
```

## 提示
### 制約

- $ 1\ <\ =\ |s|\ <\ =\ 100 $
- $ s $ は英小文字のみからなる。

### Sample Explanation 1

例えば、`serval` → `srvvl` → `svvv` → `vvv` と変えればよいです。

### Sample Explanation 2

例えば、`jackal` → `aacaa` → `aaaa` と変えればよいです。

### Sample Explanation 3

最初から $ s $ が単一の文字のみからなっています。

### Sample Explanation 4

$ 8 $ 回の操作によって、$ s $ を `rrrrrrrrrrrrrrrrrr` へ変えることができます。

