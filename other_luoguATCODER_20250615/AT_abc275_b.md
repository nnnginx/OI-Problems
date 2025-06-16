# AT_abc275_b [ABC275B] ABC-DEF

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc275/tasks/abc275_b

非負整数 $ A,B,C,D,E,F $ があり、$ A\times\ B\times\ C\geq\ D\times\ E\times\ F $ をみたしています。  
 $ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ の値を $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $ $ E $ $ F $

## 输出格式

$ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ を $ 998244353 $ で割った余りを整数で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3 5 1 2 4
```

### 输出 #1

```
22
```

## 输入输出样例 #2

### 输入 #2

```
1 1 1000000000 0 0 0
```

### 输出 #2

```
1755647
```

## 输入输出样例 #3

### 输入 #3

```
1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 0\leq\ A,B,C,D,E,F\leq\ 10^{18} $
- $ A\times\ B\times\ C\geq\ D\times\ E\times\ F $
- $ A,B,C,D,E,F $ は整数

### Sample Explanation 1

$ A\times\ B\times\ C=2\times\ 3\times\ 5=30 $, $ D\times\ E\times\ F=1\times\ 2\times\ 4=8 $ より、 $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=22 $ であり、これを $ 998244353 $ で割った余りである $ 22 $ を出力します。

### Sample Explanation 2

$ A\times\ B\times\ C=1000000000 $, $ D\times\ E\times\ F=0 $ より、 $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=1000000000 $ であり、これを $ 998244353 $ で割った余りである $ 1755647 $ を出力します。

### Sample Explanation 3

$ (A\times\ B\times\ C)-(D\times\ E\times\ F)=0 $ であり、これを $ 998244353 $ で割った余りである $ 0 $ を出力します。