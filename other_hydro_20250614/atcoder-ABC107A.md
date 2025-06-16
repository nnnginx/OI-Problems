## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc107/tasks/abc107_a

$ N $ 両編成の列車があります。 この列車の前から $ i $ 両目は、後ろから何両目でしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ i $

## 输出格式
答えを出力せよ。

## 题目大意
给定两个数 $N,i(N\leq100,i\leq N)$，找到一个 $j$，使得 $N$ 辆火车中从前往后数第 $i$ 辆与从后往前数第 $j$ 辆是同一辆火车。

```input1
4 2
```

```output1
3
```

```input2
1 1
```

```output2
1
```

```input3
15 11
```

```output3
5
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ i\ \leq\ N $

### Sample Explanation 1

$ 4 $ 両編成の列車において、前から $ 2 $ 両目の車両は、後ろから $ 3 $ 両目です。

