## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc287/tasks/abc287_d

哂弌猟忖と `?` からなる猟忖双 $ S,T $ が嚥えられます。ここで、$ |S|\ \gt\ |T| $ が撹り羨ちます(猟忖双 $ X $ に��し、 $ |X| $ で $ X $ の�Lさを燕します)。

また、$ |X|=|Y| $ を�困燭肯鍔崛� $ X,Y $ は、肝の訳周を�困燭垢箸�式びそのときに�泙�**マッチする**といいます。

- $ X,Y $ に根まれる `?` をそれぞれ鏡羨に挫きな哂弌猟忖に崔き�Qえることで $ X $ と $ Y $ を匯崑させることができる
 
$ x=0,1,\ldots,|T| $ に��して肝の���}を盾いてください。

- $ S $ の枠�^の $ x $ 猟忖と挑硫の $ |T|-x $ 猟忖を��桑を隠ったまま�B�Yすることで誼られる�Lさ $ |T| $ の猟忖双を $ S' $ とする。$ S' $ と $ T $ がマッチするならば `Yes` と、そうでなければ `No` と竃薦せよ。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ S $ $ T $

## 補竃鯉塀
$ |T|+1 $ 佩竃薦せよ。  
 $ i $ 佩朕には $ x=i-1 $ に��する竃薦をせよ。

## 籾朕寄吭
公協曾倖忖憲堪 $S$ 才 $T$��凪嶄 $|S|$ 燕幣忖憲堪 $S$ 議海業����斤噐 $x=0,1,...,|T|$ 卆肝箔盾泌和諒籾��

綜 $U$ 葎 $S$ 議念 $x$ 倖忖憲嚥恷朔 $|T|-x$ 倖忖憲怏撹議忖憲堪��頁倦贋壓匯嶽圭塀聞誼繍 $T$ 才 $U$ 嶄議耽匯倖 `?` 紋算撹販吭議弌亟忖銚聞誼 $T=U$�身膵�贋壓��補竃 `Yes`��倦夸補竃 `No`。

方象袈律��

斤噐 $100\%$ 議方象��$1\leq |T|<|S|\leq 3\times 10^5$��$S$ 才 $T$ 譲峪喇弌亟忖銚才 `?` 怏撹。

```input1
a?c
b?
```

```output1
Yes
No
No
```

```input2
atcoder
?????
```

```output2
Yes
Yes
Yes
Yes
Yes
Yes
```

```input3
beginner
contest
```

```output3
No
No
No
No
No
No
No
No
```

## 戻幣
### 崙�s

- $ S,T $ は哂弌猟忖と `?` からなる猟忖双
- $ 1\ \leq\ |T|\ \lt\ |S|\ \leq\ 3\ \times\ 10^5 $
 
### Sample Explanation 1

$ x=0 $ の��栽、$ S' $ は `?c` となります。ここで、$ S' $ の $ 1 $ 猟忖朕の `?` を `b` に、$ T $ の $ 2 $ 猟忖朕の `?` を `c` に崔き�Qえることで $ S' $ と $ T $ を匯崑させることができるため、$ S' $ と $ T $ はマッチします。このため、$ 1 $ 佩朕の竃薦は `Yes` です。 $ x=1,2 $ の��栽は $ S' $ はそれぞれ `ac`、`a?` であり、$ T $ とマッチしません。このため、$ 2,3 $ 佩朕の竃薦は `No` です。

