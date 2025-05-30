## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_i

$ N $ を屎の謎方とします。

$ N $ 旦のコインがあります。 コインには $ 1,\ 2,\ \ldots,\ N $ と桑催が尅られています。 光 $ i $ ($ 1\ \leq\ i\ \leq\ N $) について、コイン $ i $ を誘げると、�_楕 $ p_i $ で燕が竃て、�_楕 $ 1\ -\ p_i $ で�Yが竃ます。

湊隻埴は $ N $ 旦のコインをすべて誘げました。 このとき、燕の��方が�Yの��方を貧指る�_楕を箔めてください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ p_1 $ $ p_2 $ $ \ldots $ $ p_N $

## 補竃鯉塀
燕の��方が�Yの��方を貧指る�_楕を竃薦せよ。 �~���`餓が $ 10^{-9} $ 參和ならば屎盾となる。

## 籾朕寄吭
$N$ 旦啣衛��及 $i$ 旦啣衛嗤 $p_i$ 議古楕屎中劾貧��嗤 $1-p_i$ 議古楕郡中劾貧。  
飯頼侭嗤啣衛��箔**屎中劾貧議咢衛方曳郡中劾貧議咢衛方謹**議古楕。

```input1
3
0.30 0.60 0.80
```

```output1
0.612
```

```input2
1
0.50
```

```output2
0.5
```

```input3
5
0.42 0.01 0.42 0.99 0.42
```

```output3
0.3821815872
```

## 戻幣
### 崙�s

- $ N $ は謎方である。
- $ 1\ \leq\ N\ \leq\ 2999 $
- $ p_i $ は�g方であり、弌方及 $ 2 $ 了まで嚥えられる。
- $ 0\ <\ p_i\ <\ 1 $

### Sample Explanation 1

燕の��方が�Yの��方を貧指るような光ケ�`スの�_楕を��麻すると、肝のようになります。 - $ (コイン\ 1,\ コイン\ 2,\ コイン\ 3)\ =\ (燕,\ 燕,\ 燕) $ となる�_楕は、$ 0.3\ 〜\ 0.6\ 〜\ 0.8\ =\ 0.144 $ である。 - $ (コイン\ 1,\ コイン\ 2,\ コイン\ 3)\ =\ (�Y,\ 燕,\ 燕) $ となる�_楕は、$ 0.7\ 〜\ 0.6\ 〜\ 0.8\ =\ 0.336 $ である。 - $ (コイン\ 1,\ コイン\ 2,\ コイン\ 3)\ =\ (燕,\ �Y,\ 燕) $ となる�_楕は、$ 0.3\ 〜\ 0.4\ 〜\ 0.8\ =\ 0.096 $ である。 - $ (コイン\ 1,\ コイン\ 2,\ コイン\ 3)\ =\ (燕,\ 燕,\ �Y) $ となる�_楕は、$ 0.3\ 〜\ 0.6\ 〜\ 0.2\ =\ 0.036 $ である。 よって、燕の��方が�Yの��方を貧指る�_楕は、$ 0.144\ +\ 0.336\ +\ 0.096\ +\ 0.036\ =\ 0.612 $ です。

### Sample Explanation 2

箭えば、`0.500`, `0.500000001`, `0.499999999` などを竃薦しても屎盾となります。

