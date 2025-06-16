# AT_soundhound2018_summer_qual_a F

## 题目描述

[problemUrl]: https://atcoder.jp/contests/soundhound2018-summer-qual/tasks/soundhound2018_summer_qual_a

$ 2 $ つの 整数 $ a,b $ が与えられます。 $ a+b=15 $ であるか、$ a\times\ b=15 $ であるか、そのどちらでもないかを判定してください。

ただし、$ a+b=15 $ と $ a\times\ b=15 $ が同時に成り立つことはありません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $

## 输出格式

$ a+b=15 $ であれば `+` を、 $ a\times\ b=15 $ であれば `*` を、 どちらでもなければ `x` を出力してください。

## 输入输出样例 #1

### 输入 #1

```
4 11
```

### 输出 #1

```
+
```

## 输入输出样例 #2

### 输入 #2

```
3 5
```

### 输出 #2

```
*
```

## 输入输出样例 #3

### 输入 #3

```
1 1
```

### 输出 #3

```
x
```

## 说明/提示

### 制約

- $ 1\ \leq\ a,b\ \leq\ 15 $
- 入力はすべて整数

### Sample Explanation 1

$ 4+11=15 $ です。

### Sample Explanation 2

$ 3\times\ 5=15 $ です。

### Sample Explanation 3

$ 1+1=2 $ であり、 $ 1\times\ 1=1 $であるため、どちらも $ 15 $ ではありません。