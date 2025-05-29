## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc248/tasks/abc248_h

$ (1,\ldots,N) $ を並び替えて得られる長さ $ N $ の順列 $ P=(P_1,\ldots,P_N) $、及び整数 $ K $ が与えられます。

以下の条件を全て満たす整数組 $ (L,R) $ の個数を求めてください。

- $ 1\ \leq\ L\ \leq\ R\ \leq\ N $
- $ \mathrm{max}(P_L,\ldots,P_R)\ -\ \mathrm{min}(P_L,\ldots,P_R)\ \leq\ R\ -\ L\ +\ K $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ P_1 $ $ P_2 $ $ \ldots $ $ P_N $

## 输出格式
答えを出力せよ。

## 题目大意
给定排列 $ P_n $ 和整数 $ k $，求满足如下条件的点对 $ (l, r) $ 数量。

* $ 1 \le l \le r \le n $。
* $ \max_{i = l}^rP_i - \min_{i = l}^rP_i \le r - l + k $。

```input1
4 1
1 4 2 3
```

```output1
9
```

```input2
2 0
2 1
```

```output2
3
```

```input3
10 3
3 7 10 1 9 5 4 8 6 2
```

```output3
37
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 1.4\times\ 10^5 $
- $ P $ は $ (1,\ldots,N) $ を並び替えて得られる順列
- $ 0\ \leq\ K\ \leq\ 3 $
- 入力は全て整数

### Sample Explanation 1

条件を満たす組 $ (L,R) $ は以下の $ 9 $ 個です。 - $ (1,1) $ - $ (1,3) $ - $ (1,4) $ - $ (2,2) $ - $ (2,3) $ - $ (2,4) $ - $ (3,3) $ - $ (3,4) $ - $ (4,4) $ $ (L,R)\ =\ (1,2) $ は $ \mathrm{max}(A_1,A_2)\ -\mathrm{min}(A_1,A_2)\ =\ 4-1\ =\ 3 $ 、$ R-L+K=2-1+1\ =\ 2 $ となるので、条件を満たしません。

