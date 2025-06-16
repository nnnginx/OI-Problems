# AT_code_thanks_festival_2018_d Concatenation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-thanks-festival-2018/tasks/code_thanks_festival_2018_d

英小文字から成る文字列 $ S $ が与えられます。

これは `code` のように、先頭の文字がその文字列においてアルファベット順で最小となる文字列を1つ以上連結してできたものです。

元となるそれぞれの文字列には、先頭と同じ文字が複数含まれていたことはありません。

$ S $ は最小で何個の文字列を繋げてできた可能性があるでしょうか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

連結して $ S $ になるような題意の文字列の個数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
codethanksfes
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
atcoder
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
aaa
```

### 输出 #3

```
3
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^5 $
- $ S $ は英小文字から成る

### Sample Explanation 1

例えば `codeth` と `anksfes` を連結するとできます。

### Sample Explanation 2

`atcoder` は条件を満たします。