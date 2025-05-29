## 题目描述
[problemUrl]: https://atcoder.jp/contests/toyota2023spring-final/tasks/toyota2023spring_final_a

$ N $ 行 $ M $ 列からなる盤面があり，各マス目には row-major 順に $ 1 $ から $ N\ \times\ M $ までの整数が書かれています． つまり，上から $ i $ 行目，左から $ j $ 列目のマスに書かれている整数を $ A_{i,j} $ で表すことにすると， $ A_{i,j}=(i-1)\ \times\ M\ +\ j $ です．

この盤面の部分長方形であって，その内部に書かれた値の総和がちょうど $ V $ になるものの個数を数えてください．

より厳密に言えば，整数の $ 4 $ つ組 $ (a,b,c,d) $ ($ 1\ \leq\ a\ \leq\ b\ \leq\ N $, $ 1\ \leq\ c\ \leq\ d\ \leq\ M $) であって，$ \sum_{a\ \leq\ i\ \leq\ b,\ c\ \leq\ j\ \leq\ d}\ A_{i,j}=V $ を満たすものの個数を数えてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ M $ $ V $

## 输出格式
答えを出力せよ．

## 题目大意
给定一个 $N\times M$ 的矩阵 $A$，其中 $a_{i,j}=(i-1)\times M+j$，求出其中所有元素和为 $V$ 的子矩阵个数。

```input1
2 2 3
```

```output1
2
```

```input2
2 2 5
```

```output2
0
```

```input3
13 8 1032
```

```output3
5
```

## 提示
### 制約

- $ 1\ \leq\ N,\ M\ \leq\ 5000 $
- $ 1\ \leq\ V\ \leq\ 10^{15} $
- 入力される値はすべて整数である

### Sample Explanation 1

盤面には以下のように整数が書き込まれています． ``` 12 34 ``` 条件を満たす部分長方形は，$ (a,b,c,d)=(1,1,1,2),(2,2,1,1) $ の $ 2 $ つです．

