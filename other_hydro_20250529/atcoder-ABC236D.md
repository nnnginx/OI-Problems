## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc236/tasks/abc236_d

$ 1,\ 2,\ \ldots,\ 2N $ と桑催づけられた $ 2N $ 繁の繁が玲未氏に歌紗します。 泳らは $ N $ ��の $ 2 $ 繁�Mにわかれてダンスを啝ります。

$ 2 $ 繁�Mを��撹する繁のうち、桑催の弌さい圭の繁が繁 $ i $ 、桑催の寄きい圭の繁が繁 $ j $ のとき、 その $ 2 $ 繁�Mの仝�猥圈垢� $ A_{i,\ j} $ です。  
 $ N $ ��の $ 2 $ 繁�Mの�猥圓�それぞれ $ B_1,\ B_2,\ \ldots,\ B_N $ であるとき、 仝玲未氏畠悶の�Sしさ々はそれらのビットごとの電麿議��尖才である $ B_1\ \oplus\ B_2\ \oplus\ \cdots\ \oplus\ B_N $ です。

仝 $ 2N $ 繁の歌紗宀が $ N $ ��の $ 2 $ 繁�Mに蛍かれる圭隈々を徭喇に�xべるとき、仝玲未氏畠悶の�Sしさ々としてあり誼る恷寄�､魍�薦してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ A_{1,\ 2} $ $ A_{1,\ 3} $ $ A_{1,\ 4} $ $ \cdots $ $ A_{1,\ 2N} $ $ A_{2,\ 3} $ $ A_{2,\ 4} $ $ \cdots $ $ A_{2,\ 2N} $ $ A_{3,\ 4} $ $ \cdots $ $ A_{3,\ 2N} $ $ \vdots $ $ A_{2N-1,\ 2N} $

## 補竃鯉塀
玲未氏畠悶の�Sしさとしてあり誼る恷寄�､魍�薦せよ。

## 籾朕寄吭
嗤 $2N$ 倖繁歌紗匯倖玲氏。麿断氏曾曾匯怏蛍撹 $N$ 怏。

泌惚 及$i$ 倖繁嚥及 $j$ 倖繁塘斤 ($i \leq j$) ��椎担氏恢伏 $A_{i,j}$ 議＾挫螺業￣。

斑厘断協吶及 $i$ 倖塘斤議挫螺業葎 $B_{i}$ 。

匯倖塗斤議挫螺業瓜協吶葎耽倖塘斤議挫螺業議呟賜才 ($B_{1} \oplus B_{2} \oplus B_{3} \oplus ...B_{N}$) 。

泌惚繁辛參販吭喜塘��萩諒宸倖塗斤議恷寄＾挫螺業￣頁焚担�進箜�宸倖峙。

```input1
2
4 0 1
5 3
2
```

```output1
6
```

```input2
1
5
```

```output2
5
```

```input3
5
900606388 317329110 665451442 1045743214 260775845 726039763 57365372 741277060 944347467
369646735 642395945 599952146 86221147 523579390 591944369 911198494 695097136
138172503 571268336 111747377 595746631 934427285 840101927 757856472
655483844 580613112 445614713 607825444 252585196 725229185
827291247 105489451 58628521 1032791417 152042357
919691140 703307785 100772330 370415195
666350287 691977663 987658020
1039679956 218233643
70938785
```

```output3
1073289207
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 8 $
- $ 0\ \leq\ A_{i,\ j}\ <\ 2^{30} $
- 秘薦はすべて屁方

### Sample Explanation 1

繁 $ i $ と繁 $ j $ からなる $ 2 $ 繁�Mを $ \lbrace\ i,\ j\rbrace $ で燕します。 $ 4 $ 繁が $ 2 $ ��の $ 2 $ 繁�Mにわかれる圭隈は和��の $ 3 $ 宥りです。 - $ \lbrace\ 1,\ 2\rbrace,\ \lbrace\ 3,\ 4\rbrace $ という $ 2 $ �Mにわかれる。 このとき、玲未氏畠悶の�Sしさは $ A_{1,\ 2}\ \oplus\ A_{3,\ 4}\ =\ 4\ \oplus\ 2\ =\ 6 $ です。 - $ \lbrace\ 1,\ 3\rbrace,\ \lbrace\ 2,\ 4\rbrace $ という $ 2 $ �Mにわかれる。 このとき、玲未氏畠悶の�Sしさは $ A_{1,\ 3}\ \oplus\ A_{2,\ 4}\ =\ 0\ \oplus\ 3\ =\ 3 $ です。 - $ \lbrace\ 1,\ 4\rbrace,\ \lbrace\ 2,\ 3\rbrace $ という $ 2 $ �Mにわかれる。 このとき、玲未氏畠悶の�Sしさは $ A_{1,\ 4}\ \oplus\ A_{2,\ 3}\ =\ 1\ \oplus\ 5\ =\ 4 $ です。 よって、玲未氏畠悶の�Sしさとしてあり誼る恷寄�､� $ 6 $ です。

### Sample Explanation 2

繁 $ 1 $ と繁 $ 2 $ からなる $ 2 $ 繁�Mのみが恬られ、このときの玲未氏畠悶の�Sしさは $ 5 $ です。

