# AT_arc119_a [ARC119A] 119 × 2^23 + 1

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc119/tasks/arc119_a

AtCoder ではたびたび、次のような形式の問題が出題されています。

> 答えを $ 998244353 $ で割った余りを求めよ。

ところで、実は $ 998244353\ =\ 119\ \times\ 2^{23}\ +\ 1 $ という性質があります。それに関連して、次の問いに答えてください。

> 整数 $ N $ が与えられる。  
>  $ N\ =\ a\ \times\ 2^b\ +\ c $ を満たす非負整数の組 $ (a,\ b,\ c) $ のうち、$ a\ +\ b\ +\ c $ が最小となるものにおける $ a\ +\ b\ +\ c $ の値を出力せよ。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $

## 输出格式

答えを出力してください。

## 输入输出样例 #1

### 输入 #1

```
998244353
```

### 输出 #1

```
143
```

## 输入输出样例 #2

### 输入 #2

```
1000000007
```

### 输出 #2

```
49483
```

## 输入输出样例 #3

### 输入 #3

```
1
```

### 输出 #3

```
1
```

## 输入输出样例 #4

### 输入 #4

```
998984374864432412
```

### 输出 #4

```
2003450165
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^{18} $
- $ N $ は整数

### Sample Explanation 1

$ 998244353\ =\ 119\ \times\ 2^{23}\ +\ 1 $ であるため、$ (a,\ b,\ c)\ =\ (119,\ 23,\ 1) $ のとき等式 $ N\ =\ a\ \times\ 2^{b}\ +\ c $ が成り立ちます。 そのときの $ a+b+c $ の値は $ 143 $ です。 $ a+b+c\ \leq\ 142 $ となるような組は存在しないため、$ 143 $ と出力すれば正解となります。

### Sample Explanation 2

$ 1000000007\ =\ 30517\ \times\ 2^{15}\ +\ 18951 $ であるため、$ (a,\ b,\ c)\ =\ (30517,\ 15,\ 18951) $ のとき等式 $ N\ =\ a\ \times\ 2^{b}\ +\ c $ が成り立ちます。 そのときの $ a+b+c $ の値は $ 49483 $ です。 $ a+b+c\ \leq\ 49482 $ となるような組は存在しないため、$ 49483 $ と出力すれば正解となります。

### Sample Explanation 3

$ 2^0\ =\ 1 $ であることに注意してください。