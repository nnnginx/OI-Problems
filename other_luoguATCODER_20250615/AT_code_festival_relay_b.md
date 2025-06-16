# AT_code_festival_relay_b もう1年遊べるドン？

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2014-relay/tasks/code_festival_relay_b

amylase 伯爵さんは今年卒業を控えた大学生です。

   
今度行われる期末試験において $ s $ 点以上の点数を得ることができれば無事に卒業できますが、そうでなければ留年してしまいます。

   
さて、来たる期末試験当日、amylase 伯爵さんは $ a $ 点を獲得しました。数値の比較が苦手な amylase 伯爵さんに代わって、彼が卒業できるかどうか判定してください。

## 输入格式

入力は以下の形式で与えられる。

> $ a $ $ s $

- $ 1 $ 行目には、amylase 伯爵さんの試験の点数を表す整数 $ a $ ($ 0\ \leq\ a\ \leq\ 100 $) と、卒業のために必要な点数を表す整数 $ s $ ($ 0\ \leq\ s\ \leq\ 100 $) が与えられる。

## 输出格式

amylase 伯爵さんが卒業できるなら `Congratulations!` を、そうでなければ `Enjoy another semester...` を、$ 1 $ 行で出力せよ。

最後は改行し、余計な文字、空行を含まないこと。

## 输入输出样例 #1

### 输入 #1

```
100 40
```

### 输出 #1

```
Congratulations!
```

## 输入输出样例 #2

### 输入 #2

```
0 100
```

### 输出 #2

```
Enjoy another semester...
```

## 输入输出样例 #3

### 输入 #3

```
60 60
```

### 输出 #3

```
Congratulations!
```

## 说明/提示

### Sample Explanation 1

amylase 伯爵さんの期末試験の点数が $ 100 $ 点、卒業に必要な点数が $ 40 $ 点なので、卒業することができます。

### Sample Explanation 2

amylase 伯爵さんの期末試験の点数が $ 0 $ 点、卒業に必要な点数が $ 100 $ 点なので、卒業することができません。