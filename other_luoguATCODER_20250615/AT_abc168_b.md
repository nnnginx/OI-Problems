# AT_abc168_b [ABC168B] ... (Triple Dots)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc168/tasks/abc168_b

英小文字からなる文字列 $ S $ があります。

$ S $ の長さが $ K $ 以下であれば、$ S $ をそのまま出力してください。

$ S $ の長さが $ K $ を上回っているならば、先頭 $ K $ 文字だけを切り出し、末尾に `...` を付加して出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $ $ S $

## 输出格式

問題文の通りに出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7
nikoandsolstice
```

### 输出 #1

```
nikoand...
```

## 输入输出样例 #2

### 输入 #2

```
40
ferelibenterhominesidquodvoluntcredunt
```

### 输出 #2

```
ferelibenterhominesidquodvoluntcredunt
```

## 说明/提示

### 制約

- $ K $ は $ 1 $ 以上 $ 100 $ 以下の整数
- $ S $ は英小文字からなる文字列
- $ S $ の長さは $ 1 $ 以上 $ 100 $ 以下

### Sample Explanation 1

`nikoandsolstice` の長さは $ 15 $ であり、$ K=7 $ を上回っています。 この先頭 $ 7 $ 文字を切り出して末尾に `...` を付加した文字列 `nikoand...` を出力します。

### Sample Explanation 2

ガイウス・ユリウス・カエサルの名言です。