## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc188/tasks/abc188_b

$ 2 $ つの $ N $ 次元ベクトル $ A\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_N),\ B\ =\ (B_1,\ B_2,\ B_3,\ \dots,\ B_N) $ が与えられます。  
 $ A $ と $ B $ の内積が $ 0 $ かどうかを判定してください。  
 すなわち、$ A_1B_1\ +\ A_2B_2\ +\ A_3B_3\ +\ \dots\ +\ A_NB_N\ =\ 0 $ かどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ A_3 $ $ \dots $ $ A_N $ $ B_1 $ $ B_2 $ $ B_3 $ $ \dots $ $ B_N $

## 输出格式
$ A $ と $ B $ の内積が $ 0 $ ならば `Yes` を、$ 0 $ でないならば `No` を出力せよ。

## 题目大意
给定两个长度为 $n$ 的数组，$A$ 和 $B$。

若 $A_1 \times B_1 + A_2 \times B_2 +\cdots+A_n \times B_n = 0$ ，则输出 ``Yes``，否则输出 ``No``。

```input1
2
-3 6
4 2
```

```output1
Yes
```

```input2
2
4 5
-1 -3
```

```output2
No
```

```input3
3
1 3 5
3 -6 3
```

```output3
Yes
```

## 提示
### 制約

- $ 1\ \le\ N\ \le\ 100000 $
- $ -100\ \le\ A_i\ \le\ 100 $
- $ -100\ \le\ B_i\ \le\ 100 $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

$ A $ と $ B $ の内積は $ (-3)\ \times\ 4\ +\ 6\ \times\ 2\ =\ 0 $ です。

### Sample Explanation 2

$ A $ と $ B $ の内積は $ 4\ \times\ (-1)\ +\ 5\ \times\ (-3)\ =\ -19 $ です。

### Sample Explanation 3

$ A $ と $ B $ の内積は $ 1\ \times\ 3\ +\ 3\ \times\ (-6)\ +\ 5\ \times\ 3\ =\ 0 $ です。

