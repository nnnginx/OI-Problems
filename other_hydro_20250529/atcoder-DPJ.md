## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_j

$ N $ 旦の駐があります。 駐には $ 1,\ 2,\ \ldots,\ N $ と桑催が尅られています。 恷兜、光 $ i $ ($ 1\ \leq\ i\ \leq\ N $) について、駐 $ i $ には $ a_i $ ($ 1\ \leq\ a_i\ \leq\ 3) $ ��の勉望が崔かれています。

すべての勉望が�oくなるまで、湊隻埴は肝の荷恬を�Rり卦し佩います。

- $ 1,\ 2,\ \ldots,\ N $ の朕が吉�_楕で竃るサイコロを尅り、竃朕を $ i $ とする。 駐 $ i $ に勉望がある��栽、駐 $ i $ の勉望を $ 1 $ ��奮べる。 駐 $ i $ に勉望が�oい��栽、採も佩わない。

すべての勉望が�oくなるまでの荷恬指方の豚棋�､鯒鵑瓩討�ださい。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ a_1 $ $ a_2 $ $ \ldots $ $ a_N $

## 補竃鯉塀
すべての勉望が�oくなるまでの荷恬指方の豚棋�､魍�薦せよ。 �����`餓が $ 10^{-9} $ 參和ならば屎盾となる。

## 籾朕寄吭
�嶝�$N(1 ＋ N ＋ 300)$倖徒徨��園催葎$1,2,3,´,N$。及$i$倖徒徨嶄慧嗤$a_i(1＋a_i ＋3)$倖勉望。

俊和栖耽肝峇佩參和荷恬��岷崛郭頼侭嗤議勉望。貫及$1,2,3,´,N$倖徒徨嶄販僉匯倖徒徨��郭渠凪嶄議匯倖勉望。飛短嗤勉望夸音郭。

飛繍侭嗤勉望郭頼��萩諒緩扮荷恬肝方議方僥豚李頁謹富��

```input1
3
1 1 1
```

```output1
5.5
```

```input2
1
3
```

```output2
3
```

```input3
2
1 2
```

```output3
4.5
```

```input4
10
1 3 2 3 3 2 3 2 1 3
```

```output4
54.48064457488221
```

## 戻幣
### 崙�s

- 秘薦はすべて屁方である。
- $ 1\ \leq\ N\ \leq\ 300 $
- $ 1\ \leq\ a_i\ \leq\ 3 $

### Sample Explanation 1

$ 1 $ ��朕の勉望を奮べるまでの荷恬指方の豚棋�､� $ 1 $ です。 その瘁、$ 2 $ ��朕の勉望を奮べるまでの荷恬指方の豚棋�､� $ 1.5 $ です。 その瘁、$ 3 $ ��朕の勉望を奮べるまでの荷恬指方の豚棋�､� $ 3 $ です。 よって、畠悶の荷恬指方の豚棋�､� $ 1\ +\ 1.5\ +\ 3\ =\ 5.5 $ です。

### Sample Explanation 2

箭えば、`3.00`, `3.000000003`, `2.999999997` などを竃薦しても屎盾となります。

