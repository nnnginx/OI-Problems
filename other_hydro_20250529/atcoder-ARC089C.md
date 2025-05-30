## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc089/tasks/arc089_c

シカのAtCoDeerくんは肝のような訳周を�困燭荒佻鬟哀薀佞鰉�しがっています。

- ��泣方$ N $は $ 300 $ 參和
- 徭失ル�`プや謹嶷�xがあってはいけない
- ��泣には $ 1 $ から $ N $ の桑催が原けられている
- 光�xには $ 0 $ 參貧 $ 100 $ 參和の屁方�､琳悗漾△發靴�は、`X` または `Y` というラベルが原けられている
- 畠ての $ 1\ <\ =\ x\ <\ =\ A $, $ 1\ <\ =\ y\ <\ =\ B $, を�困燭衡�方の�M $ (x,y) $ に��し、 ラベル `X` が原けられた�xの嶷みを $ x $ に、 `Y` が原けられた�xの嶷みを $ y $ に��き�Qえたグラフの ��泣 $ S $ から $ T $ への恷玉鉦�xは $ d_{x,y} $

AtCoDeerくんのためにこのようなグラフ(と $ S $ と $ T $ の�M)をひとつ��撹してください。訳周を�困燭好哀薀佞�贋壓しない��栽はそれを峺姜してください。 竃薦の圭隈については竃薦の�擇魏燐佞靴討�ださい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ A $ $ B $ $ d_{1,1} $ $ d_{1,2} $ $ .. $ $ d_{1,B} $ $ d_{2,1} $ $ d_{2,2} $ $ .. $ $ d_{2,B} $ $ : $ $ d_{A,1} $ $ d_{A,2} $ $ .. $ $ d_{A,B} $

## 補竃鯉塀
訳周を�困燭好哀薀佞�贋壓しない��栽は `Impossible` と竃薦せよ。

訳周を�困燭好哀薀佞�贋壓する��栽、 $ 1 $ 佩朕に `Possible` と竃薦せよ。 $ 2 $佩朕參週に ��撹したグラフを參和の侘塀で���奮�薦に竃薦せよ。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ c_1 $ $ u_2 $ $ v_2 $ $ c_2 $ : $ u_M $ $ v_M $ $ c_M $ $ S $ $ T $

ただし、 $ M $ は竃薦するグラフの�x方、 $ u_i,v_i,c_i $ はグラフの�xを燕す。 これは��泣 $ u_i $ から ��泣 $ v_i $ に 嶷み、あるいはラベル $ c_i $ の嗤�鰤xがあることを吭龍する。 秘竃薦箭も歌深にせよ。

## 籾朕寄吭
### 籾朕宙峰

公竃匯倖$A \times B$議裳專��凪嶄及$i$佩及$j$双圷殆葎$d_{i,j}$。編更夛匯倖嗤�鰺治�諾怎��

1、嗤�鰺宍稱�$\leq 300$��

2、夕嶄短嗤徭桟才嶷円��

3、夕嶄円嗤円幡��円幡葎 $[0,100]$ 嶄議屁方��賜宀頁隆岑方`X`賜`Y`��

4、斤噐侭嗤$x \in [1,A] , y \in[1,B]$��諾怎輝隆岑方$X = x$��$Y = y$扮��夕嶄$S$欺$T$議恷玉揃葎$d_{x,y}$。

### 補秘鯉塀

及匯佩曾倖屎屁方$A,B(1 \leq A , B \leq 10)$

俊和栖匯倖$A \times B$議裳專宙峰$d$。隠屬斤噐$\forall i \in [1,A] , j \in [1,B] , d_{i,j} \in [1,100]$

### 補竃鯉塀

泌惚音贋壓諾怎訳周議嗤�鰺治�補竃匯佩`Impossible`

倦夸及匯佩補竃`Possible`��及屈佩補竃嗤�鰺宍諜稱�$n$才円方$m$��俊和栖$m$佩耽佩補竃$u,v,x$宙峰匯訳貫$u$欺$v$、円幡葎$x$議嗤�魃滷�恷朔匯佩曾倖屎屁方$S,T$。

```input1
2 3
1 2 2
1 2 3
```

```output1
Possible
3 4
1 2 X
2 3 1
3 2 Y
1 3 Y
1 3
```

```input2
1 3
100 50 1
```

```output2
Impossible
```

## 戻幣
### 崙�s

- $ 1 $ $ <\ = $ $ A,B $ $ <\ = $ $ 10 $
- $ 1 $ $ <\ = $ $ d_{x,y} $ $ <\ = $ $ 100 $ ($ 1 $ $ <\ = $ $ x $ $ <\ = $ $ A $, $ 1 $ $ <\ = $ $ y $ $ <\ = $ $ B $)
- 秘薦は畠て屁方

