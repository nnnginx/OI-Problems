## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc155/tasks/abc155_d

$ N $ 個の整数 $ A_1,\ A_2,\ ...,\ A_N $ があります。

このうち $ 2 $ つを選んでペアにする方法は $ \frac{N(N-1)}{2} $ 通りありますが、それぞれのペアについて積を求め、小さい順に並べ替えたとき、$ K $ 番目にくる数は何になるでしょう？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
$N$个数两两相乘的结果有 $\frac{N(N-1)}{2}$ 种，问第 $K$ 小的乘积是多少。  
输入格式：  
第一行两个整数 $N,K$。  
第二行 $N$ 个整数 $A_i$，为那 $N$ 个要乘起来的数  
输出格式：  
一行一个整数，第 $K$ 小的乘积  
数据范围：  
$N \leq 2 \times 10^5,-10^9 \leq A_i \leq 10^9$

```input1
4 3
3 3 -4 -2
```

```output1
-6
```

```input2
10 40
5 4 3 2 -1 0 0 0 0 0
```

```output2
6
```

```input3
30 413
-170202098 -268409015 537203564 983211703 21608710 -443999067 -937727165 -97596546 -372334013 398994917 -972141167 798607104 -949068442 -959948616 37909651 0 886627544 -20098238 0 -948955241 0 -214720580 277222296 -18897162 834475626 0 -425610555 110117526 663621752 0
```

```output3
448283280358331064
```

## 提示
### 制約

- 入力はすべて整数
- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ K\ \leq\ \frac{N(N-1)}{2} $
- $ -10^9\ \leq\ A_i\ \leq\ 10^9\ (1\ \leq\ i\ \leq\ N) $

### Sample Explanation 1

ペアの組み方は $ 6 $ 通りあり、それぞれの積は $ 9,\ -12,\ -6,\ -12,\ -6,\ 8 $ です。 小さい順に並べ替えると $ -12,\ -12,\ -6,\ -6,\ 8,\ 9 $ となり、$ 3 $ 番目にくる数は $ -6 $ です。

