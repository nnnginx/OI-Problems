## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc118/tasks/abc118_a

正整数 $ A,\ B $ が与えられます。

$ A $ が $ B $ の約数なら $ A\ +\ B $ を、そうでなければ $ B\ -\ A $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式
$ A $ が $ B $ の約数なら $ A\ +\ B $ を、そうでなければ $ B\ -\ A $ を出力せよ。

## 题目大意
给您正整数 $A$ 和 $B$。

如果 $A$ 是 $B$ 的除数，则打印 $A + B$； 否则，打印 $B -A$。

```input1
4 12
```

```output1
16
```

```input2
8 20
```

```output2
12
```

```input3
1 1
```

```output3
2
```

## 提示
### 制約

- 入力は全て整数である。
- $ 1\ \leq\ A\ \leq\ B\ \leq\ 20 $

### Sample Explanation 1

$ 4 $ は $ 12 $ の約数なので $ 4\ +\ 12\ =\ 16 $ を出力します。

### Sample Explanation 3

$ 1 $ は $ 1 $ の約数です。

