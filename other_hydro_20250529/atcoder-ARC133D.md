## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc133/tasks/arc133_d

整数 $ L,R,V $ が与えられます． 次の条件を両方満たす整数の組 $ (l,r) $ の個数を $ 998244353 $ で割った余りを求めてください．

- $ L\ \leq\ l\ \leq\ r\ \leq\ R $
- $ l\ \oplus\ (l+1)\ \oplus\ \cdots\ \oplus\ r=V $

ただしここで，$ \oplus $ はビット単位 $ \mathrm{XOR} $ 演算を表します．

  ビット単位 $ \mathrm{XOR} $ 演算とは  非負整数 $ A,\ B $ のビット単位 $ \mathrm{XOR} $ 、$ A\ \oplus\ B $ は、以下のように定義されます。

- $ A\ \oplus\ B $ を二進表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ A,\ B $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。
 
 例えば、$ 3\ \oplus\ 5\ =\ 6 $ となります (二進表記すると: $ 011\ \oplus\ 101\ =\ 110 $)。  
 一般に $ k $ 個の非負整数 $ p_1,\ p_2,\ p_3,\ \dots,\ p_k $ のビット単位 $ \mathrm{XOR} $ は $ (\dots\ ((p_1\ \oplus\ p_2)\ \oplus\ p_3)\ \oplus\ \dots\ \oplus\ p_k) $ と定義され、これは $ p_1,\ p_2,\ p_3,\ \dots\ p_k $ の順番によらないことが証明できます。

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ L $ $ R $ $ V $

## 输出格式
答えを出力せよ．

## 题目大意
定义 $\oplus$ 为**异或**运算，给定整数 $L,R,V$，求：

$$
\displaystyle\sum_{l=L}^{R}\displaystyle\sum_{r=l}^{R}[(\oplus_{i=l}^{r}i)=V]
$$

$1\leqslant L,R\leqslant 10^{18}$，$0\leqslant V\leqslant 10^{18}$。

```input1
1 3 3
```

```output1
2
```

```input2
10 20 0
```

```output2
6
```

```input3
1 1 1
```

```output3
1
```

```input4
12345 56789 34567
```

```output4
16950
```

## 提示
### 制約

- $ 1\ \leq\ L\ \leq\ R\ \leq\ 10^{18} $
- $ 0\ \leq\ V\ \leq\ 10^{18} $
- 入力される値はすべて整数である

### Sample Explanation 1

条件を満たすのは，$ (l,r)=(1,2) $ と $ (l,r)=(3,3) $ の $ 2 $ つです．

