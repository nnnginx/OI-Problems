# AT_abc110_c [ABC110C] String Transformation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc110/tasks/abc110_c

英小文字のみからなる文字列 $ S $, $ T $ が与えられます。

文字列 $ S $ に対して、次の操作を何度でも行うことができます。

操作: 2つの異なる英小文字 $ c_1 $, $ c_2 $ を選び、$ S $ に含まれる全ての $ c_1 $ を $ c_2 $ に、$ c_2 $ を $ c_1 $ に置き換える

$ 0 $ 回以上操作を行って、$ S $ を $ T $ に一致させられるか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式

$ S $ を $ T $ に一致させられる場合は `Yes`、そうでない場合は `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
azzel
apple
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
chokudai
redcoder
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
abcdefghijklmnopqrstuvwxyz
ibyhqfrekavclxjstdwgpzmonu
```

### 输出 #3

```
Yes
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 2\ \times\ 10^5 $
- $ |S|\ =\ |T| $
- $ S $, $ T $ は英小文字のみからなる

### Sample Explanation 1

次のように操作を行えば、`azzel` を `apple` にできます。 - $ c_1 $ として `e` を、$ c_2 $ として `l` を選ぶと、`azzel` が `azzle` になる - $ c_1 $ として `z` を、$ c_2 $ として `p` を選ぶと、`azzle` が `apple` になる

### Sample Explanation 2

どのように操作を行っても `chokudai` を `redcoder` にできません。