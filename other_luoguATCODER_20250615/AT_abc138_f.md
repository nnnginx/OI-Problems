# AT_abc138_f [ABC138F] Coincidence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc138/tasks/abc138_f

整数 $ L,\ R $ が与えられます。整数の組 $ (x,\ y) $ $ (L\ \leq\ x\ \leq\ y\ \leq\ R) $ であって、$ y $ を $ x $ で割った余りが $ y\ \text{\ XOR\ }\ x $ に等しいものの個数を $ 10^9\ +\ 7 $ で割ったあまりを求めてください。

 $ \text{\ XOR\ } $ とは 整数 $ A,\ B $ のビットごとの排他的論理和 $ a\ \text{\ XOR\ }\ b $ は、以下のように定義されます。

- $ a\ \text{\ XOR\ }\ b $ を二進数表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ A,\ B $ を二進数表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。
 
 例えば、$ 3\ \text{\ XOR\ }\ 5\ =\ 6 $ となります (二進数表記すると: $ 011\ \text{\ XOR\ }\ 101\ =\ 110 $)。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ L $ $ R $

## 输出格式

条件を満たす整数の組 $ (x,\ y) $ $ (L\ \leq\ x\ \leq\ y\ \leq\ R) $ の個数を $ 10^9\ +\ 7 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
10 100
```

### 输出 #2

```
604
```

## 输入输出样例 #3

### 输入 #3

```
1 1000000000000000000
```

### 输出 #3

```
68038601
```

## 说明/提示

### 制約

- $ 1\ \leq\ L\ \leq\ R\ \leq\ 10^{18} $

### Sample Explanation 1

条件を満たす組は $ (2,\ 2),\ (2,\ 3),\ (3,\ 3) $ の $ 3 $ 通りです。

### Sample Explanation 3

個数を $ 10^9\ +\ 7 $ で割ったあまりを計算することを忘れないでください。