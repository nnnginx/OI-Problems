## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/abc082/tasks/arc087_b

屈肝圷峠中の圻泣にロボットが崔かれています。 恷兜、ロボットは $ x $ �Sの屎の�鬚�を�鬚い討い泙后�

このロボットに凋綜双 $ s $ が嚥えられます。 $ s $ は肝の $ 2 $ 猟忖のみからなり、枠�^から挑硫まで��に�g佩されます。

- `F` : 書�鬚い討い誅鬚�に�Lさ $ 1 $ だけ卞�咾垢襦�
- `T` : �r��指りまたは郡�r��指りの挫きな圭�鬚� $ 90 $ 業だけ�鬚�を�笋┐襦�

ロボットの朕�砲蓮�凋綜双をすべて�g佩し�Kわった瘁に恙�� $ (x,\ y) $ にいることです。 この朕�砲��_撹辛嬬か登協してください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ s $ $ x $ $ y $

## 補竃鯉塀
朕�砲��_撹辛嬬ならば `Yes` を竃薦し、�_撹音辛嬬ならば `No` を竃薦せよ。

## 籾朕寄吭
籾吭宙峰��
�嶝侑燦�字匂繁壓恫炎已圻泣侃��劾��x已屎圭�髻８�協匯倖凋綜堪s��s坪根嗤曾嶽凋綜��F,T。F燕幣�魑映鯵��鯒綾�1化��T燕幣�鰈�**賜**�鰉厥�廬90業。萩低指基��梓孚凋綜堪s峇佩��氏音氏欺器(x,y)侃。��x嚥y喇籾朕補秘��

```input1
FTFFTFFF
4 2
```

```output1
Yes
```

```input2
FTFFTFFF
-2 -2
```

```output2
Yes
```

```input3
FF
1 0
```

```output3
No
```

```input4
TF
1 0
```

```output4
No
```

```input5
FFTTFF
0 0
```

```output5
Yes
```

```input6
TTTT
1 0
```

```output6
No
```

## 戻幣
### 崙�s

- $ s $ は `F`, `T` のみからなる。
- $ 1\ \leq\ |s|\ \leq\ 8\ 000 $
- $ x $, $ y $ は屁方である。
- $ |x|,\ |y|\ \leq\ |s| $

### Sample Explanation 1

$ 1 $ 桑朕の `T` で郡�r��巓りに $ 90 $ 業だけ�鬚�を�笋─�$ 2 $ 桑朕の `T` で�r��巓りに $ 90 $ 業だけ�鬚�を�笋┐譴个茲い任后�

### Sample Explanation 2

$ 1 $ 桑朕の `T` で�r��巓りに $ 90 $ 業だけ�鬚�を�笋─�$ 2 $ 桑朕の `T` で�r��巓りに $ 90 $ 業だけ�鬚�を�笋┐譴个茲い任后�

### Sample Explanation 5

箭えば、$ 1 $ 桑朕の `T` で郡�r��巓りに $ 90 $ 業だけ�鬚�を�笋─�$ 2 $ 桑朕の `T` で郡�r��巓りに $ 90 $ 業だけ�鬚�を�笋┐譴个茲い任后�

