## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/dwacon6th-prelims/tasks/dwacon6th_prelims_c

$ N $ 繁の徨工たちがいます。徨工たちには $ 1,2,\ldots,N $ と桑催が尅られています。 これから $ K $ 晩�g、徨工たちにクッキ�`が塘られることになりました。 $ i $ 晩朕には $ N $ 繁の嶄から $ a_i $ 繁の徨工が吉�_楕で�xばれ、�xばれた徨工たちはそれぞれクッキ�`を $ 1 $ 旦鞭け函ります。($ K $ 指の徨工の�x�kはすべて鏡羨に佩われます。)

$ K $ 晩�gで徨工 $ i $ が鞭け函るクッキ�`の旦方を $ c_i $ として、徨工たちの *うれしさ* を $ c_1\ \times\ c_2\ \times\ \ldots\ \times\ c_N $ で協�xします。 うれしさの豚棋�､� $ \binom{N}{a_1}\ \times\ \binom{N}{a_2}\ \times\ \ldots\ \times\ \binom{N}{a_K} $ をかけた��(これは屁方となることが幣せます)を $ 10^9+7 $ で護ったあまりを箔めてください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ K $ $ a_1 $ $ a_2 $ $ \ldots $ $ a_K $

## 補竃鯉塀
基えを竃薦せよ。

## 籾朕寄吭
匯慌嗤 $N$ 倖繁��壓 $K$ 爺嶄議及 $i$ 爺昧字公 $a_i$ 倖繁窟匯翠往孤。$c_i$ 葎及 $i$ 倖繁壓 $k$ 爺嶄資誼議滅惚悳方。箔 $c_1 \times c_2 \times c_3 \cdots \times c_N \times \begin{pmatrix}N\\a_1\end{pmatrix} \times \begin{pmatrix}N\\a_2\end{pmatrix} \times \cdots \times \begin{pmatrix}N\\a_K\end{pmatrix}$ 議豚李峙 $\text{mod} \ 10^9+7$。

```input1
3 2
3 2
```

```output1
12
```

```input2
856 16
399 263 665 432 206 61 784 548 422 313 848 478 827 26 398 63
```

```output2
337587117
```

## 戻幣
### 廣��

$ \binom{n}{k} $ は��なる $ n $ ��の���鵑�ら $ k $ ��を�xぶ�xび圭の�t方を燕します。

### 崙�s

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ K\ \leq\ 20 $
- $ 1\ \leq\ a_i\ \leq\ N $

### Sample Explanation 1

\- $ 1 $ 晩朕では、徨工 $ 1,2,3 $ のいずれもクッキ�`を鞭け函ります。 - $ 2 $ 晩朕では、徨工 $ 1,2,3 $ のいずれか $ 1 $ 繁がクッキ�`を鞭け函りません。 - どの��栽もうれしさは $ 4 $ のため、うれしさの豚棋�､� $ 4 $ となります。これに $ \binom{3}{3}\ \times\ \binom{3}{2} $ をかけた�､任△� $ 12 $ を竃薦してください。

### Sample Explanation 2

\- 豚棋�､� $ \binom{N}{a_1}\ \times\ \binom{N}{a_2}\ \times\ \ldots\ \times\ \binom{N}{a_K} $ 蔚を $ 10^9+7 $ で護ったあまりを箔めてください。

