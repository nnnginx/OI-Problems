## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc247/tasks/abc247_b

繁 $ 1 $, 繁 $ 2 $, $ \dots $ 繁 $ N $ の $ N $ 繁の繁がいます。繁 $ i $ の侖は $ s_i $、兆は $ t_i $ です。

$ N $ 繁の繁すべてにあだ兆をつけることを深えます。繁 $ i $ のあだ兆 $ a_i $ は參和の訳周を�困燭恒慴�があります。

- $ a_i $ は繁 $ i $ の侖あるいは兆と匯崑する。冱い�Qえると、$ a_i\ =\ s_i $ または $ a_i\ =\ t_i $ の富なくとも匯圭が撹り羨つ。
- $ a_i $ は徭蛍參翌の繁の侖および兆のどちらとも匯崑しない。冱い�Qえると、$ 1\ \leq\ j\ \leq\ N,\ i\ \neq\ j $ を�困燭垢垢戮討燐�方 $ j $ について $ a_i\ \neq\ s_j $ かつ $ a_i\ \neq\ t_j $ が撹り羨つ。

$ N $ 繁畠�Tに訳周を�困燭垢△醒�をつけることは辛嬬でしょうか。辛嬬ならば `Yes` を、そうでないならば `No` を竃薦してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ s_1 $ $ t_1 $ $ s_2 $ $ t_2 $ $ \vdots $ $ s_N $ $ t_N $

## 補竃鯉塀
$ N $ 繁すべてにあだ兆をつけることが辛嬬ならば `Yes` を、そうでないならば `No` を竃薦せよ。

## 籾朕寄吭
公協 $ n $ 倖繁議侖才兆��協吶匯倖繁議蠻各葎麿議侖賜兆��拝匯倖繁議蠻各音嬬嚥凪麿繁議侖賜兆嶷鹸��登僅公協議方象頁倦嬬葎耽倖繁杯協匯倖蠻各。辛佩補竃 `Yes`��郡岻補竃 `No`。

```input1
3
tanaka taro
tanaka jiro
suzuki hanako
```

```output1
Yes
```

```input2
3
aaa bbb
xxx aaa
bbb yyy
```

```output2
No
```

```input3
2
tanaka taro
tanaka taro
```

```output3
No
```

```input4
3
takahashi chokudai
aoki kensho
snu ke
```

```output4
Yes
```

## 戻幣
### 崙�s

- $ 2\ \leq\ N\ \leq\ 100 $
- $ N $ は屁方である。
- $ s_i,t_i $ は哂弌猟忖からなる $ 1 $ 猟忖參貧 $ 10 $ 猟忖參和の猟忖双である。

### Sample Explanation 1

$ a_1\ = $ `taro`, $ a_2\ = $ `jiro`, $ a_3\ = $ `hanako` とすれば、これは���}猟にあるあだ兆の訳周を�困燭靴討い泙后�($ a_3 $ は `suzuki` でもよいです。) ここで、$ a_1\ = $ `tanaka` とはできないことに廣吭してください。なぜならば 繁 $ 2 $ の侖 $ s_2 $ もまた `tanaka` であるため、あだ兆の訳周の $ 2 $ つ朕を�困燭気覆�なるからです。

### Sample Explanation 2

���}猟の訳周を�困燭垢△醒�のつけ圭は贋壓しません。

### Sample Explanation 3

揖侖揖兆である繁の�Mが贋壓する��栽もあります。

### Sample Explanation 4

$ a_1\ = $ `chokudai`, $ a_2\ = $ `kensho`, $ a_3\ = $ `ke` とすればよいです。

