# AT_abc210_c [ABC210C] Colorful Candies

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc210/tasks/abc210_c

$ N $ 個のキャンディが左右一列に並んでいます。  
 それぞれのキャンディは、色 $ 1 $、色 $ 2 $、$ \ldots $、色 $ 10^9 $の、$ 10^9 $ 種類の色のうちいずれかの色をしています。  
 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、左から $ i $ 番目のキャンディの色は色 $ c_i $ です。

高橋君は並んでいるキャンディのうち、連続して並んだ $ K $ 個のキャンディをもらうことができます。  
 すなわち、$ 1\ \leq\ i\ \leq\ N-K+1 $ を満たす整数 $ i $ を選んで、 左から $ i $ 番目、$ i+1 $ 番目、$ i+2 $ 番目、$ \ldots $、$ i+K-1 $ 番目のキャンディをもらうことができます。

高橋君はいろいろな色のキャンディを食べたいので、 もらうキャンディに含まれる色の種類数が多いほどうれしい気持ちになります。  
 高橋君がもらうキャンディに含まれる色の種類数の最大値を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ c_1 $ $ c_2 $ $ \ldots $ $ c_N $

## 输出格式

高橋君がもらうキャンディに含まれる色の種類数の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7 3
1 2 1 2 3 3 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5 5
4 4 4 4 4
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
10 6
304621362 506696497 304621362 506696497 834022578 304621362 414720753 304621362 304621362 414720753
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 3\ \times\ 10^5 $
- $ 1\ \leq\ c_i\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

高橋君が左から $ 3 $ 番目から $ 5 $ 番目のキャンディをもらうと、もらうキャンディに含まれる色は $ 3 $ 種類になり、これが最大です。

### Sample Explanation 2

高橋君は並んでいるすべてのキャンディをもらうことが出来ますが、もらうキャンディに含まれる色は $ 1 $ 種類です。