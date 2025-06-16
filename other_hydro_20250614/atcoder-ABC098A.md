## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc098/tasks/abc098_a

$ 2 $ つの整数 $ A $, $ B $ が与えられます。 $ A+B $, $ A-B $, $ A\ \times\ B $ の中で最大の値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
$ A+B $, $ A-B $, $ A\ \times\ B $ の中で最大の値を出力せよ。

## 题目大意
给你 $2$ 个正整数 $a$ 和 $b$，请你求出 $a+b$ ， $a-b$ 和 $a\times b$ 的最大值。

```input1
3 1
```

```output1
4
```

```input2
4 -2
```

```output2
6
```

```input3
0 0
```

```output3
0
```

## 提示
### 制約

- $ -1000\ \leq\ A,B\ \leq\ 1000 $
- 入力はすべて整数である

### Sample Explanation 1

$ 3+1=4 $, $ 3-1=2 $, $ 3\ \times\ 1=3 $ なので、この中で最大の値である $ 4 $ が答えになります。

### Sample Explanation 2

$ 4\ -\ (-2)\ =\ 6 $ が最大の値になります。

