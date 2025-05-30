## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc264/tasks/abc264_g

文字列品評会では、英小文字のみからなる空でない文字列 $ S $ に対して、その「美しさ」を決定します。

文字列 $ S $ の美しさは、$ N $ 個の審査項目の点数の和として定められます。 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、$ i $ 番目の審査項目の点数は 「文字列 $ T_i $（入力で与えられる**長さ $ 3 $ 以下**の文字列）が $ S $ に連続な部分文字列として含まれる回数」に $ P_i $ を掛けて得られる値です。

英小文字のみからなる**空でない**文字列 $ S $ の美しさとしてあり得る最大値を出力して下さい。 ただし、美しさとしていくらでも大きい値が考えられる場合は、代わりに `Infinity` と出力して下さい。

ここで、文字列 $ U\ =\ U_1U_2\ldots\ U_{|U|} $ に文字列 $ V $ が連続な部分列として含まれる回数とは、 $ 1\ \leq\ i\ \leq\ |U|-|V|+1 $ を満たす整数 $ i $ であって $ U_iU_{i+1}\ldots\ U_{i+|V|-1}\ =\ V $ を満たすものの個数です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ T_1 $ $ P_1 $ $ T_2 $ $ P_2 $ $ \vdots $ $ T_N $ $ P_N $

## 输出格式
英小文字のみからなる**空でない**文字列 $ S $ の美しさとしてあり得る最大値を出力せよ。 ただし、美しさとしていくらでも大きい値が考えられる場合は、代わりに `Infinity` と出力せよ。

## 题目大意
在“字符串评鉴大会”上，由小写字母构成的非空字符串 $S$ 的由 $N$ 条标准决定：  

每条标准是一个字符串 $T_i$ （$T_i$ 的长度不超过 $3$）和对应的得分 $P_i$，$S$ 的“美丽度”定义为：  

$$\sum_{i=1}^N P_i\times C_i$$  

其中 $C_i$ 为 $T_i$ 在 $S$ 中出现的次数。  

字符串 $V$ 在字符串 $U=U_1U_2
\cdots U_{|U|}$ 中出现的次数定义为：满足 $1\le i\le \vert U\vert -\vert V\vert +1$ 且 $U_iU_{i+1}\cdots U_{i+\vert V\vert -1}=V$ 的整数 $i$ 的数量，其中 $\vert U\vert$ 表示字符串 $U$ 的长度。  

现在给出 $N$ 条标准，求出这 $N$ 条标准下“美丽度”最大的**非空**字符串 $S$ 的“美丽度”。如果这个答案是无限大，输出 `Infinity`。  

数据范围：  
+ $1\le N\le 18278$，$N$ 为整数。  
+ $1\le \vert T_i\vert \le 3$，$T_i$ 只包含小写字母。  
+ 若 $i\neq j$，则 $T_i\neq T_j$。  
+ $-10^9\le P_i\le 10^9$。  
+ $P_i$ 均为整数。  

样例解释：  

样例 $1$：$S$ 为 $X$ 个 $\texttt{abz}$ 相连时，它的“美丽度”是 $5X$，所以 $S$ 的最大“美丽度”无限大。  

样例 $2$：$S=\texttt{ab}$ 时“美丽度”最大。  

样例 $3$：请注意 $S$ 不能为空。

```input1
3
a -5
ab 10
ba -20
```

```output1
Infinity
```

```input2
28
a -5
ab 10
ba -20
bb -20
bc -20
bd -20
be -20
bf -20
bg -20
bh -20
bi -20
bj -20
bk -20
bl -20
bm -20
bn -20
bo -20
bp -20
bq -20
br -20
bs -20
bt -20
bu -20
bv -20
bw -20
bx -20
by -20
bz -20
```

```output2
5
```

```input3
26
a -1
b -1
c -1
d -1
e -1
f -1
g -1
h -1
i -1
j -1
k -1
l -1
m -1
n -1
o -1
p -1
q -1
r -1
s -1
t -1
u -1
v -1
w -1
x -1
y -1
z -1
```

```output3
-1
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 18278 $
- $ N $ は整数
- $ T_i $ は英小文字のみからなる長さ $ 1 $ 以上 $ 3 $ 以下の文字列
- $ i\ \neq\ j\ \Rightarrow\ T_i\ \neq\ T_j $
- $ -10^9\ \leq\ P_i\ \leq\ 10^9 $
- $ P_i $ は整数

### Sample Explanation 1

例えば、$ S\ = $ `abzabz` について、 - $ 1 $ 番目の審査項目の点数は、`a` が $ S $ に連続な部分列として含まれる回数が $ 2 $ 回であることから、$ 2\ \times\ (-5)\ =\ -10 $ 点 - $ 2 $ 番目の審査項目の点数は、`ab` が $ S $ に連続な部分列として含まれる回数が $ 2 $ 回であることから、$ 2\ \times\ 10\ =\ 20 $ 点 - $ 3 $ 番目の審査項目の点数は、`ba` が $ S $ に連続な部分列として含まれる回数が $ 0 $ 回であることから、$ 0\ \times\ (-20)\ =\ 0 $ 点 であるので、$ S $ の美しさは $ (-10)\ +\ 20\ +\ 0\ =\ 10 $ となります。 別の例として、$ S\ = $ `abzabzabz` について、 - $ 1 $ 番目の審査項目の点数は、`a` が $ S $ に連続な部分列として含まれる回数が $ 3 $ 回であることから、$ 3\ \times\ (-5)\ =\ -15 $ 点 - $ 2 $ 番目の審査項目の点数は、`ab` が $ S $ に連続な部分列として含まれる回数が $ 3 $ 回であることから、$ 3\ \times\ 10\ =\ 30 $ 点 - $ 3 $ 番目の審査項目の点数は、`ba` が $ S $ に連続な部分列として含まれる回数が $ 0 $ 回であることから、$ 0\ \times\ (-20)\ =\ 0 $ 点 であるので、$ S $ の美しさは $ (-15)\ +\ 30\ +\ 0\ =\ 15 $ となります。 一般に、正の整数 $ X $ について、`abz` を $ X $ 回繰り返した文字列の美しさは $ 5X $ となります。 $ S $ の美しさとしていくらでも大きい値が考えられるため、`Infinity` を出力します。

### Sample Explanation 2

$ S\ = $ `ab` が考えられる美しさの最大値を達成します。

### Sample Explanation 3

$ S $ は空でない文字列でなければならないことに注意して下さい。

