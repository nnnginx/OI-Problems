## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc268/tasks/abc268_h

猟忖双 $ S $ が嚥えられます。また、互�鮠�は肝の荷恬を $ 0 $ 指參貧佩うことが竃栖ます。

- $ 1\ \leq\ i\ \leq\ |S| $ なる屁方 $ i $ を�xび、$ S $ の $ i $ 猟忖朕を `*` に�笋┐襦�

互�鮠�の朕議は、$ S $ の**何蛍猟忖双として** $ N $ ��の猟忖双 $ T_1,T_2,\ldots,T_N $ がいずれも�Fれないようにすることです。  
 これを�_撹するために駅勣な荷恬の指方の恷弌�､鯒鵑瓩討�ださい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ S $ $ N $ $ T_1 $ $ T_2 $ $ \vdots $ $ T_N $

## 補竃鯉塀
基えを竃薦せよ。

## 籾朕寄吭
公協叙嗤哂猟弌亟忖銚議忖憲堪 $ S $��辛參斤凪序佩飛孤肝荷恬��耽肝繍 $ S $ 嶄蝶倖忖憲紋算葎 `*`。公協 $ n $ 倖叙嗤哂猟弌亟忖銚議庁塀堪��勣箔序佩荷恬聞誼 $ S $ 嶄音贋壓販吭徨堪嚥庁塀堪�猴�。恷弌晒荷恬肝方��補竃恷弌峙。

```input1
abcdefghijklmn
3
abcd
ijk
ghi
```

```output1
2
```

```input2
atcoderbeginnercontest
1
abc
```

```output2
0
```

```input3
aaaaaaaaa
2
aa
xyz
```

```output3
4
```

## 戻幣
### 崙�s

- $ 1\ \leq\ |S|\ \leq\ 5\ \times\ 10^5 $
- $ 1\ \leq\ N $
- $ N $ は屁方
- $ 1\ \leq\ |T_i| $
- $ \sum{|T_i|}\ \leq\ 5\ \times\ 10^5 $
- $ i\ \neq\ j $ ならば $ T_i\ \neq\ T_j $
- $ S,\ T_i $ は哂弌猟忖のみからなる猟忖双

### Sample Explanation 1

$ i $ として $ 1 $ と $ 9 $ を�xんで荷恬をすると $ S $ は `\*bcdefgh\*jklmn` となり、`abcd`、`ijk`、`ghi` がいずれも何蛍猟忖双として�Fれなくなります。

### Sample Explanation 2

荷恬をする駅勣がありません。

