# AT_abc262_d [ABC262D] I Hate Non-integer Number

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc262/tasks/abc262_d

項数が $ N $ の正整数列 $ A=(a_1,\ldots,a_N) $ が与えられます。  
 $ A $ の項を $ 1 $ 個以上選ぶ方法は $ 2^N-1 $ 通りありますが、そのうち選んだ項の平均値が整数であるものが何通りかを $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ \ldots $ $ a_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 6 2
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
5
5 5 5 5 5
```

### 输出 #2

```
31
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ a_i\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

$ A $ の項を選ぶ方法それぞれに対する平均値は以下のようになります。 - $ a_1 $ のみを選んだ場合、平均値は $ \frac{a_1}{1}=\frac{2}{1}\ =\ 2 $ であり、整数である。 - $ a_2 $ のみを選んだ場合、平均値は $ \frac{a_2}{1}=\frac{6}{1}\ =\ 6 $ であり、整数である。 - $ a_3 $ のみを選んだ場合、平均値は $ \frac{a_3}{1}=\frac{2}{1}\ =\ 2 $ であり、整数である。 - $ a_1 $ と $ a_2 $ を選んだ場合、平均値は $ \frac{a_1+a_2}{2}=\frac{2+6}{2}\ =\ 4 $ であり、整数である。 - $ a_1 $ と $ a_3 $ を選んだ場合、平均値は $ \frac{a_1+a_3}{2}=\frac{2+2}{2}\ =\ 2 $ であり、整数である。 - $ a_2 $ と $ a_3 $ を選んだ場合、平均値は $ \frac{a_2+a_3}{2}=\frac{6+2}{2}\ =\ 4 $ であり、整数である。 - $ a_1 $ と $ a_2 $ と $ a_3 $ を選んだ場合、平均値は $ \frac{a_1+a_2+a_3}{3}=\frac{2+6+2}{3}\ =\ \frac{10}{3} $ であり、整数ではない。 以上より、$ 6 $ 通りの選び方が条件を満たします。

### Sample Explanation 2

どのように $ A $ の項を $ 1 $ 個以上選んでも平均値が $ 5 $ になります。