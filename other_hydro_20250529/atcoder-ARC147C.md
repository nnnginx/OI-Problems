## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc147/tasks/arc147_c

$ 1,2,\ldots\ ,N $ の番号のついた $ N $ 人の人を数直線上に並べます。人 $ i\,(1\ \leq\ i\ \leq\ N) $ がいる地点の座標を $ x_i $ としたとき、 $ x_i $ は $ L_i $ 以上 $ R_i $ 以下の整数である必要があります。複数の人が同じ座標にいても構いません。

ここで、並べ方の**不満度**を以下の式で定義します。

> $ \displaystyle\sum_{i=1}^{N-1}\sum_{j=i+1}^{N}|x_j-x_i| $

不満度としてあり得る値の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ \vdots $ $ L_N $ $ R_N $

## 输出格式
答えを出力せよ。

## 题目大意
求 
$$
\sum^{n-1}_{i=1}\sum^{n}_{j=i+1}\left|x_j - x_i\right|
$$
其中 $l_i \leq x_i \leq r_i$

```input1
3
1 3
2 4
5 6
```

```output1
4
```

```input2
3
1 1
1 1
1 1
```

```output2
0
```

```input3
6
1 5
2 4
1 1
4 4
3 6
3 3
```

```output3
15
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 3\ \times\ 10^5 $
- $ 1\ \leq\ L_i\ \leq\ R_i\ \leq\ 10^7\ \,(1\ \leq\ i\ \leq\ N) $
- 入力はすべて整数

### Sample Explanation 1

$ x_1=3,x_2=4,x_3=5 $ とすると、不満度は $ 4 $ です。不満度を $ 3 $ 以下にすることはできないので、$ 4 $ を出力します。

