## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc127/tasks/arc127_b

屁方 $ N,L $ が嚥えられます�� 參和の訳周をすべて�困燭� $ 3N $ ��の猟忖双の�M $ (S_1,S_2,\cdots,S_{3N}) $ を匯つ箔めてください��

- $ S_i $ は `0`, `1`, `2` からなる�Lさ $ L $ の猟忖双である��
- $ S_i $ はすべて札いに��なる��
- すべての $ j $ ($ 1\ \leq\ j\ \leq\ L $) および $ c= $`0`, `1`, `2` について��肝が撹り羨つ��
  
  
  - $ S_i $ のうち��$ j $ 猟忖朕が $ c $ であるようなものはちょうど $ N $ ��贋壓する��
- $ S_1,S_2,\cdots,S_{3N} $ の嶄で��看����で恷も寄きい猟忖双を $ t $ で燕すことにする�� このときの $ t $ は��$ t $ としてありうる猟忖双の嶄で看����恷弌の猟忖双である��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる��

> $ N $ $ L $

## 補竃鯉塀
參和の侘塀で基えを竃薦せよ��

> $ S_1 $ $ S_2 $ $ \vdots $ $ S_{3N} $

なお��訳周を�困燭構發��}方贋壓する��栽��どれを竃薦しても屎盾とみなされる��

## 籾朕寄吭
公協 $N$ 才 $L$��低勣更夛 $3\times N$ 倖海業葎 $L$ 議堪��諾怎參和勣箔。

- 更夛議堪曾曾音揖。

- 斤噐侭嗤忖憲堪議耽匯了��$0$,$1$,$2$ 光竃�崛� $N$ 肝。

- 忖灸會恷寄議堪忖灸會恷弌。

```input1
2 2
```

```output1
00
02
11
12
20
21
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 5\ \times\ 10^4 $
- $ 1\ \leq\ L\ \leq\ 15 $
- $ 3N\ \leq\ 3^L $
- 秘薦される�､呂垢戮噸�方である

### Sample Explanation 1

この竃薦箭はすべての訳周を�困燭靴討い泙坑� 箭えば��$ 2 $ 猟忖朕が `0` であるような猟忖双は $ 2 $ ��贋壓しています�� また��この箭では $ t= $`21` ですが��$ t $ がこれより看����で弌さくなることはありません��

