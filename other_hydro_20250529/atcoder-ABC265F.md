## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc265/tasks/abc265_f

$ N $ 次元空間上の $ 2 $ 点 $ x=(x_1,\ x_2,\ \dots,\ x_N) $, $ y\ =\ (y_1,\ y_2,\ \dots,\ y_N) $ のマンハッタン距離 $ d(x,y) $ は次の式で定義されます。

$ \displaystyle\ d(x,y)=\sum_{i=1}^n\ \vert\ x_i\ -\ y_i\ \vert $ 

また、座標成分 $ x_1,\ x_2,\ \dots,\ x_N $ がすべて整数であるような点 $ x=(x_1,\ x_2,\ \dots,\ x_N) $ を格子点と呼びます。

$ N $ 次元空間上の格子点 $ p=(p_1,\ p_2,\ \dots,\ p_N) $, $ q\ =\ (q_1,\ q_2,\ \dots,\ q_N) $ が与えられます。  
$ d(p,r)\ \leq\ D $ かつ $ d(q,r)\ \leq\ D $ であるような格子点 $ r $ としてあり得るものは全部で何個ありますか？答えを $ 998244353 $ で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ D $ $ p_1 $ $ p_2 $ $ \dots $ $ p_N $ $ q_1 $ $ q_2 $ $ \dots $ $ q_N $

## 输出格式
答えを出力せよ。

## 题目大意
在 $n$ 维空间内我们定义两个点 $x(x_1,x_2,\ldots,x_n)$，$y(y_1,y_2,\ldots,y_n)$ 的**曼哈顿距离**为

$$d(x,y)=\sum_{i=1}^n|x_i-y_i|$$

如果一个点 $x$ 的所有坐标均为整数，我们称其为整点。

给出 $n$ 维空间内两个整点 $p,q$ 和一个整数 $D$，求有多少个整点 $r$ 有 $d(p,r)\le D,d(q,r)\le D$。

由于答案可能过大，你需要将答案对 $998244353$ 求余。

```input1
1 5
0
3
```

```output1
8
```

```input2
3 10
2 6 5
2 1 2
```

```output2
632
```

```input3
10 100
3 1 4 1 5 9 2 6 5 3
2 7 1 8 2 8 1 8 2 8
```

```output3
145428186
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 0\ \leq\ D\ \leq\ 1000 $
- $ -1000\ \leq\ p_i,\ q_i\ \leq\ 1000 $
- 入力される値はすべて整数

### Sample Explanation 1

$ N=1 $ の場合は $ 1 $ 次元空間、すなわち数直線上の点に関する問題になります。 条件を満たす点は $ -2,-1,0,1,2,3,4,5 $ の $ 8 $ 個です。

