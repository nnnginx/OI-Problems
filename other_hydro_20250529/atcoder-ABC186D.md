## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc186/tasks/abc186_d

$ N $ 個の整数 $ A_1,\ldots,A_N $ が与えられます。

$ 1\leq\ i\ <\ j\ \leq\ N $ を満たす全ての $ i,j $ の組についての $ |A_i-A_j| $ の和を求めてください。

すなわち、$ \displaystyle{\sum_{i=1}^{N-1}\sum_{j=i+1}^{N}\ |A_i-A_j|} $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
### 题意简述
高桥君~~又~~想了一个新游戏。

输入 $n$ 个整数 $a_1,a_2,...a_n$，

求在满足 $1 \leq i < j \leq n$ 的所有 $\lvert a_i-a_j \rvert$ 的和 $X$ 。

即求$X=\sum_{i=1}^{n-1}\sum_{j=i+1}^{n} \lvert a_i-a_j\rvert$ 。

### 输入格式
第一行是一个整数 $n$ ,

第二行是 $n$ 个整数 $a_1,a_2...a_n$。

所有数据保证 $2 \leq n \leq 10^5,\lvert a_i\rvert \leq 10^8。$

### 输出格式
输出所求的 $X$ 。

```input1
3
5 1 2
```

```output1
8
```

```input2
5
31 41 59 26 53
```

```output2
176
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ |A_i|\leq\ 10^8 $
- $ A_i $ は整数である。

### Sample Explanation 1

$ |5-1|+|5-2|+|1-2|=8 $ です。

