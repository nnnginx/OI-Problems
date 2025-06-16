# AT_soundhound2018_summer_qual_b Acrostic

## 题目描述

[problemUrl]: https://atcoder.jp/contests/soundhound2018-summer-qual/tasks/soundhound2018_summer_qual_b

小文字のアルファベットからなる文字列 $ S $ が与えられます。 この文字列を $ w $ 文字ごとに改行したときに、各行の先頭の文字を上から順番につなげて得られる文字列を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ w $

## 输出格式

答えの文字列を $ 1 $ 行に出力してください。

## 输入输出样例 #1

### 输入 #1

```
abcdefgh
3
```

### 输出 #1

```
adg
```

## 输入输出样例 #2

### 输入 #2

```
lllll
1
```

### 输出 #2

```
lllll
```

## 输入输出样例 #3

### 输入 #3

```
souuundhound
2
```

### 输出 #3

```
suudon
```

## 说明/提示

### 制約

- $ 1\leq\ w\leq\ |S|\ \leq\ 1000 $
- $ S $ は小文字のアルファベットのみからなる
- $ w $ は整数

### Sample Explanation 1

`abcdefgh` を $ 3 $ 文字ごとに改行すると、 abc def gh となります。これらの行の先頭の文字を上から順に読むと `adg` となります。