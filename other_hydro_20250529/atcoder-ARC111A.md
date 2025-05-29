## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc111/tasks/arc111_a

正整数 $ N,\ M $ が与えられます。$ \lfloor\ \frac{10^N}{M}\ \rfloor $ を $ M $ で割った余りを求めてください。

  $ \lfloor\ x\ \rfloor $ について $ \lfloor\ x\ \rfloor $ は、 $ x $ を超えない最大の整数を表します。例としては次のようになります。 - $ \lfloor\ 2.5\ \rfloor\ =\ 2 $
- $ \lfloor\ 3\ \rfloor\ =\ 3 $
- $ \lfloor\ 9.9999999\ \rfloor\ =\ 9 $
- $ \lfloor\ \frac{100}{3}\ \rfloor\ =\ \lfloor\ 33.33...\ \rfloor\ =\ 33 $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
答えを出力せよ。

## 题目大意
给定两个数 $n$ 和 $m$。

输出 $\left\lfloor\frac{10^n}{m}\right\rfloor \bmod m$ 的值。

$n \le 10^{18},m \le 10^4$。

```input1
1 2
```

```output1
1
```

```input2
2 7
```

```output2
0
```

```input3
1000000000000000000 9997
```

```output3
9015
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^{18} $
- $ 1\ \leq\ M\ \leq\ 10000 $

### Sample Explanation 1

$ \lfloor\ \frac{10^1}{2}\ \rfloor\ =\ 5 $ なので、$ 5 $ を $ 2 $ で割った余りの $ 1 $ を出力します。

