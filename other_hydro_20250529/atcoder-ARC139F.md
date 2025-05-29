## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc139/tasks/arc139_f

PCT 君は以下の問題を作りました。

> **Xor Optimization Problem**長さ $ N $ の非負整数列 $ A_1,A_2,...,A_N $ が与えられる。$ A $ の要素を好きな個数選ぶとき、選んだ値の $ \mathrm{XOR} $ が取りうる最大値はいくらか？

この問題は、Nyaan さんにとっては簡単だったため PCT 君は以下のように改題しました。

> **Many Xor Optimization Problems**長さ $ N $ かつ全ての要素が $ 0 $ 以上 $ 2^M-1 $ 以下である整数列は $ 2^{NM} $ 通り存在しますが、その全てに対して **Xor Optimization Problem** を解いた時の解の総和を $ 998244353 $ で割ったあまりを求めてください。

**Many Xor Optimization Problems** を解いてください。

  $ \mathrm{XOR} $ とは  非負整数 $ A,\ B $ のビット単位 $ \mathrm{XOR} $ 、$ A\ \oplus\ B $ は、以下のように定義されます。

- $ A\ \oplus\ B $ を二進表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ A,\ B $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。
 
 例えば、$ 3\ \oplus\ 5\ =\ 6 $ となります (二進表記すると: $ 011\ \oplus\ 101\ =\ 110 $)。  
 一般に $ k $ 個の非負整数 $ p_1,\ p_2,\ p_3,\ \dots,\ p_k $ のビット単位 $ \mathrm{XOR} $ は $ (\dots\ ((p_1\ \oplus\ p_2)\ \oplus\ p_3)\ \oplus\ \dots\ \oplus\ p_k) $ と定義され、これは $ p_1,\ p_2,\ p_3,\ \dots,\ p_k $ の順番によらないことが証明できます。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ M $

## 输出格式
答えを出力してください。

## 题目大意
给定 $n,m$，$A_i$ 从 $[0,2^m-1]$ 中随机生成。

令 $F(A)$ 为所有子集异或和的最大值，即对于一个下标集合 $S=\{i_1,i_2,\cdots,i_k\}$，$A_{i_1}\oplus A_{i_2}\oplus\cdots\oplus A_{i_k}$ 的最大值。

对于 $2^{nm}$ 种生成方式，求 $F(A)$ 的和模 $998244353$。

```input1
2 1
```

```output1
3
```

```input2
3 4
```

```output2
52290
```

```input3
1234 5678
```

```output3
495502261
```

## 提示
### 制約

- $ 1\ \le\ N,M\ \le\ 250000 $
- 入力は全て整数である。

### Sample Explanation 1

長さが $ 2 $ かつ全ての要素が $ 0 $ 以上 $ 1 $ 以下である整数列全てに対して \*\*Xor Optimization Problem\*\* を解きます。 - $ A=(0,0) $ の時の解は $ 0 $ - $ A=(0,1) $ の時の解は $ 1 $ - $ A=(1,0) $ の時の解は $ 1 $ - $ A=(1,1) $ の時の解は $ 1 $ よって、$ 0+1+1+1=3 $ が解となります。

