## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/arc142/tasks/arc142_e

$ N $ 繁の徴隈聞いがいて、$ 1,\ \ldots\ ,N $ と桑催原けられています。  
 徴隈聞い $ i $ の��さは $ a_i $ です。また、徴隈聞い $ i $ は��さが $ b_i $ のモンスタ�`を宜そうとしています。

あなたは肝の荷恬を採業でも佩えます。

- 挫きな徴隈聞いを $ 1 $ 繁�xび、その��さを $ 1 $ ��やす。

また、徴隈聞い $ i $ と徴隈聞い $ j $ のペア (參週ペア $ (i,j) $ と柵ぶ) が**措いペア**であるとは、參和の訳周のうち富なくとも匯圭を�困燭垢海箸鰆犬靴泙后�

- 徴隈聞い $ i $ の��さが $ b_i $ 參貧かつ徴隈聞い $ j $ の��さが $ b_j $ 參貧
- 徴隈聞い $ i $ の��さが $ b_j $ 參貧かつ徴隈聞い $ j $ の��さが $ b_i $ 參貧

あなたの朕議は $ i=1,\ldots,\ M $ すべてに��し、ペア $ (x_i,y_i) $ が措いペアであるようにすることです。  
 朕議を�_撹するために駅勣な荷恬の指方の恷弌�､鯒鵑瓩討�ださい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ a_1 $ $ b_1 $ $ \vdots $ $ a_N $ $ b_N $ $ M $ $ x_1 $ $ y_1 $ $ \vdots $ $ x_M $ $ y_M $

## 補竃鯉塀
基えを竃薦せよ。

## 籾朕寄吭
嗤 $n$ 倖臨弗��及 $i$ 倖臨弗嗤 $a_i$ 議隈薦旺柴皿嬉移 $b_i$ 隈薦議講舗。

更夛 $\{A_n\}$��聞誼斤噐公協議 $m$ 怏 $(x,y)$��譲嗤 $A_x\geqslant b_x,A_y\geqslant b_y$ 賜 $A_y\geqslant b_x,A_x\geqslant b_y$。

萩恷弌晒 $\sum\limits_{i=1}^n |A_i-a_i|。$

translated by syzf2222

```input1
5
1 5
2 4
3 3
4 2
5 1
3
1 4
2 5
3 5
```

```output1
2
```

```input2
4
1 1
1 1
1 1
1 1
3
1 2
2 3
3 4
```

```output2
0
```

```input3
9
1 1
2 4
5 5
7 10
9 3
9 13
10 9
3 9
2 9
7
1 5
2 5
1 6
2 4
3 4
4 9
8 9
```

```output3
22
```

## 戻幣
### 崙�s

- $ 2\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ a_i,b_i\ \leq\ 100 $
- $ 1\ \leq\ M\ \leq\ \frac{N(N-1)}{2} $
- $ 1\ \leq\ x_i\ \lt\ y_i\ \leq\ N $
- $ i\neq\ j $ ならば $ (x_i,y_i)\ \neq\ (x_j,y_j) $
- 秘薦はすべて屁方

### Sample Explanation 1

徴隈聞い $ 1 $ と徴隈聞い $ 4 $ に $ 1 $ 指ずつ荷恬を佩えば恷弌の荷恬指方で朕議を�_撹できます。

### Sample Explanation 2

$ 1 $ 指も荷恬を佩う駅勣がありません。

