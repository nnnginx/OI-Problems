## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc155/tasks/arc155_c

長さ $ N $ の整数列 $ A=(A_1,\ A_2,\ \dots,\ A_N),\ B=(B_1,\ B_2,\ \dots,\ B_N) $ が与えられます。

あなたは以下の操作を好きな回数行うことができます。

- $ A_i+A_{i+1}+A_{i+2} $ が偶数であるような整数 $ i\ (1\ \leq\ i\ \leq\ N-2) $ を選ぶ。そして $ A_i,\ A_{i+1},\ A_{i+2} $ を好きに並び替える。
 
$ A $ を $ B $ に一致させることができるか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $ $ B_1 $ $ B_2 $ $ \dots $ $ B_N $

## 输出格式
$ A $ を $ B $ に一致させることが可能な場合は `Yes` を、そうでない場合は `No` を出力せよ。

## 题目大意
Feyn 有两个长度为 $n$ 的整数序列 $A,B$，他可以执行以下操作任意次：

+ 选定 $i\in [1,n-2]$，如果 $A_i+A_{i+1}+A_{i+2}$ 是偶数，则可以任意重排这三个数的位置。

请判断他是否能通过操作将 $A$ 序列变成 $B$ 序列。

(translated by 342873)

```input1
5
1 2 3 4 5
3 1 2 4 5
```

```output1
Yes
```

```input2
5
1 2 4 6 5
5 1 4 2 6
```

```output2
No
```

```input3
9
2 10 4 3 6 2 6 8 5
2 4 10 3 8 6 6 2 5
```

```output3
Yes
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i,\ B_i\ \leq\ 2\ \times\ 10^5 $
- 入力される値はすべて整数
 
### Sample Explanation 1

$ A_1+A_2+A_3 $ は $ 1+2+3=6 $ であり偶数なので、操作では $ i=1 $ を選ぶことができます。 $ i=1 $ を選んで操作し、$ A_1,\ A_2,\ A_3 $ を $ A_3,\ A_1,\ A_2 $ に並び替えると、 $ A $ は $ (3,\ 1,\ 2,\ 4,\ 5) $ に変化します。 この操作により $ A $ を $ B $ に一致させることができるので、 `Yes` を出力します。

