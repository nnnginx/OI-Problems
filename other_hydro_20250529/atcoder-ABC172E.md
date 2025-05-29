## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc172/tasks/abc172_e

$ 1 $ 以上 $ M $ 以下の整数からなる長さ $ N $ の数列 $ A_1,A_2,\cdots,\ A_{N} $ と $ B_1,B_2,\cdots,\ B_{N} $ の組であって、以下の条件をすべて満たすものの個数を求めてください。

- $ 1\leq\ i\leq\ N $ なる任意の $ i $ について $ A_i\ \neq\ B_i $
- $ 1\leq\ i\ <\ j\leq\ N $ なる任意の $ (i,j) $ について $ A_i\ \neq\ A_j $ かつ $ B_i\ \neq\ B_j $

ただし、答えは非常に大きくなる可能性があるので、$ (10^9+7) $ で割ったあまりを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
答えを $ (10^9+7) $ で割ったあまりを出力せよ。

## 题目大意
给定 $N$，$M$。

构造长为 $N$ 的整数序列 $A,B$ ，满足：

- $1 \leq A_i,B_i \leq M$
- $\forall i\neq j$，$A_i\neq A_j,B_i\neq B_j$
- $\forall i$，$A_i\neq B_i$

求合法构造方案数，对 $10^9+7$ 取模。

```input1
2 2
```

```output1
2
```

```input2
2 3
```

```output2
18
```

```input3
141421 356237
```

```output3
881613484
```

## 提示
### 制約

- $ 1\leq\ N\ \leq\ M\ \leq\ 5\times10^5 $
- 入力はすべて整数

### Sample Explanation 1

$ A_1=1,A_2=2,B_1=2,B_2=1 $ のときと $ A_1=2,A_2=1,B_1=1,B_2=2 $ のとき条件が満たされます。

