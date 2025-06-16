## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc152/tasks/abc152_c

$ 1,\ \ldots,\ N $ の順列 $ P_1,\ \ldots,\ P_N $ が与えられます。  
 次の条件を満たす整数 $ i(1\ \leq\ i\ \leq\ N) $ の個数を数えてください。

- 任意の整数 $ j(1\ \leq\ j\ \leq\ i) $ に対して、 $ P_i\ \leq\ P_j $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ P_1 $ $ ... $ $ P_N $

## 输出格式
条件を満たす整数 $ i $ の個数を出力せよ。

## 题目大意
给定一个排列 $(P_1,\ldots,P_N)$ 为 $1,\ldots,N$ 。找出满足以下条件的整数 $i(1 \leq i \leq N)$ 的数目：
- 对于任意整数 $j(1 \leq j \leq i)$，$P_i \leq P_j$。

```input1
5
4 2 5 1 3
```

```output1
3
```

```input2
4
4 3 2 1
```

```output2
4
```

```input3
6
1 2 3 4 5 6
```

```output3
1
```

```input4
8
5 7 4 2 6 8 1 3
```

```output4
4
```

```input5
1
1
```

```output5
1
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ P_1,\ \ldots,\ P_N $ は $ 1,\ \ldots,\ N $ の順列である。
- 入力はすべて整数である。

### Sample Explanation 1

$ i=1,2,4 $ が条件を満たします。 $ i=3 $ は条件を満たしません。 例えば、 $ j=1 $ とすると、 $ P_i\ >\ P_j $ となります。 同様に、 $ i=5 $ も条件を満たしません。 したがって、条件を満たす整数 $ i $ の個数は $ 3 $ となります。

### Sample Explanation 2

すべての整数 $ i(1\ \leq\ i\ \leq\ N) $ が条件を満たします。

### Sample Explanation 3

$ i=1 $ のみが条件を満たします。

