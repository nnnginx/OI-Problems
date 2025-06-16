# AT_pakencamp_2020_day1_o Xor Sum Sum

## 题目描述

[problemUrl]: https://atcoder.jp/contests/pakencamp-2020-day1/tasks/pakencamp_2020_day1_o

 kaage くんは [Xor Sum](https://atcoder.jp/contests/abc050/tasks/arc066_b) っぽい問題を作ろうと思いました。次の問題を解いてください。

 長さ $ N $ の数列 $ A,\ B $ が与えられる。 集合 $ U=\{x|x\in\mathbb{N},1\leq\ x\leq\ N\} $ の空でない任意の部分集合 $ S $ をとったとき、$ S=\{k_1,\ k_2,\ \cdots\ k_l\} $ として、$ (A_{k_1}\ xor\ A_{k_2}\ xor\cdots\ xor\ A_{k_l})+(B_{k_1}\ xor\ B_{k_2}\ xor\cdots\ xor\ B_{k_l}) $ の最大値を求めよ。 ただし、ここで $ xor $ はビットごとの排他的論理和を表す。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $  
> \\(A\_1\\) \\(A\_2\\) \\(\\cdots\\ A\_N\\)  
> \\(B\_1\\) \\(B\_2\\) \\(\\cdots\\ B\_N\\)

## 输出格式

考えられる最大値を一行に出力してください。

## 输入输出样例 #1

### 输入 #1

```
4
4 2 6 7
1 5 3 4
```

### 输出 #1

```
11
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 5\times\ 10^5 $
- $ 0\ \leq\ A_i,B_i $