# AT_abc154_a [ABC154A] Remaining Balls

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc154/tasks/abc154_a

文字列 $ S $ の書かれたボールが $ A $ 個、文字列 $ T $ の書かれたボールが $ B $ 個あります。  
 高橋君は、文字列 $ U $ の書かれたボールを $ 1 $ 個選んで捨てました。  
 文字列 $ S,T $ の書かれたボールがそれぞれ何個残っているか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $ $ A $ $ B $ $ U $

## 输出格式

答えを空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
red blue
3 4
red
```

### 输出 #1

```
2 4
```

## 输入输出样例 #2

### 输入 #2

```
red blue
5 5
blue
```

### 输出 #2

```
5 4
```

## 说明/提示

### 制約

- $ S,T,U $ は英小文字のみからなる文字列
- $ S,T $ の長さは $ 1 $ 以上 $ 10 $ 以下
- $ S\ \not=\ T $
- $ S=U $ または $ T=U $
- $ 1\ \leq\ A,B\ \leq\ 10 $
- $ A,B $ は整数

### Sample Explanation 1

高橋君は `red` が書かれたボールを $ 1 $ つ選んで捨てました。 文字列 $ S,T $ が書かれたボールは、それぞれ $ 2,4 $ 個残っています。

### Sample Explanation 2

高橋君は `blue` が書かれたボールを $ 1 $ つ選んで捨てました。 文字列 $ S,T $ が書かれたボールは、それぞれ $ 5,4 $ 個残っています。