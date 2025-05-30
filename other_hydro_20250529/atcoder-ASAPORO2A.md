## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/cf17-tournament-round2-open/tasks/asaporo2_a

りんごさんは��泣に $ 1,2,...,N $ の桑催がついた $ N $ ��の��泣と $ 1,2,...,M $ の桑催がついた $ M $ 云の�xからなる�o�鬟哀薀� $ G $ を隔っています。 �x $ i $ は��泣 $ a_{i} $ と $ b_{i} $ を褒圭�鬚砲弔覆育Lさ $ w_i $ の�xです。

�F壓、りんごさんはこれらの $ N $ ��の��泣を $ 1,2,...,K $ の桑催がついた $ K $ �N��の弼で科弼している余嶄です。��泣 $ i $ は弼 $ c_i $ で�Tられています。ただし、$ c_i\ =\ 0 $ ならば��泣 $ i $ にはまだ弼が�Tられていません。

りんごさんはまだ弼が�Tられていない畠ての��泣を $ K $ �N��の弼のいずれかでそれぞれ�Tったのち、すぬけくんに $ G $ をあげます。

すぬけくんは $ G $ を聞って��泣に $ 1,2,...,K $ の桑催がついた $ K $ ��の��泣と $ M $ 云の�xからなる�o�鬟哀薀� $ G' $ を恬ります。 はじめ、$ G' $ には�xがありません。$ i $ 桑朕の�xは參和のようにして弖紗されます。

- $ G $ の�x $ i $ に彭朕したとき�I極の��泣に�Tられている弼をそれぞれ $ x,y $ とする
- ��泣 $ x $ と $ y $ を褒圭�鬚砲弔覆育Lさ $ w_i $ の�xを $ G' $ に弖紗する

$ G' $ の恷弌畠囃直に根まれる�xの�Lさの�t才としてありうる�､�恷弌でいくつになりますか�燭蠅鵑瓦気鵑�どのように弼を�Tっても $ G' $ が�B�Yにならない��栽は $ -1 $ を竃薦してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ M $ $ K $ $ c_1 $ $ c_2 $ $ ... $ $ c_{N} $ $ a_1 $ $ b_1 $ $ w_1 $ $ : $ $ a_M $ $ b_M $ $ w_M $

## 補竃鯉塀
基えを竃薦せよ。

```input1
4 3 3
1 0 1 2
1 2 10
2 3 20
2 4 50
```

```output1
60
```

```input2
5 2 4
0 0 0 0 0
1 2 10
2 3 10
```

```output2
-1
```

```input3
9 12 9
1 2 3 4 5 6 7 8 9
6 9 9
8 9 6
6 7 85
9 5 545631016
2 1 321545
1 6 33562944
7 3 84946329
9 7 15926167
4 7 53386480
5 8 70476
4 6 4549
4 8 8
```

```output3
118901402
```

```input4
18 37 12
5 0 4 10 8 7 2 10 6 0 9 12 12 11 11 11 0 1
17 1 1
11 16 7575
11 15 9
10 10 289938980
5 10 17376
18 4 1866625
8 11 959154208
18 13 200
16 13 2
2 7 982223
12 12 9331
13 12 8861390
14 13 743
2 10 162440
2 4 981849
7 9 1
14 17 2800
2 7 7225452
3 7 85
5 17 4
2 13 1
10 3 45
1 15 973
14 7 56553306
16 17 70476
7 18 9
9 13 27911
18 14 7788322
11 11 8925
9 13 654295
2 10 9
10 1 545631016
3 4 5
17 12 1929
2 11 57
1 5 4
1 17 7807368
```

```output4
171
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N,M\ \leq\ 10^{5} $
- $ 1\ \leq\ K\ \leq\ N $
- $ 0\ \leq\ c_i\ \leq\ K $
- $ 1\ \leq\ a_i,b_i\ \leq\ N $
- $ 1\ \leq\ w_i\ \leq\ 10^{9} $
- 嚥えられるグラフは�g��とも�B�Yとも�泙蕕覆�
- 嚥えられる秘薦は畠て屁方

### 何蛍泣

- $ 100 $ 泣蛍のデ�`タセットでは $ N=K,c_i\ =\ i $ が撹羨する
- �eの $ 100 $ 泣蛍のデ�`タセットでは $ c_i\ \neq\ 0 $ が撹羨する
- �eの $ 200 $ 泣蛍のデ�`タセットでは $ c_i\ =\ 0 $ が撹羨する

### Sample Explanation 1

��泣 $ 2 $ に弼 $ 3 $ を�Tったときのみ、$ G' $ が�B�Yになります。

### Sample Explanation 2

どのようにりんごさんが弼を�Tっても、$ 2 $ 云の�xで $ 4 $ つの��泣が�B�Yになるようにすることはできません。

