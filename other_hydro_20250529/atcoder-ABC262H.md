## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc262/tasks/abc262_h

長さ $ N $ の整数列 $ A\ =\ (A_1,\ \dots,\ A_N) $ であって、以下の条件を全て満たすものの総数を $ 998244353 $ で割った余りを求めてください。

- $ 1\ \leq\ i\ \leq\ N $ を満たす全ての $ i $ について、$ 0\ \leq\ A_i\ \leq\ M $
- $ 1\ \leq\ j\ \leq\ Q $ を満たす全ての $ j $ について、$ A_{L_j},\ \dots,\ A_{R_j} $ の最大値は $ X_j $ である。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ Q $ $ L_1 $ $ R_1 $ $ X_1 $ $ \vdots $ $ L_Q $ $ R_Q $ $ X_Q $

## 输出格式
答えを出力せよ。

## 题目大意
### 题目大意
求满足以下条件的长度为 $N$ 的序列 $A=(A_1,A_2,\cdots A_N)$ 有多少种：
+ $\forall i \in[1,N],0\leq A_i\leq M$
+ $\forall i \in[1,Q],\max \limits_{L_i\leq j\leq R_i}A_j=X_i$
### 输入格式
第一行输入 $3$ 个正整数 $N,M,Q$ 

后面 $Q$ 行每行 $3$ 个正整数表示 $L_i,R_i,X_i$

$1\leq N\leq 2\times 10^5$

$1\leq M<998244353$

$1\leq Q\leq 2\times 10^5$

$\forall i \in [1,Q],1\leq L_i\leq R_i\leq N,1\leq X_i\leq M$
### 输出格式
输出满足条件的序列数，对 $998244353$ 取模。

```input1
3 3 2
1 2 2
2 3 3
```

```output1
5
```

```input2
1 1 1
1 1 1
```

```output2
1
```

```input3
6 40000000 3
1 4 30000000
2 6 20000000
3 5 10000000
```

```output3
135282163
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ M\ \lt\ 998244353 $
- $ 1\ \leq\ Q\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ L_i\ \leq\ R_i\ \leq\ N\ \,\ (1\ \leq\ i\ \leq\ Q) $
- $ 1\ \leq\ X_i\ \leq\ M\ \,\ (1\ \leq\ i\ \leq\ Q) $
- 入力は全て整数

### Sample Explanation 1

$ A\ =\ (0,\ 2,\ 3),\ (1,\ 2,\ 3),\ (2,\ 0,\ 3),\ (2,\ 1,\ 3),\ (2,\ 2,\ 3) $ が条件を満たします。

