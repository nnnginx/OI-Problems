## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc067/tasks/arc067_c

$ 1 $ から $ N $ までの桑催のついた $ N $ 繁の繁がいます。 參和の屈つの訳周を�困燭垢茲Δ法�泳らをいくつかのグル�`プに蛍けたいです。

- どのグル�`プも、そのグル�`プに根まれる繁方が $ A $ 繁參貧 $ B $ 繁參和である。
- ちょうど $ i $ 繁の繁が根まれるようなグル�`プの方を $ F_i $ で燕したとき、 すべての $ i $ について、$ F_i=0 $ または $ C�QF_i�QD $ が撹り羨っている。

このようなグル�`プ蛍けが採宥りあり誼るか箔めてください。 ただし、ある屈つのグル�`プ蛍けが��なるとは、屈繁の繁の�Mであって、 頭圭のグル�`プ蛍けでは揖じグル�`プに根まれ、麿圭では揖じグル�`プに根まれないようなものが贋壓することを吭龍します。 なお、基えは掲械に寄きくなることがあるので、$ 10^9+7 $ で護った噫りを竃薦してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ A $ $ B $ $ C $ $ D $

## 補竃鯉塀
あり誼るグル�`プ蛍けの��方を、$ 10^9+7 $ で護った噫りを竃薦せよ。

## 籾朕寄吭
嗤$N$倖繁��園催卆肝頁$1,2,\cdots ,N$, �嶬斷�繍麿断蛍撹飛孤怏��諾怎��

- 耽匯怏議繁方譲壓$[A,B]$岻寂。

- 芝$F_i$葎輝念蛍怏圭宛嶄繁方葎$i$議怏議方楚��夸$F_i$哘諾怎$F_i=0$賜$C\leq F_i\leq D$.

凪嶄$A,B,C,D$譲葎公協峙。

箔云嵎音揖議蛍怏圭宛方斤$10^9+7$函庁朔議潤惚。曾嶽圭宛頁云嵎音揖議輝拝叙輝贋壓曾倖繁聞誼壓及匯嶽圭宛嶄麿断壓揖匯怏��遇壓及屈嶽圭宛嶄音頁。

方象袈律��$1\leq N\leq 10^3,1\leq A\leq B\leq N,1\leq C\leq D\leq N$

```input1
3 1 3 1 2
```

```output1
4
```

```input2
7 2 3 1 3
```

```output2
105
```

```input3
1000 1 1000 1 1000
```

```output3
465231251
```

```input4
10 3 4 2 5
```

```output4
0
```

## 戻幣
### 崙�s

- $ 1�QN�Q10^3 $
- $ 1�QA�QB�QN $
- $ 1�QC�QD�QN $

### Sample Explanation 1

參和の $ 4 $ 宥りの蛍け圭があります。 - $ (1,2),(3) $ - $ (1,3),(2) $ - $ (2,3),(1) $ - $ (1,2,3) $ $ (1),(2),(3) $ のような蛍け圭は、匯つ朕の訳周は�困燭靴討い泙垢�、 屈つ朕の訳周を�困燭靴討い覆い燭瓩吠�えられません。

### Sample Explanation 2

$ 2 $ 繁グル�`プ、$ 2 $ 繁グル�`プ、$ 3 $ 繁グル�`プの眉つに蛍ける參翌に�m俳な蛍け圭はありません。 そして、このような蛍け圭は $ 105 $ 宥りあります。

### Sample Explanation 4

基えが $ 0 $ になることもあり誼ます。

