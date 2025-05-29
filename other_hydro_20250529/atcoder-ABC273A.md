## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc273/tasks/abc273_a

非負整数 $ x $ に対し定義される関数 $ f(x) $ は以下の条件を満たします。

- $ f(0)\ =\ 1 $
- 任意の正整数 $ k $ に対し $ f(k)\ =\ k\ \times\ f(k-1) $

このとき、 $ f(N) $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを整数として出力せよ。

## 题目大意
求 $n$ 的阶乘。$0\le n\le 10$。

特别的：$0$ 的阶乘为 $1$。

```input1
2
```

```output1
2
```

```input2
3
```

```output2
6
```

```input3
0
```

```output3
1
```

```input4
10
```

```output4
3628800
```

## 提示
### 制約

- $ N $ は $ 0\ \le\ N\ \le\ 10 $ を満たす整数

### Sample Explanation 1

$ f(2)\ =\ 2\ \times\ f(1)\ =\ 2\ \times\ 1\ \times\ f(0)\ =\ 2\ \times\ 1\ \times\ 1\ =\ 2 $ です。

### Sample Explanation 2

$ f(3)\ =\ 3\ \times\ f(2)\ =\ 3\ \times\ 2\ =\ 6 $ です。

