## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc060/tasks/agc060_d

$ (1,2,\cdots,N) $ の順列のペア $ (P,Q)=((P_1,P_2,\cdots,P_N),(Q_1,Q_2,\cdots,Q_N)) $ であって，次の条件を満たすものの個数を $ 998244353 $ で割ったあまりを求めてください．

- すべての $ i $ ($ 1\ \leq\ i\ \leq\ N-1 $) について，以下のいずれかの条件が成り立つ．
  - $ P_i\ <\ P_{i+1} $ かつ $ Q_i\ <\ Q_{i+1} $
  - $ P_i\ >\ P_{i+1} $ かつ $ Q_i\ >\ Q_{i+1} $

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $

## 输出格式
答えを出力せよ．

## 题目大意
计算有多少个 $1 \dots n$ 的排列对 $(A,B)$ 满足 $(A_{i+1}-A_i)(B_{i+1}-B_i) > 0$ 对于每一个 $1\leq i < n$ 都成立。

$2\leq n\leq 2\times 10 ^ 5$。

```input1
2
```

```output1
2
```

```input2
3
```

```output2
10
```

```input3
4
```

```output3
88
```

```input4
10
```

```output4
286574791
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- 入力される数はすべて整数

### Sample Explanation 1

$ (P,Q)=((1,2),(1,2)) $ と $ (P,Q)=((2,1),(2,1)) $ の $ 2 $ つが条件を満たします．

