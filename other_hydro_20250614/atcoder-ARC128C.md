## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc128/tasks/arc128_c

整数 $ N,M,S $，及び長さ $ N $ の整数列 $ A=(A_1,A_2,\cdots,A_N) $ が与えられます．

次の条件をすべて満たす長さ $ N $ の非負**実数**列 $ x=(x_1,x_2,\cdots,x_N) $ を作ることを考えます．

- $ 0\ \leq\ x_1\ \leq\ x_2\ \leq\ \cdots\ \leq\ x_N\ \leq\ M $
- $ \sum_{1\ \leq\ i\ \leq\ N}\ x_i=S $

ここで，$ x $ のスコアを $ \sum_{1\ \leq\ i\ \leq\ N}\ A_i\ \times\ x_i $ と定義します． $ x $ のスコアとしてありうる最大の値を求めてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ M $ $ S $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式
答えを出力せよ． 絶対誤差または相対誤差が $ 10^{-6} $ 以内であれば，正解と判定される．

## 题目大意
给定一个长度为 $n$ 的序列 $a$。称 $\sum\limits_{i=1}^n p_i=S$ 且 $0\le p_1\le p_2\le \cdots \le p_n \le m$ 的序列 $p$ 为猴子数列。$p_i$ **可以为任意实数**。

求 $\max\sum\limits_{i=1}^n a_ip_i$，其中 $p$ 是一个猴子数列。

translated by @[liangbowen](https://www.luogu.com.cn/user/367488).

```input1
3 2 3
1 2 3
```

```output1
8.00000000000000000000
```

```input2
3 3 2
5 1 1
```

```output2
4.66666666666666666667
```

```input3
10 234567 1000000
353239 53676 45485 617014 886590 423581 172670 928532 312338 981241
```

```output3
676780145098.25000000000000000000
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 5000 $
- $ 1\ \leq\ M\ \leq\ 10^6 $
- $ 1\ \leq\ S\ \leq\ \min(N\ \times\ M,10^6) $
- $ 1\ \leq\ A_i\ \leq\ 10^6 $
- 入力される値はすべて整数である

### Sample Explanation 1

$ x=(0,1,2) $ とするのが最適です．

### Sample Explanation 2

$ x=(2/3,2/3,2/3) $ とするのが最適です．

