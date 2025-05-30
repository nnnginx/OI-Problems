## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc151/tasks/abc151_b

高橋君は $ N $ 科目のテストを受けます。各テストは $ K $ 点満点であり、点数はそれぞれ $ 0 $ 以上の整数です。

高橋君は $ N-1 $ 科目のテストを既に受けており、$ i $ 番目の科目のテストの点数は $ A_i $ 点でした。

高橋君の目標は、$ N $ 科目のテストの平均点を $ M $ 点以上にすることです。

高橋君が目標を達成するためには、最後のテストで最低何点取る必要があるか出力してください。

達成不可能である場合は、代わりに `-1` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ M $ $ A_1 $ $ A_2 $ $ ... $ $ A_{N-1} $

## 输出格式
最後のテストでの必要最低点または `-1` を出力せよ。

## 题目大意
高桥要参加 $N$ 门科目的考试，每门考试的满分都是 $K$ 分。他给自己定了 $N$ 门平均分上 $M$ 分的目标（含 $M$ 分）。现在高桥已经完成了 $N-1$ 门科目的考试，他在第 $i$ 门考试中的得分为 $A_i$ 分。现在高桥给出了你 $N,K,M$ 以及所有的 $A_i$ ，想请你求出他为了达成目标，在最后的测试中至少应该得多少分。如果他不可能完成目标，输出-1.

```input1
5 10 7
8 10 3 6
```

```output1
8
```

```input2
4 100 60
100 100 100
```

```output2
0
```

```input3
4 100 60
0 0 0
```

```output3
-1
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ K\ \leq\ 100 $
- $ 1\ \leq\ M\ \leq\ K $
- $ 0\ \leq\ A_i\ \leq\ K $
- 入力中のすべての値は整数である。

### Sample Explanation 1

最後のテストで $ 8 $ 点を取ると、$ (8+10+3+6+8)/5\ =\ 7 $ より平均点は $ 7 $ 点となり目標を達成できます。

### Sample Explanation 2

最後のテストで $ 0 $ 点を取っても目標を達成できます。

### Sample Explanation 3

もはや挽回は不可能です。

