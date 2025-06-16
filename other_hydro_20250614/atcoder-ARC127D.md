## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc127/tasks/arc127_d

長さ $ N $ の整数列 $ (A_1,A_2,\cdots,A_N) $ および $ (B_1,B_2,\cdots,B_N) $ が与えられます．

$ \sum_{1\ \leq\ i\ <\ j\ \leq\ N}\ \min(A_i\ \oplus\ A_j,\ B_i\ \oplus\ B_j) $ の値を求めてください． ただしここで，$ \oplus $ はビットごとの排他的論理和を表します．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $ $ B_1 $ $ B_2 $ $ \cdots $ $ B_N $

## 输出格式
答えを出力せよ．

## 题目大意
给定两个长度为 $n$ 的数组 a,b，求

$$\sum_{i=1}^n\sum_{j=i+1}^n\min\{a_i\oplus a_j,b_i\oplus b_j\}$$

其中 $oplus$ 表示按位异或。

```input1
3
1 2 3
4 5 6
```

```output1
4
```

```input2
4
1 2 3 4
1 2 3 4
```

```output2
24
```

```input3
10
195247 210567 149398 9678 23694 46151 187762 17915 176476 249828
68649 128425 249346 62366 194119 117620 26327 161384 207 57656
```

```output3
4019496
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 250000 $
- $ 0\ \leq\ A_i,B_i\ <\ 2^{18} $
- 入力される値はすべて整数である

### Sample Explanation 1

\- $ \min(1\ \oplus\ 2,\ 4\ \oplus\ 5)=\min(3,1)=1 $ - $ \min(1\ \oplus\ 3,\ 4\ \oplus\ 6)=\min(2,2)=2 $ - $ \min(2\ \oplus\ 3,\ 5\ \oplus\ 6)=\min(1,3)=1 $ よって，答えは $ 1+2+1=4 $ になります．

