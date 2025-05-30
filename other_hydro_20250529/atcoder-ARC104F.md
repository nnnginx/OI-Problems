## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc104/tasks/arc104_f

一列に並んだ $ N $ 棟のビルが建設中であり、ビルには左から順番に $ 1,\ 2,\ \ldots,\ N $ の番号がついています。

長さ $ N $ の整数列 $ X $ が与えられ、ビル $ i $ の高さ $ H_i $ は、$ 1 $ 以上 $ X_i $ 以下の整数のいずれかにすることができます。

$ 1\ \leq\ i\ \leq\ N $ に対して、$ P_i $ を次のように定めます。

- $ H_j\ >\ H_i $ を満たすような整数 $ j\ (1\ \leq\ j\ <\ i) $ が存在する場合はそのような $ j $ の最大値、存在しない場合は $ -1 $ とする

全てのビルの高さの組み合わせを考えるとき、 $ P $ としてありうる整数列の個数を $ 1000000007 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X_1 $ $ X_2 $ $ \cdots $ $ X_N $

## 输出格式
全てのビルの高さの組み合わせを考えるとき、 $ P $ としてありうる整数列の個数を $ 1000000007 $ で割った余りを出力せよ。

## 题目大意
有一排共 $n$ 栋房子，同时给出一个长为 $n$ 的序列 $X$，第 $i$ 栋房子的高度 $H_i\in[1,X_i]$ 且为整数。  
按照房屋的高度生成一个序列 $P$，其中 $P_i$ 为 $i$ 左边第一个比它高的房子的编号，若不存在，则为 $-1$。  
求有多少种本质不同的 $P$，对 $10^9+7$ 取模。

```input1
3
3 2 1
```

```output1
4
```

```input2
3
1 1 2
```

```output2
1
```

```input3
5
2 2 2 2 2
```

```output3
16
```

```input4
13
3 1 4 1 5 9 2 6 5 3 5 8 9
```

```output4
31155
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ X_i\ \leq\ 10^5 $
- 入力は全て整数である

### Sample Explanation 1

$ H $ としては、次の $ 6 $ 通りが考えられます。 - $ H\ =\ (1,\ 1,\ 1) $ のとき、$ P $ は $ (-1,\ -1,\ -1) $ である - $ H\ =\ (1,\ 2,\ 1) $ のとき、$ P $ は $ (-1,\ -1,\ 2) $ である - $ H\ =\ (2,\ 1,\ 1) $ のとき、$ P $ は $ (-1,\ 1,\ 1) $ である - $ H\ =\ (2,\ 2,\ 1) $ のとき、$ P $ は $ (-1,\ -1,\ 2) $ である - $ H\ =\ (3,\ 1,\ 1) $ のとき、$ P $ は $ (-1,\ 1,\ 1) $ である - $ H\ =\ (3,\ 2,\ 1) $ のとき、$ P $ は $ (-1,\ 1,\ 2) $ である よって、$ P $ としてありうる整数列は $ (-1,\ -1,\ -1),\ (-1,\ -1,\ 2),\ (-1,\ 1,\ 1),\ (-1,\ 1,\ 2) $ の $ 4 $ 個です。

### Sample Explanation 2

$ H $ としては、次の $ 2 $ 通りが考えられます。 - $ H\ =\ (1,\ 1,\ 1) $ のとき、$ P $ は $ (-1,\ -1,\ -1) $ である - $ H\ =\ (1,\ 1,\ 2) $ のとき、$ P $ は $ (-1,\ -1,\ -1) $ である よって、$ P $ としてありうる整数列は $ 1 $ 個です。

