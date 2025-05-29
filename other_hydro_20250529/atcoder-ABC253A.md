## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc253/tasks/abc253_a

整数 $ a,\ b,\ c $ が与えられます。$ b $ がこれらの整数の中央値であるかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ c $

## 输出格式
$ b $ が与えられた整数の中央値であるならば `Yes`、そうでないならば `No` と出力せよ。

## 题目大意
输入3个整数a,b,c，判断b是不是中间大小的数，是输出Yes，不是输出No

```input1
5 3 2
```

```output1
Yes
```

```input2
2 5 3
```

```output2
No
```

```input3
100 100 100
```

```output3
Yes
```

## 提示
### 制約

- $ 1\ \leq\ a,\ b,\ c\ \leq\ 100 $
- 入力は全て整数

### Sample Explanation 1

与えられた整数を小さい順に並べると $ 2,\ 3,\ 5 $ となり、$ b $ はこれらの整数の中央値です。

### Sample Explanation 2

$ b $ は与えられた整数の中央値ではありません。

