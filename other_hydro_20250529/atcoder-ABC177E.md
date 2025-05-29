## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_e

$ N $ 個の整数があります。$ i $ 番目の数は $ A_i $ です。

「全ての $ 1\leq\ i\ <\ j\ \leq\ N $ について、$ GCD(A_i,A_j)=1 $」が成り立つとき、$ \{A_i\} $ は pairwise coprime であるといいます。

$ \{A_i\} $ が pairwise coprime ではなく、かつ、$ GCD(A_1,\ldots,A_N)=1 $ であるとき、$ \{A_i\} $ は setwise coprime であるといいます。

$ \{A_i\} $ が pairwise coprime、setwise coprime、そのどちらでもない、のいずれであるか判定してください。

ただし $ GCD(\ldots) $ は最大公約数を表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式
$ \{A_i\} $ が pairwise coprime ならば `pairwise coprime`、setwise coprime ならば `setwise coprime`、そのどちらでもなければ `not coprime` と出力せよ。

## 题目大意
给一个长度为 $N$ 的数组 $A$ ，如果对于任意的 $1 \leq i < j \leq n, gcd(A_i,A_j)=1$就输出 `pairwise coprime`否则如果 $gcd(A_1,\ldots ,A_n)=1$,就输出`setwize coprome`否则输出`not coprime`

```input1
3
3 4 5
```

```output1
pairwise coprime
```

```input2
3
6 10 15
```

```output2
setwise coprime
```

```input3
3
6 10 16
```

```output3
not coprime
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ 1\ \leq\ A_i\leq\ 10^6 $

### Sample Explanation 1

$ GCD(3,4)=GCD(3,5)=GCD(4,5)=1 $ なので pairwise coprime です。

### Sample Explanation 2

$ GCD(6,10)=2 $ なので pairwise coprime ではありませんが、$ GCD(6,10,15)=1 $ なので setwise coprime です。

### Sample Explanation 3

$ GCD(6,10,16)=2 $ なので、pairwise coprime でも setwise coprime でもありません。

