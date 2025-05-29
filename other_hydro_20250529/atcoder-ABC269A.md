## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc269/tasks/abc269_a

整数 $ a,\ b,\ c,\ d $ が与えられるので、以下の指示に従って 2 行出力してください。

1 行目は $ (a\ +\ b)\ \times\ (c\ -\ d) $ の計算結果を整数として出力してください。  
 2 行目は入力にかかわらず `Takahashi` と出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ c $ $ d $

## 输出格式
問題文の指示に従って 2 行出力せよ。

## 题目大意
题意:

输入整数 $ a,\ b,\ c,\ d $ .

第一行输出 $ (a\ +\ b)\ \times\ (c\ -\ d) $ 的计算结果(以整数输出).

第二行输出 `Takahashi`

```input1
1 2 5 3
```

```output1
6
Takahashi
```

```input2
10 -20 30 -40
```

```output2
-700
Takahashi
```

```input3
100 100 100 -100
```

```output3
40000
Takahashi
```

## 提示
### 制約

- $ -100\ \leq\ a,\ b,\ c,\ d\ \leq\ 100 $
- $ a,b,c,d $ は整数

### Sample Explanation 1

$ (1\ +\ 2)\ \times(5\ -\ 3)\ =\ 3\ \times\ 2\ =\ 6 $ です。よって 1 行目は $ 6 $ を出力します。 2 行目は `Takahashi` を出力します。1 文字目を小文字にしたりスペルを誤ったりすると誤答となるので注意してください。

### Sample Explanation 2

入出力に負の数が含まれる場合もあります。

