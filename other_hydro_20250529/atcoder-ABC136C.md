## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc136/tasks/abc136_c

左右一列に $ N $ 個のマスが並んでおり、左から $ i $ 番目のマスの高さは $ H_i $ です。

あなたは各マスについて $ 1 $ 度ずつ次のいずれかの操作を行います。

- マスの高さを $ 1 $ 低くする。
- 何もしない。

操作をうまく行うことでマスの高さを左から右に向かって単調非減少にできるか求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ H_1 $ $ H_2 $ $ ... $ $ H_N $

## 输出格式
マスの高さを左から右に向かって単調非減少にできるなら `Yes`、そうでないなら `No` を出力せよ。

## 题目大意
从左到右连续排列 $N$ 个正方形。从左起第 $i$ 个正方形的高度为 $H_i$。

对于每个正方形，您将一次执行以下任一操作：

- 将正方形的高度减少 $1$。
- 什么都不做

确定是否可以执行操作，以使正方形的高度从左到右不减小。


```input1
5
1 2 1 1 3
```

```output1
Yes
```

```input2
4
1 3 2 1
```

```output2
No
```

```input3
5
1 2 3 4 5
```

```output3
Yes
```

```input4
1
1000000000
```

```output4
Yes
```

## 提示
### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ H_i\ \leq\ 10^9 $

### Sample Explanation 1

左から $ 2 $ 番目のマスのみ高さを $ 1 $ 低くすることで目的を達成できます。

