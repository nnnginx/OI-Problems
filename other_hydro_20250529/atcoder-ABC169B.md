## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc169/tasks/abc169_b

$ N $ 個の整数 $ A_1,...,A_N $ が与えられます。

$ A_1\ \times\ ...\ \times\ A_N $ を求めてください。

ただし、結果が $ 10^{18} $ を超える場合は、代わりに `-1` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ ... $ $ A_N $

## 输出格式
値 $ A_1\ \times\ ...\ \times\ A_N $ を整数として出力せよ。ただし、この値が $ 10^{18} $ を超える場合は、代わりに `-1` を出力せよ。

## 题目大意
一个长度为 $n$ 的序列 $a_1,a_2,\cdots,a_n$，请求出 $s=\prod\limits_{i=1}^na_i$，如果 $s>10^{18}$ 输出 `-1`，否则输出 $s$。

```input1
2
1000000000 1000000000
```

```output1
1000000000000000000
```

```input2
3
101 9901 999999000001
```

```output2
-1
```

```input3
31
4 1 5 9 2 6 5 3 5 8 9 7 9 3 2 3 8 4 6 2 6 4 3 3 8 3 2 7 9 5 0
```

```output3
0
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 10^{18} $
- 入力は全て整数である。

### Sample Explanation 1

$ 1000000000\ \times\ 1000000000\ =\ 1000000000000000000 $ です。

### Sample Explanation 2

$ 101\ \times\ 9901\ \times\ 999999000001\ =\ 1000000000000000001 $ ですが、これは $ 10^{18} $ を超えるので、代わりに `-1` を出力します。

