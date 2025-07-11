# AT_abc357_d [ABC357D] 88888888

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc357/tasks/abc357_d

正整数 $ N $ に対して、$ N $ を $ N $ 個つなげた整数を $ V_N $ とします。  
 より厳密には、$ N $ を文字列とみなしたものを $ N $ 個連結し、 それを再度整数とみなしたものを $ V_N $ とします。  
 例えば、$ V_3=333 $, $ V_{10}=10101010101010101010 $ です。

$ V_N $ を $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

$ V_N $ を $ 998244353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
```

### 输出 #1

```
55555
```

## 输入输出样例 #2

### 输入 #2

```
9
```

### 输出 #2

```
1755646
```

## 输入输出样例 #3

### 输入 #3

```
10000000000
```

### 输出 #3

```
468086693
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 10^{18} $
- $ N $ は整数
 
### Sample Explanation 1

$ V_5=55555 $ を $ 998244353 $ で割った余りは $ 55555 $ です。

### Sample Explanation 2

$ V_9=999999999 $ を $ 998244353 $ で割った余りは $ 1755646 $ です。

### Sample Explanation 3

入力が $ 32 $ bit 整数型に収まらない可能性があることに注意してください。