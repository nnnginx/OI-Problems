## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc265/tasks/abc265_d

長さ $ N $ の数列 $ A=(A_0,\ldots,A_{N-1}) $ があります。  
次の条件を全て満たす整数の組 $ (x,y,z,w) $ が存在するか判定してください。

- $ 0\ \leq\ x\ <\ y\ <\ z\ <\ w\ \leq\ N $
- $ A_x\ +\ A_{x+1}\ +\ \ldots\ +\ A_{y-1}\ =\ P $
- $ A_y\ +\ A_{y+1}\ +\ \ldots\ +\ A_{z-1}\ =\ Q $
- $ A_z\ +\ A_{z+1}\ +\ \ldots\ +\ A_{w-1}\ =\ R $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ P $ $ Q $ $ R $ $ A_0 $ $ A_1 $ $ \ldots $ $ A_{N-1} $

## 输出格式
条件を満たす組が存在するなら `Yes`、存在しないなら `No` を出力せよ。

## 题目大意
有一个长度为 $N$ 的数列$A=(A_0,\ldots,A
_{N-1})$，

判断有满足以下所有条件的整数 $(x,y,z,w)$ 是否存在

+ $0\leq x < y < z < w \le N$
+ $A_x+A_{x+1}+\cdots+A_{y-1} = P$
+ $A_y+A_{y+1}+\cdots+A_{z-1}= Q$
+ $A_z+A_{z+1}+\cdots+A_{w-1}=R$

#### 数据范围：

- $3\le N \le 2 \times10^5$
- $1\le A_i \le 10^9$
- $1 \le P,Q,R \le 10^{15}$

```input1
10 5 7 5
1 3 2 2 2 3 1 4 3 2
```

```output1
Yes
```

```input2
9 100 101 100
31 41 59 26 53 58 97 93 23
```

```output2
No
```

```input3
7 1 1 1
1 1 1 1 1 1 1
```

```output3
Yes
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- $ 1\ \leq\ P,Q,R\ \leq\ 10^{15} $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

$ (x,y,z,w)=(1,3,6,8) $ が条件を満たします。

