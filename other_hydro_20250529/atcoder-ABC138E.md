## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc138/tasks/abc138_e

哂弌猟忖からなる屈つの猟忖双 $ s,\ t $ が嚥えられます。肝の訳周を�困燭衡�方 $ i $ $ (1\ \leq\ i\ \leq\ 10^{100}\ \times\ |s|) $ が贋壓するか登協し、贋壓する��栽はそのような $ i $ の恷弌�､鯒鵑瓩討�ださい。

- $ s $ を $ 10^{100} $ ���B�Yして誼られる猟忖双を $ s' $ とする。$ t $ は、猟忖双 $ {s'}_1{s'}_2\ldots{s'}_i $ ($ s' $ の枠�^ $ i $ 猟忖) の何蛍双である。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ s $ $ t $

## 補竃鯉塀
訳周を�困燭衡�方 $ i $ が贋壓する��栽はそのような $ i $ の恷弌�､髻�贋壓しない��栽は `-1` を竃薦せよ。

## 籾朕寄吭
公協匯倖猟忖堪 $S$��才匯倖庁塀堪 $T$��繍 $S$ 嶷鹸 $10^{100}$ 肝圭��諒謄塘欺及叱倖忖憲扮胡挫繍 $T$ 謄塘頼��徨方双����飛嬬補竃謄塘頼撹議忖憲了崔��飛涙隈頼撹謄塘��補竃 $-1$。

```input1
contest
son
```

```output1
10
```

```input2
contest
programming
```

```output2
-1
```

```input3
contest
sentence
```

```output3
33
```

## 戻幣
### 廣��

- 猟忖双 $ a $ の何蛍双とは、$ a $ から $ 0 $ 猟忖參貧を��茅して火った猟忖を����議な��會を隠ったまま�B�Yして誼られる猟忖双です。箭えば、`contest` の何蛍双には `net`, `c`, `contest` などがあります。

### 崙�s

- $ 1\ \leq\ |s|\ \leq\ 10^5 $
- $ 1\ \leq\ |t|\ \leq\ 10^5 $
- $ s,\ t $ は哂弌猟忖からなる。

### Sample Explanation 1

$ t\ = $ `son` は猟忖双 `contestcon` ($ s'\ = $ `contestcontestcontest...` の枠�^ $ 10 $ 猟忖) の何蛍双であるため、$ i\ =\ 10 $ は訳周を�困燭靴泙后� 匯圭で、$ t $ は猟忖双 `contestco` ($ s' $ の枠�^ $ 9 $ 猟忖) の何蛍双ではないため、$ i\ =\ 9 $ は訳周を�困燭靴泙擦鵝� 揖��に、$ 8 $ 參和の販吭の屁方も訳周を�困燭靴泙擦鵝�よって、訳周を�困燭衡�方 $ i $ の恷弌�､� $ 10 $ です。

### Sample Explanation 2

$ t\ = $ `programming` は $ s'\ = $ `contestcontestcontest...` の何蛍双ではありません。よって、訳周を�困燭衡�方 $ i $ は贋壓しません。

### Sample Explanation 3

ここにそのようなケ�`スを崔くことはできませんが、基えは $ 32 $ bit 屁方に�Г泙蕕覆た苗榻圓�あるのでご廣吭ください。

