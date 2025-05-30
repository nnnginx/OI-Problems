## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc250/tasks/abc250_f

ABC250 は、 ABC1000 の開催を目指す高橋くんにとってちょうど $ 1/4 $ となる記念すべき回です。  
 そこで、高橋くんはピザを $ 1 $ 枚買ってきて、そのピザのうちなるべく $ 1/4 $ に近い分量を食べて祝うことにしました。

高橋くんが買ってきたピザは凸 $ N $ 角形 ($ N\ \ge\ 4 $) の平らな形をしており、このピザを $ xy $ 平面上に置いた際、 $ i $ 番目の頂点の座標は $ (X_i,Y_i) $ でした。

高橋くんは、このピザを以下のように切って食べることにしました。

- まず、高橋くんはピザの頂点のうち隣接しない $ 2 $ 頂点を選び、それらを通る直線に沿ってナイフを入れ、ピザを $ 2 $ つに切り分ける。
- その後、 $ 2 $ つのピースのうち好きなものをどちらか $ 1 $ つ選んで食べる。

高橋くんが買ってきたピザの面積の $ 1/4 $ を $ a $ 、高橋くんが食べるピースの面積を $ b $ とした時、 $ 8\ \times\ |a-b| $ としてありえる最小値を求めてください。なお、この値は常に整数となることが示せます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X_1 $ $ Y_1 $ $ X_2 $ $ Y_2 $ $ \dots $ $ X_N $ $ Y_N $

## 输出格式
答えを整数として出力せよ。

## 题目大意
给定凸包，逆时针给定凸包的每个顶点。你需要通过连结两个顶点将凸包划分为两部分并选择其中一个。令凸包面积为 $ a $，选定部分面积为 $ b $，需要最小化 $ 8 \times \lvert \dfrac{a}{4} - b \rvert $，求最小值。易证该值为整数。

```input1
5
3 0
2 3
-1 3
-3 1
-1 -1
```

```output1
1
```

```input2
4
400000000 400000000
-400000000 400000000
-400000000 -400000000
400000000 -400000000
```

```output2
1280000000000000000
```

```input3
6
-816 222
-801 -757
-165 -411
733 131
835 711
-374 979
```

```output3
157889
```

## 提示
### 制約

- 入力は全て整数
- $ 4\ \le\ N\ \le\ 10^5 $
- $ |X_i|,\ |Y_i|\ \le\ 4\ \times\ 10^8 $
- 入力される頂点は反時計回りに凸 $ N $ 角形をなす。

### Sample Explanation 1

$ 3 $ 番目の頂点と $ 5 $ 番目の頂点を通る直線に沿ってピザを切り分け、 $ 4 $ 番目の頂点を含む側のピースを食べたとします。 このとき、$ a=\frac{33}{2}\ \times\ \frac{1}{4}\ =\ \frac{33}{8} $ 、 $ b=4 $ 、 $ 8\ \times\ |a-b|=1 $ であり、これがありえる最小値です。

