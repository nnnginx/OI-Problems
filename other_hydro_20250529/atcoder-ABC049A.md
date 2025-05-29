## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc049/tasks/abc049_a

英小文字 $ c $ が与えられるので、$ c $ が母音であるか判定してください。ここで、英小文字のうち母音は `a`、`e`、`i`、`o`、`u`の $ 5 $ つです。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ c $

## 输出格式
$ c $ が母音であるとき、`vowel` と、そうでないとき `consonant` と出力せよ。

## 题目大意
输入一个字符，输出TA是不是元音，如果是，输出$vowel$。如果不是，输出$consonant$. （元音指$a$,$e$,$i$,$o$,$u$)  


```input1
a
```

```output1
vowel
```

```input2
z
```

```output2
consonant
```

```input3
s
```

```output3
consonant
```

## 提示
### 制約

- $ c $ は英小文字である。

### Sample Explanation 1

`a` は母音なので、`vowel` と出力します。

