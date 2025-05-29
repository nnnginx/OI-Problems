## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc107/tasks/arc107_b

整数 $ N,K $ が与えられます． $ 4 $ つの整数の組 $ (a,b,c,d) $ であって，以下の条件を両方満たすものは何個あるでしょうか．

- $ 1\ \leq\ a,b,c,d\ \leq\ N $
- $ a+b-c-d=K $

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ K $

## 输出格式
答えを出力せよ．

## 题目大意
给定 $n, k$

求 $\sum_{a = 1}^{n}\sum_{b = 1}^{n}\sum_{c = 1}^{n}\sum_{d = 1}^{n}[a + b - c - d == k]$

```input1
2 1
```

```output1
4
```

```input2
2525 -425
```

```output2
10314607400
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ -2(N-1)\ \leq\ K\ \leq\ 2(N-1) $
- 入力される数はすべて整数．

### Sample Explanation 1

以下の $ 4 $ 通りです． - $ (a,b,c,d)=(2,1,1,1) $ - $ (a,b,c,d)=(1,2,1,1) $ - $ (a,b,c,d)=(2,2,2,1) $ - $ (a,b,c,d)=(2,2,1,2) $

