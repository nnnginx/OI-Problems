## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc064/tasks/arc064_c

$ x $$ y $ 平面があります。 すぬけ君は座標 $ (x_s,\ y_s) $ から座標 $ (x_t,\ y_t) $ まで移動しようとしています。 すぬけ君は好きな向きへ速さ $ 1 $ で動くことができます。 なお、すぬけ君は大きさのない点と見なすことにします。

平面上には $ N $ 個の円形のバリアが張ってあります。 $ i $ 番目のバリアは中心が $ (x_i,\ y_i) $ で半径が $ r_i $ です。 バリアは互いに重なっていたり、互いを含んでいたりすることがあります。

平面上の各座標について、その座標がどのバリアの内部にも含まれない場合、その座標には宇宙線が降り注いでいます。

すぬけ君は移動中にできるだけ宇宙線を浴びたくないので、宇宙線を浴びる時間が最小になるように移動します。 すぬけ君が移動中に宇宙線を浴びる時間の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ x_s $ $ y_s $ $ x_t $ $ y_t $ $ N $ $ x_1 $ $ y_1 $ $ r_1 $ $ x_2 $ $ y_2 $ $ r_2 $ $ : $ $ x_N $ $ y_N $ $ r_N $

## 输出格式
すぬけ君が移動中に宇宙線を浴びる時間の最小値を出力せよ。 絶対誤差または相対誤差が $ 10^{-9} $ 以下ならば正解となる。

## 题目大意
  这里有一个 $x,y$ 平面。一个小偷正打算从坐标 $(xs, ys)$ 移动到坐标 $(xt, yt)$。小偷能以每次 $1$ 个单位的速度朝着任意方向移动。小偷可以看作是没有大小的一个点。
  
  平面上有 $N$ 个圆形的障碍物。第 $i$ 个障碍物以 $(x_i, y_i)$ 为中心，$r_i$ 为半径。障碍物也许会互相重叠或互相包含。
  
  宇宙射线会倾泻在平面上的每个不含于任何障碍物内的坐标上。
  
  因为小偷在移动过程中想要尽可能少地暴露在宇宙射线之下，所以会以遭受最少宇宙射线的方式移动。请求出小偷在移动过程中暴露在宇宙射线之下的最短时间。

```input1
-2 -2 2 2
1
0 0 1
```

```output1
3.6568542495
```

```input2
-2 0 2 0
2
-1 0 2
1 0 2
```

```output2
0.0000000000
```

```input3
4 -2 -2 4
3
0 0 2
4 0 1
0 4 1
```

```output3
4.0000000000
```

## 提示
### 制約

- 入力はすべて整数である。
- $ -10^9\ <\ =\ x_s,\ y_s,\ x_t,\ y_t\ <\ =\ 10^9 $
- $ (x_s,\ y_s) $ ≠ $ (x_t,\ y_t) $
- $ 1\ <\ =N\ <\ =1,000 $
- $ -10^9\ <\ =\ x_i,\ y_i\ <\ =\ 10^9 $
- $ 1\ <\ =\ r_i\ <\ =\ 10^9 $

### Sample Explanation 1

たとえば、図のように移動すればよいです。 !\[e9c630751968b7051df5750b7ddc0e07.png\](https://atcoder.jp/img/arc064/e9c630751968b7051df5750b7ddc0e07.png)

### Sample Explanation 2

たとえば、図のように移動すればよいです。 !\[fb82f6f4df5b22cffb868ce6333277aa.png\](https://atcoder.jp/img/arc064/fb82f6f4df5b22cffb868ce6333277aa.png)

### Sample Explanation 3

たとえば、図のように移動すればよいです。 !\[d09006720c225cbe69eae3fd9c186e67.png\](https://atcoder.jp/img/arc064/d09006720c225cbe69eae3fd9c186e67.png)

