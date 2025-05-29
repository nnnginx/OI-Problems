## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc275/tasks/abc275_d

非負整数 $ x $ に対し定義される関数 $ f(x) $ は以下の条件を満たします。

- $ f(0)\ =\ 1 $
- 任意の正整数 $ k $ に対し $ f(k)\ =\ f(\lfloor\ \frac{k}{2}\rfloor)\ +\ f(\lfloor\ \frac{k}{3}\rfloor) $

ここで、$ \lfloor\ A\ \rfloor $ は $ A $ の小数点以下を切り捨てた値を指します。

このとき、 $ f(N) $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを出力せよ。

## 题目大意
## 题目描述

定义函数 $f(x)$ 有如下定义

- $ f(0)\ =\ 1 $
- 对于任意正整数 $k$ 有 $f(k)\ = f(\lfloor\ \frac{k}{2}\rfloor)\ +\ f(\lfloor\ \frac{k}{3}\rfloor) $

$ \lfloor\ A\ \rfloor $ 代表小于 $A$ 的最大整数。

求 $f(x)$。

## 输入格式

一个整数。

> $ N $

## 输出格式

一行，一个整数，代表 $f(N)$ 的值。

## 样例 #1

### 样例输入 #1

```
2
```

### 样例输出 #1

```
3
```

## 样例 #2

### 样例输入 #2

```
0
```

### 样例输出 #2

```
1
```

## 样例 #3

### 样例输入 #3

```
100
```

### 样例输出 #3

```
55
```

## 提示

### 数据范围

- $ 0\ \le\ N\ \le\ 10^{18} $

### 样例一解释

$ f(2)\ =\ f(\lfloor\ \frac{2}{2}\rfloor)\ +\ f(\lfloor\ \frac{2}{3}\rfloor)\ =\ f(1)\ +\ f(0)\ =(f(\lfloor\ \frac{1}{2}\rfloor)\ +\ f(\lfloor\ \frac{1}{3}\rfloor))\ +\ f(0)\ =(f(0)+f(0))\ +\ f(0)=\ 3 $。

```input1
2
```

```output1
3
```

```input2
0
```

```output2
1
```

```input3
100
```

```output3
55
```

## 提示
### 制約

- $ N $ は $ 0\ \le\ N\ \le\ 10^{18} $ を満たす整数

### Sample Explanation 1

$ f(2)\ =\ f(\lfloor\ \frac{2}{2}\rfloor)\ +\ f(\lfloor\ \frac{2}{3}\rfloor)\ =\ f(1)\ +\ f(0)\ =(f(\lfloor\ \frac{1}{2}\rfloor)\ +\ f(\lfloor\ \frac{1}{3}\rfloor))\ +\ f(0)\ =(f(0)+f(0))\ +\ f(0)=\ 3 $ です。

