## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc157/tasks/arc157_c

$ H $ 佩 $ W $ 双のマス朕の光マスに `X`, `Y` のいずれかの猟忖が��かれています�� 貧から $ i $ 佩朕��恣から $ j $ 双朕のマスを $ (i,\ j) $ で燕します�� マス朕に��かれている猟忖は $ H $ ��の猟忖双 $ S_1,\ S_2,\ \dots,\ S_H $ によって嚥えられ��$ S_i $ の $ j $ 猟忖朕がマス $ (i,\ j) $ に��かれた猟忖を燕します��

和または嘔に�O俊するマスへの卞�咾鮴Rり卦してマス $ (1,\ 1) $ からマス $ (H,\ W) $ に崛る�U揃 $ P $ に��して��

- 仝 $ P $ で宥るマスに��かれた猟忖を��に�Kべて誼られる�Lさ $ (H\ +\ W\ -\ 1) $ の猟忖双々を $ \mathrm{str}(P) $ とし��
- 仝 $ \mathrm{str}(P) $ 嶄で `Y` 揖平が�Oり栽う�w侭の**��方の $ 2 $ �\**々を $ P $ の**スコア**と協�xします��
 
そのような�U揃 $ P $ としてあり誼るものは $ \displaystyle\binom{H\ +\ W\ -\ 2}{H\ -\ 1} $ 宥りありますが��その畠てに��するスコアの�t才を $ 998244353 $ で護った噫りを箔めてください��

  $ \binom{N}{K} $ の吭龍 $ \displaystyle\binom{N}{K} $ は��$ N $ ��の�牀�なる勣殆から $ K $ ��を�xぶ��栽の方を燕す屈���S方です��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる��

> $ H $ $ W $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_H $

## 補竃鯉塀
あり誼る�U揃畠てに��するスコアの�t才を $ 998244353 $ で護った噫りを竃薦せよ��

## 籾朕寄吭
公協 $H \times W$ 議裳專��耽倖了崔貧嗤匯倖忖憲��頁 `X` 賜 `Y`。

協吶匯訳揃抄議幡峙葎��繍凪将狛議忖憲梓乏會憧俊撹匯倖忖憲堪��`YY` 壓宸倖忖憲堪議竃�峇諒�。

勣箔耽肝峪嬬�鰉匯鯱鯱戴滷�箔��侭嗤議 $\binom{H + W - 2}{H - 1}$ 訳恣貧欺嘔和議揃抄��万断幡峙峠圭議才。

```input1
2 2
YY
XY
```

```output1
4
```

```input2
2 2
XY
YY
```

```output2
2
```

```input3
10 20
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
```

```output3
423787835
```

## 戻幣
### 崙�s

- $ 1\ \leq\ H\ \leq\ 2000 $
- $ 1\ \leq\ W\ \leq\ 2000 $
- $ S_i\ (1\ \leq\ i\ \leq\ H) $ は `X`, `Y` からなる�Lさ $ W $ の猟忖双である��
 
### Sample Explanation 1

�U揃 $ P $ としてあり誼るものは $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2) $ と $ (1,\ 1)\ \to\ (2,\ 1)\ \to\ (2,\ 2) $ の $ 2 $ 宥りです�� - $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2) $ の��栽��$ \mathrm{str}(P)\ =\ {} $`YYY` であり��$ 1,\ 2 $ 猟忖朕と $ 2,\ 3 $ 猟忖朕の $ 2 $ �w侭で `Y` 揖平が�Oり栽っているので��スコアは $ 2^2\ =\ 4 $ です�� - $ (1,\ 1)\ \to\ (2,\ 1)\ \to\ (2,\ 2) $ の��栽��$ \mathrm{str}(P)\ =\ {} $`YXY` であり��`Y` 揖平が�Oり栽う�w侭は�oいので��スコアは $ 0^2\ =\ 0 $ です�� したがって��箔める�t才は $ 4\ +\ 0\ =\ 4 $ となります��

### Sample Explanation 2

$ 2 $ 宥りのいずれの�U揃の��栽も $ \mathrm{str}(P)\ =\ {} $`XYY` であり��スコアは $ 1^2\ =\ 1 $ です��

### Sample Explanation 3

スコアの�t才を $ 998244353 $ で護った噫りを竃薦してください��

