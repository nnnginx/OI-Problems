## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc252/tasks/abc252_d

長さ $ N $ の数列 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。  
 以下の $ 2 $ 条件をともに満たすような整数の組 $ (i,j,k) $ の個数を求めてください。

- $ 1\leq\ i\ \lt\ j\ \lt\ k\ \leq\ N $
- $ A_i,A_j,A_k $ は相異なる

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
有一个长度为 $n$ 的数列 $A$，求满足以下条件的三元组的数量：

* $1 \leq i < j < k \leq n $

* $A_i$，$A_j$，$A_k$ 互不相同

$ 3 \leq n \leq 2 \times 10^5 $

$ 1 \leq A_i \leq 2 \times 10^5 $

```input1
4
3 1 4 1
```

```output1
2
```

```input2
10
99999 99998 99997 99996 99995 99994 99993 99992 99991 99990
```

```output2
120
```

```input3
15
3 1 4 1 5 9 2 6 5 3 5 8 9 7 9
```

```output3
355
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 2\times\ 10^5 $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

条件を満たす整数の組 $ (i,j,k) $ は $ (1,2,3),(1,3,4) $ の $ 2 $ つです。

