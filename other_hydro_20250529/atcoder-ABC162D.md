## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_d

`R`, `G`, `B` のみからなる、�Lさ $ N $ の猟忖双 $ S $ があります。

參和の $ 2 $ つの訳周をともに�困燭構M $ (i,~j,~k)~(1\ \leq\ i\ <\ j\ <\ k\ \leq\ N) $ の方を箔めてください。

- $ S_i\ \neq\ S_j $ かつ $ S_i\ \neq\ S_k $ かつ $ S_j\ \neq\ S_k $ である
- $ j\ -\ i\ \neq\ k\ -\ j $ である

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ S $

## 補竃鯉塀
�}吭を�困燭構Mの方を竃薦せよ。

## 籾朕寄吭
公低匯倖叙喇 $R$��$G$��$B$ 眉嶽忖憲怏撹議忖憲堪��低俶勣孀欺侭嗤諾怎勣箔議眉圷怏 $(i,j,k)$。凪嶄 $S_i \ne S_j$��$S_j \ne S_k$��$S_i \ne S_k$��$j-i \ne k-j$��$1 \le i < j < k \le N$。凪嶄 $N$ 頁峺 $S$ 嶄忖憲議倖方。補竃諾怎訳周議眉圷怏倖方。

```input1
4
RRGB
```

```output1
1
```

```input2
39
RBRBGRBGGBBRRGBBRRRBGGBRBGBRBGBRBBBGBBB
```

```output2
1800
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 4000 $
- $ S $ は `R`, `G`, `B` のみからなる、�Lさ $ N $ の猟忖双である

### Sample Explanation 1

�M $ (1,~3,~4) $ だけが $ 2 $ つの訳周をともに�困燭靴泙后��M $ (2,~3,~4) $ は、$ 1 $ つ朕の訳周は�困燭靴泙垢� $ 2 $ つ朕の訳周を�困燭気覆い里撚止mです。

