# AT_abc203_a [ABC203A] Chinchirorin

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc203/tasks/abc203_a

高橋君が $ 3 $ つのサイコロを振ったところそれぞれ $ a,b,c $ の目が出ました。

$ a,b,c $ のうちある $ 2 $ つが同じときは残りの $ 1 $ つのサイコロの目を、同じものがないときは $ 0 $ を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ c $

## 输出格式

$ a,b,c $ のうちある $ 2 $ つが同じときは残りの $ 1 $ つのサイコロの目を、同じものがないときは $ 0 $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 5 2
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
4 5 6
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
1 1 1
```

### 输出 #3

```
1
```

## 说明/提示

### 制約

- $ 1\ \leq\ a,b,c\ \leq\ 6 $
- $ a,b,c $ は全て整数である。

### Sample Explanation 1

$ 1 $ つめと $ 3 $ つめのサイコロの目がともに $ 2 $ であるので、残り $ 1 $ つの目である $ 5 $ を出力します。

### Sample Explanation 2

サイコロの目はどの $ 2 $ つも相異なるため $ 0 $ を出力します。

### Sample Explanation 3

どの $ 2 $ つのサイコロの目も同じであり、そのいずれを選んだ場合でも残り $ 1 $ つの目は $ 1 $ となります。