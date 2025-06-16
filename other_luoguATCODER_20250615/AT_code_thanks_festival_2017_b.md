# AT_code_thanks_festival_2017_b Concatenated Palindrome

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-thanks-festival-2017/tasks/code_thanks_festival_2017_b

英小文字からなる文字列 $ S $ が与えられます。   
 $ S $ の後ろに英小文字からなる任意の文字列 $ T $ (空文字列も含む)を連結することで、回文にしたいです。   
 条件を満たす文字列 $ T $ のうち、$ T $ の最小の長さを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

条件を満たす文字列 $ T $ の最小の長さを求めよ。

## 输入输出样例 #1

### 输入 #1

```
abcde
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
level
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
codethanksfestival
```

### 输出 #3

```
17
```

## 输入输出样例 #4

### 输入 #4

```
abcdefghijklmnopqrstuvwxyzyxwvutsrqponmlkjihgfedcb
```

### 输出 #4

```
1
```

## 说明/提示

### 制約

- $ 1≦|S|≦50 $ ($ |S| $ は文字列 $ S $ の長さ)
- 文字列 $ S $ は英小文字から成る。

### Sample Explanation 1

$ T="dcba" $ とすると、文字列 $ S $ と 文字列 $ T $ を順番に連結した文字列は回文になります。 この文字列 $ T $ は条件を満たす中で最小の長さであるため、答えは $ 4 $ です。

### Sample Explanation 2

文字列 $ S $ は回文であるため、文字列 $ T $ は空文字列でも条件を満たします。 空文字列の長さは $ 0 $ であるため、答えは $ 0 $ です。