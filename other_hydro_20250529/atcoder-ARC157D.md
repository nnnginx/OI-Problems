## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc157/tasks/arc157_d

$ H $ 佩 $ W $ 双のマス朕の光マスに `X`, `Y` のいずれかの猟忖が��かれています�� 貧から $ i $ 佩朕��恣から $ j $ 双朕のマスを $ (i,\ j) $ で燕します�� マス朕に��かれている猟忖は $ H $ ��の猟忖双 $ S_1,\ S_2,\ \dots,\ S_H $ によって嚥えられ��$ S_i $ の $ j $ 猟忖朕がマス $ (i,\ j) $ に��かれた猟忖を燕します��

�Oり栽う光佩および光双の�gに��マス朕畠悶を罪僅�┸k僅��するように�鼎鰓O崔できます�� �斗�平は住餓しても��いません�� �鼎淋O崔瘁に��仝あるマスから兵めて貧和恣嘔に�O俊するマスへの卞�咾鮴Rり卦すことで���鼎鰓修┐困傍淳_辛嬬なマス畠悶々を**曝鮫**と協�xします�� �┳�薦箭 1 の�h苧も歌深にしてください����

�鼎淋O崔圭隈は畠何で $ 2^{H-1}\ \times\ 2^{W-1} $ 宥りありますが��そのうち肝の訳周を�困燭垢發里���方を $ 998244353 $ で護った噫りを箔めてください��

**訳周:** 光曝鮫には `Y` が��かれたマスがちょうど $ 2 $ ��根まれている��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる��

> $ H $ $ W $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_H $

## 補竃鯉塀
訳周を�困燭��鼎淋O崔圭隈の�t方を $ 998244353 $ で護った噫りを竃薦せよ��

## 籾朕寄吭
Feyn 嗤匯倖 $H$ 佩 $W$ 双議裳專��裳專戦中議圷殆譲葎忖憲 $X$ 賜 $Y$。Feyn �誨�壓裳專嶄慧匯乂佞生��佞生勣担慧壓罪彭議曾佩岻寂��勣担慧壓抱彭議曾双岻寂��駅倬慧頼屁佩賜屁双。否叟岑祇��壓音�渣噸だ己�楚議念戻和��嗤 $2^{H-1}\times 2^{W-1}$ 嶽慧佞生議圭宛。Feyn 嗤匯乂蒙歩議餘挫�宰�錬李佞生蛍護竃議耽倖銭宥翠坪��脅嗤**如挫**曾倖忖憲 $Y$。萩補竃貧峰侭嗤圭宛嶄憲栽訳周議圭宛方��斤 $998244353$ 函庁。

(translated by 342873)

```input1
2 3
XYY
YXY
```

```output1
2
```

```input2
2 3
XYX
YYY
```

```output2
0
```

```input3
2 58
YXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXY
YXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXYXXY
```

```output3
164036797
```

## 戻幣
### 崙�s

- $ 1\ \leq\ H\ \leq\ 2000 $
- $ 1\ \leq\ W\ \leq\ 2000 $
- $ S_i\ (1\ \leq\ i\ \leq\ H) $ は `X`, `Y` からなる�Lさ $ W $ の猟忖双である��
 
### Sample Explanation 1

�鼎淋O崔圭隈として��參和の $ 8 $ 宥りがあります�� ``` X Y Y X|Y Y X Y|Y X|Y|Y | | | | Y X Y Y|X Y Y X|Y Y|X|Y X Y Y X|Y Y X Y|Y X|Y|Y ----- -+--- ---+- -+-+- Y X Y Y|X Y Y X|Y Y|X|Y ``` たとえば��$ 2,\ 3 $ 双朕の�gに�鼎鰓O崔した��栽��曝鮫は ``` XY YX ``` ``` Y Y ``` であり��それぞれにちょうど $ 2 $ ��の `Y` が根まれているので��訳周を�困燭靴泙坑� また��$ 1,\ 2 $ 佩朕の�gと $ 1,\ 2 $ 双朕の�gに�鼎鰓O崔した��栽��曝鮫は ``` X ``` ``` YY ``` ``` Y ``` ``` XY ``` となり��$ 2 $ つ朕の曝鮫參翌にはちょうど $ 2 $ ��の `Y` が根まれていないので��訳周を�困燭靴泙擦鵤�

### Sample Explanation 2

どのように�鼎鰓O崔しても訳周を�困燭靴泙擦鵤�

### Sample Explanation 3

訳周を�困燭��鼎淋O崔圭隈の�t方を $ 998244353 $ で護った噫りを竃薦してください��

