## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc128/tasks/arc128_f

$ 1 $ から $ N $ までの桑催のついた $ N $ 旦のカ�`ドがあり��カ�`ド $ i $ には屁方 $ A_i $ が��かれています�� なお��$ N $ は甜方です��

すぬけくんとロボットがゲ�`ムをします�� ゲ�`ムは��參和のように�M佩します��

- ゲ�`ムマスタ�`が $ (1,2,\cdots,N) $ の��双 $ (p_1,p_2,\cdots,p_N) $ を傚冱する�� この��双はすぬけくんとロボット�I圭に岑らされる��
- その瘁��すぬけくんからはじめて���I宀が住札に返桑をプレイする�� 光返桑では參和のことが軟こる��
  - すぬけくんの返桑: 火っているカ�`ドの嶄から挫きなものを匯つ�xび��奮べる��
  - ロボットの返桑: 火っているカ�`ドのうち��$ p_i $ が恷寄となるカ�`ド $ i $ を�xび��伴やす��
- カ�`ドがなくなったらゲ�`ムは�K阻する��

恷�K議なゲ�`ムのスコアは��すぬけくんが奮べたカ�`ドに��かれた屁方の�t才です�� すぬけくんは��ゲ�`ムのスコアを恷寄晒するように恷�mな佩�咾鬚靴泙坑�

��双 $ p $ は $ N! $ 宥り深えられますが��これらすべてについてゲ�`ムのスコアを箔め��その�t才を $ 998244353 $ で護った噫りを箔めてください��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる��

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 補竃鯉塀
基えを竃薦せよ��

## 籾朕寄吭
公協 $n$ 倖方議會双 $a_{1\cdots n}$��低俶勣箔竃耽匯倖電双 $p_{1\cdots n}$ 議幡峙岻才庁 $998244353$ 議峙。

斤噐匯倖電双 $p_{1\cdots n}$��万議幡峙協吶泌和��

- 曾倖繁 Alice 才 Bob 態送螺嗄老��Alice 枠返。
- 壓 Alice 議指栽��慢辛參函恠會双嶄議匯倖方忖。
- 壓 Bob 議指栽��麿駅倬函恠輝念複和議侭嗤方忖嶄��$p_i$ 恷弌議 $a_i$。

幡峙葎 Alice 宥狛恷單貨待資誼議方忖岻才。

$1\le n\le 10^6$��$1\le a_i\le 10^9$。

```input1
2
1 2
```

```output1
4
```

```input2
4
1 100 10000 1000000
```

```output2
24200400
```

```input3
10
866111664 178537096 844917655 218662351 383133839 231371336 353498483 865935868 472381277 579910117
```

```output3
710984634
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 10^6 $
- $ N $ は甜方
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- 秘薦される�､呂垢戮噸�方である

### Sample Explanation 1

��双 $ p $ に卆らず��すぬけくんはカ�`ド $ 2 $ を奮べます��

### Sample Explanation 2

箭えば $ p=(3,1,4,2) $ であるとき��ゲ�`ムは參和のように�M佩します�� - すぬけくんがカ�`ド $ 3 $ を奮べる�� - ロボットがカ�`ド $ 1 $ を伴やす�� - すぬけくんがカ�`ド $ 4 $ を奮べる�� - ロボットがカ�`ド $ 2 $ を伴やす�� このとき��ゲ�`ムのスコアは $ 1010000 $ になります��

