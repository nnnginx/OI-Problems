## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc274/tasks/abc274_d

長さ $ N $ の正整数列 $ A\ =\ (A_1,\ A_2,\ \dots,\ A_N) $ および整数 $ x,\ y $ が与えられます。  
次の条件をすべて満たすように、$ xy $ 座標平面上に $ N+1 $ 個の点 $ p_1,\ p_2,\ \dots,\ p_N,\ p_{N+1} $ を配置することができるか判定してください。(同じ座標に $ 2 $ 個以上の点を配置してもよいです。)

- $ p_1\ =\ (0,\ 0) $
- $ p_2\ =\ (A_1,\ 0) $
- $ p_{N+1}\ =\ (x,\ y) $
- 点 $ p_i $ と点 $ p_{i+1} $ の距離は $ A_i $ ($ 1\ \leq\ i\ \leq\ N $)
- 線分 $ p_i\ p_{i+1} $ と線分 $ p_{i+1}\ p_{i+2} $ のなす角は $ 90 $ 度 ($ 1\ \leq\ i\ \leq\ N\ -\ 1 $)

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x $ $ y $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式
問題文の条件をすべて満たすように $ p_1,\ p_2,\ \dots,\ p_N,\ p_{N+1} $ を配置することができる場合は `Yes` を、そうでない場合は `No` を出力せよ。

## 题目大意
给你一个数列 $A = (A_1,A_2,...,A_n)$，和两个整数 $x,y$。

你需要在平面直角坐标系上放置 $N + 1$ 个点 $P_1,P_2,...,P_n$，满足以下要求：

- $P_1=(0,0)$。

- $P_2=(A_1,0)$。

- $P_{n+1}=(x,y)$。

- 对于 $i = 1,2,...,N$，满足 $P_i$ 和 $P_{i+1}$ 之间的距离为 $A_i$。

- 对于 $i = 1,2,...,N-1$，满足两条线段 $P_iP_{i+1}$ 和 $P_{i+1}P_{i+2}$ 互相垂直。

求有没有一种合法的放置方式。

```input1
3 -1 1
2 1 3
```

```output1
Yes
```

```input2
5 2 0
2 2 2 2 2
```

```output2
Yes
```

```input3
4 5 5
1 2 3 4
```

```output3
No
```

```input4
3 2 7
2 7 4
```

```output4
No
```

```input5
10 8 -7
6 10 4 1 5 9 8 6 5 1
```

```output5
Yes
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^3 $
- $ 1\ \leq\ A_i\ \leq\ 10 $
- $ |x|,\ |y|\ \leq\ 10^4 $
- 入力される値はすべて整数

### Sample Explanation 1

$ xy $ 座標平面に $ p_1\ =\ (0,\ 0),\ p_2\ =\ (2,\ 0),\ p_3\ =\ (2,\ 1),\ p_4\ =\ (-1,\ 1) $ として点を配置したのが以下の図です。これは問題文の条件をすべて満たしています。 !\[\](https://img.atcoder.jp/ghi/9e66a2e8cd081f011d3baba22dbe64fa.jpg)

### Sample Explanation 2

$ p_1\ =\ (0,\ 0),\ p_2\ =\ (2,\ 0),\ p_3\ =\ (2,\ 2),\ p_4\ =\ (0,\ 2),\ p_5\ =\ (0,\ 0),\ p_6\ =\ (2,\ 0) $ とすれば問題文の条件をすべて満たすことができます。同じ座標に複数の点を置いてもよいのに注意してください。

