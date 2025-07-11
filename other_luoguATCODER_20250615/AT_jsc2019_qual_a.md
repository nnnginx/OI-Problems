# AT_jsc2019_qual_a Takahashi Calendar

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jsc2019-qual/tasks/jsc2019_qual_a

今日は $ 8 $ 月 $ 24 $ 日、年に $ 5 $ 日しかない積の日です。

$ d $ が $ 2 $ 桁の整数で、$ d $ の $ 1 $ の位を $ d_1 $、$ 10 $ の位を $ d_{10} $ としたときに $ m,\ d_1,\ d_{10} $ が次の条件をすべて満たす場合、$ m $ 月 $ d $ 日を積の日と呼びます。

- $ d_1\ \geq\ 2 $
- $ d_{10}\ \geq\ 2 $
- $ d_1\ \times\ d_{10}\ =\ m $

高橋くんはこの日をもっと増やしたいと考え、$ 1 $ 年が $ 1 $ 月から $ M $ 月までの合計 $ M $ ヶ月、どの月も $ 1 $ 日から $ D $ 日までの合計 $ D $ 日からなる高橋暦を誕生させました。

高橋暦において、積の日は年に何日あるでしょうか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ M $ $ D $

## 输出格式

高橋暦において積の日が $ 1 $ 年のうちに訪れる回数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
15 40
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
12 31
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
1 1
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ M\ \leq\ 100 $
- $ 1\ \leq\ D\ \leq\ 99 $

### Sample Explanation 1

年に訪れる積の日は次の $ 10 $ 日です。 - $ 4 $ 月 $ 22 $ 日 - $ 6 $ 月 $ 23 $ 日 - $ 6 $ 月 $ 32 $ 日 - $ 8 $ 月 $ 24 $ 日 - $ 9 $ 月 $ 33 $ 日 - $ 10 $ 月 $ 25 $ 日 - $ 12 $ 月 $ 26 $ 日 - $ 12 $ 月 $ 34 $ 日 - $ 14 $ 月 $ 27 $ 日 - $ 15 $ 月 $ 35 $ 日