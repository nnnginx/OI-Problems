## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc109/tasks/abc109_a

$ 1 $ 以上 $ 3 $ 以下の整数 $ A,\ B $ が与えられます。

$ A\ \times\ B\ \times\ C $ が奇数となるような $ 1 $ 以上 $ 3 $ 以下の整数 $ C $ が存在するか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
条件を満たすような $ C $ が存在するなら `Yes`、そうでないなら `No` を出力せよ。

## 题目大意
### 题目描述

给出两个正整数 $a, b$ 且 $1 \le a, b \le 3$，判断是否有正整数 $c$ 满足 $1 \le c \le 3$ 且 $a \times b \times c$ 是奇数。若有输出 "Yes"，否则输出 "No"。

### 输入格式

输入两个数 $a, b$。

### 输出格式

如果有数 $c$ 满足条件则输出 "Yes"，否则输出 "No"。

```input1
3 1
```

```output1
Yes
```

```input2
1 2
```

```output2
No
```

```input3
2 2
```

```output3
No
```

## 提示
### 制約

- 入力はすべて整数である
- $ 1\ \leq\ A,\ B\ \leq\ 3 $

### Sample Explanation 1

$ C\ =\ 3 $ とすると $ A\ \times\ B\ \times\ C\ =\ 3\ \times\ 1\ \times\ 3\ =\ 9 $ となり、奇数となります。

