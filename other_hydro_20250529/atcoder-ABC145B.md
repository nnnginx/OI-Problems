## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc145/tasks/abc145_b

正整数 $ N $ 及び、長さ $ N $ の英小文字から成る文字列 $ S $ が与えられます。

この文字列が、ある文字列を二度繰り返したものであるかを判定してください。 則ち、文字列 $ T $ であって、 $ S\ =\ T\ +\ T $ となるものが存在するかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
$ S $ が文字列を二度繰り返したものであるならば `Yes` と、そうでないならば `No` と出力せよ。

## 题目大意
给定长度为 $N$ 的字符串 $S$，问是否存在一个子串 $T$，使得 $S=T+T$。是则 `Yes`，否则 `No`。

Translated by @Expecting_Sharing(@_JYqwq_)

```input1
6
abcabc
```

```output1
Yes
```

```input2
6
abcadc
```

```output2
No
```

```input3
1
z
```

```output3
No
```

## 提示
### 制約

- $ 1\ <\ =\ N\ <\ =\ 100 $
- $ S $ は英小文字から成る
- $ |S|\ =\ N $

### Sample Explanation 1

$ T\ = $ `abc` とおくと、 $ S\ =\ T\ +\ T $ となります。

