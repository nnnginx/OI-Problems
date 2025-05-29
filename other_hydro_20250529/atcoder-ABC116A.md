## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc116/tasks/abc116_a

直角三角形 $ ABC $ があります。$ ∠ABC=90° $ です。

三角形 $ ABC $ の三辺の長さである $ |AB|,|BC|,|CA| $ が与えられるので、直角三角形 $ ABC $ の面積を求めて下さい。

ただし、三角形 $ ABC $ の面積は整数となることが保証されています。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ |AB| $ $ |BC| $ $ |CA| $

## 输出格式
三角形 $ ABC $ の面積を出力してください。

## 题目大意
给定一个 $∠ ABC = 90 °$ 的直角三角形的三条边，输出这个三角形的面积。保证答案为整数。

Translated by ShanCreeper.

```input1
3 4 5
```

```output1
6
```

```input2
5 12 13
```

```output2
30
```

```input3
45 28 53
```

```output3
630
```

## 提示
### 制約

- $ 1\ \leqq\ |AB|,|BC|,|CA|\ \leqq\ 100 $
- 入力はすべて整数である。
- 三角形 $ ABC $ の面積は整数である。

### Sample Explanation 1

!\[tri\](https://img.atcoder.jp/ghi/44c1d4cbdf4677ce3b08ca70b5ce98ea.png) この三角形の面積は $ 6 $ です。

### Sample Explanation 2

この三角形の面積は $ 30 $ です。

### Sample Explanation 3

この三角形の面積は $ 630 $ です。

