# AT_arc100_d [ARC100F] Colorful Sequences

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc100/tasks/arc100_d

整数 $ N $ と $ K $、そして長さ $ M $ の整数列 $ A $ が与えられます。

各要素が $ 1 $ 以上 $ K $ 以下の整数である整数列がカラフルであるとは、 その整数列の長さ $ K $ の連続する部分列であって、$ 1 $ から $ K $ までの整数を $ 1 $ 個ずつ含むものが存在することを意味します。

すべての長さ $ N $ のカラフルな整数列について、その連続する部分列であって $ A $ に一致するものの個数を数えて、その総和を求めてください。 ただし、答えは非常に大きくなることがあるので、$ 10^9+7 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ M $ $ A_1 $ $ A_2 $ $ ... $ $ A_M $

## 输出格式

すべての長さ $ N $ のカラフルな整数列について、その連続する部分列であって $ A $ に一致するものの個数を数えて、 その総和を $ 10^9+7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2 1
1
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
4 2 2
1 2
```

### 输出 #2

```
12
```

## 输入输出样例 #3

### 输入 #3

```
7 4 5
1 2 3 1 2
```

### 输出 #3

```
17
```

## 输入输出样例 #4

### 输入 #4

```
5 4 3
1 1 1
```

### 输出 #4

```
0
```

## 输入输出样例 #5

### 输入 #5

```
10 3 5
1 1 2 3 3
```

### 输出 #5

```
1458
```

## 输入输出样例 #6

### 输入 #6

```
25000 400 4
3 7 31 127
```

### 输出 #6

```
923966268
```

## 输入输出样例 #7

### 输入 #7

```
9954 310 12
267 193 278 294 6 63 86 166 157 193 168 43
```

### 输出 #7

```
979180369
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 25000 $
- $ 1\ \leq\ K\ \leq\ 400 $
- $ 1\ \leq\ M\ \leq\ N $
- $ 1\ \leq\ A_i\ \leq\ K $
- 入力はすべて整数である。

### Sample Explanation 1

長さ $ 3 $ のカラフルな整数列は、$ (1,1,2) $, $ (1,2,1) $, $ (1,2,2) $, $ (2,1,1) $, $ (2,1,2) $, $ (2,2,1) $ の $ 6 $ 個です。 これらの整数列の、連続する部分列であって $ A=(1) $ に一致するものの個数は、それぞれ $ 2 $, $ 2 $, $ 1 $, $ 2 $, $ 1 $, $ 1 $ 個です。 よって、これらの合計である $ 9 $ が答えになります。