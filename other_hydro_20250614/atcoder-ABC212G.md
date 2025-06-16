## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc212/tasks/abc212_g

素数 $ P $ が与えられます。

以下の条件を満たす整数の組 $ (x,\ y) $ はいくつありますか？

- $ 0\ \leq\ x\ \leq\ P-1 $
- $ 0\ \leq\ y\ \leq\ P-1 $
- ある正整数 $ n $ が存在して、$ x^n\ \equiv\ y\ \pmod{P} $ を満たす

ただし答えは非常に大きくなる可能性があるので、$ 998244353 $ で割った余りを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ P $

## 输出格式
答えを $ 998244353 $ で割った余りを出力せよ。

## 题目大意
给定质数 $P$，求有多少个整数 $x,y$，满足

- $0\le x,y\le P-1$

- $\exist n\in \mathbb{N},x^n\equiv y\pmod p$

translated by @ternary_tree

```input1
3
```

```output1
4
```

```input2
11
```

```output2
64
```

```input3
998244353
```

```output3
329133417
```

## 提示
### 制約

- $ 2\ \leq\ P\ \leq\ 10^{12} $
- $ P $ は素数

### Sample Explanation 1

$ (x,\ y)\ =\ (0,\ 0),\ (1,\ 1),\ (2,\ 1),\ (2,\ 2) $ の $ 4 $ 組が条件を満たします。

