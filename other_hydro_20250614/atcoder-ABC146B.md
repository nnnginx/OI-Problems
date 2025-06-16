## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc146/tasks/abc146_b

英大文字のみからなる文字列 $ S $ があります。また、整数 $ N $ が与えられます。

$ S $ の各文字を、アルファベット順で $ N $ 個後の文字に置き換えた文字列を出力してください。

ただしアルファベット順で `Z` の $ 1 $ 個後の文字は `A` とみなします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
$ S $ の各文字を、アルファベット順で $ N $ 個後の文字に置き換えた文字列を出力せよ。

## 题目大意
输入一个整数 $N$ ，和一个仅包含大写字母的字符串 $S$ 。

将字符串 $S$ 中的每个字母替换为字母顺序中的向后第 $N$ 个字母。

注意：Z后第一个字母记作A。

输出该字符串。

```input1
2
ABCXYZ
```

```output1
CDEZAB
```

```input2
0
ABCXYZ
```

```output2
ABCXYZ
```

```input3
13
ABCDEFGHIJKLMNOPQRSTUVWXYZ
```

```output3
NOPQRSTUVWXYZABCDEFGHIJKLM
```

## 提示
### 制約

- $ 0\ \leq\ N\ \leq\ 26 $
- $ 1\ \leq\ |S|\ \leq\ 10^4 $
- $ S $ は英大文字のみからなる

### Sample Explanation 1

アルファベット順で `Z` の $ 1 $ 個後の文字は `A` であることに注意してください。

