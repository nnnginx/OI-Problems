# AT_abc154_e [ABC154E] Almost Everywhere Zero

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc154/tasks/abc154_e

$ 1 $ 以上 $ N $ 以下の整数であって、 $ 10 $ 進法で表したときに、$ 0 $ でない数字がちょうど $ K $ 個あるようなものの個数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式

条件を満たす数の個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
100
1
```

### 输出 #1

```
19
```

## 输入输出样例 #2

### 输入 #2

```
25
2
```

### 输出 #2

```
14
```

## 输入输出样例 #3

### 输入 #3

```
314159
2
```

### 输出 #3

```
937
```

## 输入输出样例 #4

### 输入 #4

```
9999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
3
```

### 输出 #4

```
117879300
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ <\ 10^{100} $
- $ 1\ \leq\ K\ \leq\ 3 $

### Sample Explanation 1

条件を満たす数は次の $ 19 $ 個です。 - $ 1,2,3,4,5,6,7,8,9,10,20,30,40,50,60,70,80,90,100 $

### Sample Explanation 2

条件を満たす数は次の $ 14 $ 個です。 - $ 11,12,13,14,15,16,17,18,19,21,22,23,24,25 $