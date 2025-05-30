## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc144/tasks/arc144_c

屎屁方 $ N,\ K $ が嚥えられます�� $ 1 $ から $ N $ までの屁方からなる��双 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_N) $ であって肝の訳周を�困燭垢發里里Δ腺� 看����恷弌のものを箔めてください��

- 販吭の $ i $ ($ 1\leq\ i\leq\ N $) に��して $ \lvert\ A_i\ -\ i\rvert\ \geq\ K $ が撹り羨つ��

そのような��双が贋壓しない��栽には��`-1` を竃薦してください��

 方双の看����とは�� �牀�なる方双 $ S $ と方双 $ T $ の寄弌を登協するアルゴリズムを參和に�h苧します��

參和では $ S $ の $ i $ 桑朕の勣殆を $ S_i $ のように燕します��また�� $ S $ が $ T $ より看����で弌さい��栽は $ S\ \lt\ T $ ��寄きい��栽は $ S\ \gt\ T $ と燕します��

1. $ S $ と $ T $ のうち�Lさが玉い圭の猟忖双の�Lさを $ L $ とします��$ i=1,2,\dots,L $ に��して $ S_i $ と $ T_i $ が匯崑するか�{べます��
2. $ S_i\ \neq\ T_i $ である $ i $ が贋壓する��栽��そのような $ i $ のうち恷弌のものを $ j $ とします��そして��$ S_j $ と $ T_j $ を曳�^して�� $ S_j $ が $ T_j $ より��方として��弌さい��栽は $ S\ \lt\ T $ ��寄きい��栽は $ S\ \gt\ T $ と�Q協して��アルゴリズムを�K阻します��
3. $ S_i\ \neq\ T_i $ である $ i $ が贋壓しない��栽�� $ S $ と $ T $ の�Lさを曳�^して��$ S $ が $ T $ より玉い��栽は $ S\ \lt\ T $ ���Lい��栽は $ S\ \gt\ T $ と�Q協して��アルゴリズムを�K阻します��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられます��

> $ N $ $ K $

## 補竃鯉塀
訳周を�困燭麹�双 $ A $ のうち��看����恷弌のものを肝の侘塀で竃薦してください��

> $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

そのような��双が贋壓しない��栽には��`-1` を竃薦してください��

## 籾朕寄吭
- 箔忖灸會恷弌議 $1\sim n$ 議電双 $p$ 諾怎 $\left|p_i-i\right|\geq k$��涙盾補竃 $-1$。
- $2\leq n\leq 3\times 10^5$��$1\leq p<n$。

```input1
3 1
```

```output1
2 3 1
```

```input2
8 3
```

```output2
4 5 6 7 8 1 2 3
```

```input3
8 6
```

```output3
-1
```

## 戻幣
### 崙�s

- $ 2\leq\ N\leq\ 3\times\ 10^5 $
- $ 1\leq\ K\leq\ N\ -\ 1 $

### Sample Explanation 1

訳周を�困燭麹�双は��$ (2,\ 3,\ 1) $ と $ (3,\ 1,\ 2) $ の $ 2 $ つです��箭えば $ (2,\ 3,\ 1) $ は - $ \lvert\ A_1\ -\ 1\rvert\ =\ 1\ \geq\ K $ - $ \lvert\ A_2\ -\ 2\rvert\ =\ 1\ \geq\ K $ - $ \lvert\ A_3\ -\ 3\rvert\ =\ 2\ \geq\ K $ であるため訳周を�困燭靴討い泙坑�

