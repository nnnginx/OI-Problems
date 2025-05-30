## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc268/tasks/abc268_f

`1` から `9` の方忖および `X` のみからなる $ N $ ��の猟忖双 $ S_1,\ S_2,\ \ldots,\ S_N $ が嚥えられます。

$ (1,\ 2,\ \ldots,\ N) $ を�Kべ紋えた双 $ P\ =\ (P_1,\ P_2,\ \ldots,\ P_N) $ を匯つ�xび、 猟忖双 $ T\ =\ S_{P_1}\ +\ S_{P_2}\ +\ \cdots\ +\ S_{P_N} $ を恬ります。ここで、$ + $ は猟忖双の�B�Yを燕します。

そして、猟忖双 $ T\ =\ T_1T_2\ldots\ T_{|T|} $ の仝スコア々を��麻します�� $ |T| $ は猟忖双 $ T $ の�Lさを燕します��。  
 $ T $ のスコアは、スコアが $ 0 $ の彜�Bから兵め、和��の $ 9 $ ��の返��を佩うことで��麻されます。

- $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `1` を�困燭衡�方の�M $ (i,\ j) $ の��方だけ、スコアを $ 1 $ 泣紗麻する 。
- $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `2` を�困燭衡�方の�M $ (i,\ j) $ の��方だけ、スコアを $ 2 $ 泣紗麻する。
- $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `3` を�困燭衡�方の�M $ (i,\ j) $ の��方だけ、スコアを $ 3 $ 泣紗麻する。
- $ \cdots $
- $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `9` を�困燭衡�方の�M $ (i,\ j) $ の��方だけ、スコアを $ 9 $ 泣紗麻する。

$ P $ を販吭に�xぶときの、$ T $ のスコアとしてあり誼る恷寄�､魍�薦してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 補竃鯉塀
基えを竃薦せよ。

## 籾朕寄吭
公協 $ n $ 倖喇 `X` 才方忖更撹議忖憲堪��低俶勣斤凪序佩電双旺憧俊撹仟議忖憲堪 $ T $ 參恷寄晒凪蛍方。協吶凪蛍方葎斤噐忖憲堪嶄耽匯倖方忖��聞方忖斤哘議方峙核貧凪岻念 `X` 議方楚��旺箔才。補竃蛍方恷寄峙。

```input1
3
1X3
59
XXX
```

```output1
71
```

```input2
10
X63X395XX
X2XX3X22X
13
3716XXX6
45X
X6XX
9238
281X92
1XX4X4XX6
54X9X711X1
```

```output2
3010
```

## 戻幣
### 崙�s

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ N $ は屁方
- $ S_i $ は `1` から `9` の方忖および `X` のみからなる�Lさ $ 1 $ 參貧の猟忖双
- $ S_1,\ S_2,\ \ldots,\ S_N $ の�Lさの�t才は $ 2\ \times\ 10^5 $ 參和

### Sample Explanation 1

$ P\ =\ (3,\ 1,\ 2) $ とすると、$ T\ =\ S_3\ +\ S_1\ +\ S_2\ = $ `XXX1X359` です。 このとき、$ T $ のスコアは肝の宥り��麻されます。 - $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `1` を�困燭衡�方の�M $ (i,\ j) $ が $ 3 $ ��あり、 - $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `3` を�困燭衡�方の�M $ (i,\ j) $ が $ 4 $ ��あり、 - $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `5` を�困燭衡�方の�M $ (i,\ j) $ が $ 4 $ ��あり、 - $ 1\ \leq\ i\ \lt\ j\ \leq\ |T| $ および $ T_i\ = $ `X` かつ $ T_j\ = $ `9` を�困燭衡�方の�M $ (i,\ j) $ が $ 4 $ ��あります。 よって、$ T $ のスコアは $ 1\ \times\ 3\ +\ 3\ \times\ 4\ +\ 5\ \times\ 4\ +\ 9\ \times\ 4\ =\ 71 $ であり、これが深えられる恷寄�､任后�

