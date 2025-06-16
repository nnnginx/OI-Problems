## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc198/tasks/abc198_c

$ 2 $ 次元平面上の原点に高橋君がいます。

高橋君が $ 1 $ 歩歩くと、いまいる点からのユークリッド距離がちょうど $ R $ であるような点に移動することができます(移動先の座標が整数である必要はありません)。これ以外の方法で移動することはできません。

高橋君が点 $ (X,Y) $ に到達するまでに必要な歩数の最小値を求めてください。

なお、点 $ (x_1,y_1) $ と点 $ (x_2,y_2) $ のユークリッド距離は $ \sqrt{(x_1-x_2)^2+(y_1-y_2)^2} $ で与えられます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ R $ $ X $ $ Y $

## 输出格式
高橋君が $ (X,Y) $ に到達するまでに必要な歩数の最小値を出力せよ。

## 题目大意
给定 $x,y$，输出 $ \sqrt{(x_1-x_2)^2+(y_1-y_2)^2} $。

> Translated by [Present_Coming_Time](https://www.luogu.com.cn/user/793625)。

```input1
5 15 0
```

```output1
3
```

```input2
5 11 0
```

```output2
3
```

```input3
3 4 4
```

```output3
2
```

## 提示
### 制約

- $ 1\ \leq\ R\ \leq\ 10^5 $
- $ 0\ \leq\ X,Y\ \leq\ 10^5 $
- $ (X,Y)\ \neq\ (0,0) $
- 入力は全て整数

### Sample Explanation 1

$ (0,0)\ \to\ (5,0)\ \to\ (10,0)\ \to\ (15,0) $ と $ 3 $ 歩で到達できます。 $ 2 $ 歩以下で到達することはできないのでこれが最小です。 !\[図1\](https://img.atcoder.jp/ghi/d34bbf4b43d8de5baf54bf589618c64e.png)

### Sample Explanation 2

例えば $ (0,0)\ \to\ (5,0)\ \to\ (8,4)\ \to\ (11,0) $ と移動すれば良いです。 !\[図2\](https://img.atcoder.jp/ghi/0932ca629f834af5124563f198bb3f9e.png)

### Sample Explanation 3

例えば $ (0,0)\ \to\ (2-\frac{\sqrt{2}}{2},\ 2+\frac{\sqrt{2}}{2})\ \to\ (4,4) $ と移動すれば良いです。 !\[図3\](https://img.atcoder.jp/ghi/50d67c401f9aceed8baa130918144597.png)

