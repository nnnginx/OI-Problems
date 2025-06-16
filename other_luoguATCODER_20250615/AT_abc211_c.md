# AT_abc211_c [ABC211C] chokudai

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc211/tasks/abc211_c

文字列 $ S $ が与えられます。  
 このうち $ 8 $ 文字を選び下線を引き、下線を引いた文字が左から順に `c` , `h` , `o` , `k` , `u` , `d` , `a` , `i` となるようにする方法は何通りありますか？  
 ただし答えは非常に大きくなる可能性があるので、$ (10^9\ +\ 7) $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

答えを $ (10^9\ +\ 7) $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
chchokudai
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
atcoderrr
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
chokudaichokudaichokudai
```

### 输出 #3

```
45
```

## 说明/提示

### 制約

- $ 8\ \leq\ |S|\ \leq\ 10^5 $
- $ S $ は英小文字からなる

### Sample Explanation 1

chchokudai chchokudai chchokudai 上の $ 3 $ つが条件を満たします。 chchokudai は、条件を満たさないことに注意してください。

### Sample Explanation 2

答えが $ 0 $ 通りになることもあります。