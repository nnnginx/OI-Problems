## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc006/tasks/agc006_a

すぬけ君は次の条件を満たす文字列に興味があります。

- 長さ $ N $ 以上である。
- 先頭 $ N $ 文字が文字列 $ s $ に一致する。
- 末尾 $ N $ 文字が文字列 $ t $ に一致する。

条件を満たす文字列のうち、最も短いものの長さを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s $ $ t $

## 输出格式
条件を満たす文字列のうち、最も短いものの長さを出力せよ。

## 题目大意
给出长度为n的字符串s,t，求一个字符串满足：
* 长度至少为n
* 前缀为s
* 后缀为t

请找出长度最短的这样的字符串并输出他的长度

翻译提供者：WAAutoMaton

```input1
3
abc
cde
```

```output1
5
```

```input2
1
a
z
```

```output2
2
```

```input3
4
expr
expr
```

```output3
4
```

## 提示
### 制約

- $ 1\ <\ =N\ <\ =100 $
- $ s $, $ t $ は長さ $ N $ である。
- $ s $, $ t $ は英小文字のみからなる。

### Sample Explanation 1

最も短い文字列は `abcde` です。

### Sample Explanation 2

最も短い文字列は `az` です。

### Sample Explanation 3

最も短い文字列は `expr` です。

