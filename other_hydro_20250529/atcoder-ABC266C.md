## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc266/tasks/abc266_c

$ 2 $ 次元座標平面があります。$ x $ 軸正方向を右向き、$ y $ 軸正方向を上向きとします。

この平面上に自己交差のない四角形があります。  
 $ 4 $ つの頂点の座標は反時計回りに $ (A_x,A_y),(B_x,B_y),(C_x,C_y),(D_x,D_y) $ です。

この四角形が凸であるか判定してください。

なお、四角形の $ 4 $ つの内角が全て $ 180 $ 度未満であるとき、かつ、その時に限り、その四角形は凸であるといいます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A_x $ $ A_y $ $ B_x $ $ B_y $ $ C_x $ $ C_y $ $ D_x $ $ D_y $

## 输出格式
与えられる四角形が凸なら `Yes`、凸でないなら `No` を出力せよ。

## 题目大意
输入平面直角坐标系内四个点 $A,B,C,D$ 的坐标，判断四边形 $ABCD$ （四条边分别为 $AB,BC,CD,DA$）是否为凸四边形。

题目保证两组对边（指这两条线段）均不相交。

```input1
0 0
1 0
1 1
0 1
```

```output1
Yes
```

```input2
0 0
1 1
-1 0
1 -1
```

```output2
No
```

## 提示
### 制約

- $ -100\ \leq\ A_x,A_y,B_x,B_y,C_x,C_y,D_x,D_y\ \leq\ 100 $
- 入力に含まれる値は全て整数である
- 与えられる $ 4 $ 点は四角形の $ 4 $ 頂点を反時計回りに並べたものである
- 与えられる $ 4 $ 点のなす四角形は自己交差がなく退化していない。すなわち
  - どの $ 2 $ 頂点も同じ座標にない
  - どの $ 3 $ 頂点も同一直線上にない
  - 隣接しない $ 2 $ 辺は共有点を持たない

### Sample Explanation 1

与えられた四角形は正方形であり、$ 4 $ つの内角は全て $ 90 $ 度です。したがって、この四角形は凸です。 !\[図\](https://img.atcoder.jp/abc266/cda66d9b9f4291781d1ce47f59f29ab0.png)

### Sample Explanation 2

角 $ A $ が $ 270 $ 度です。したがって、この四角形は凸ではありません。 !\[図\](https://img.atcoder.jp/abc266/2927f9f67e2cb7c35aeab05269b6fcc2.png)

