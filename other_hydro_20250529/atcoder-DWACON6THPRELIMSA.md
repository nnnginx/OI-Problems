## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/dwacon6th-prelims/tasks/dwacon6th_prelims_a

ニワンゴ埴は $ N $ 爆からなるプレイリストを恬りました。 $ i $ 桑朕の爆はタイトルが $ s_i $ で、壅伏�r�gが $ t_i $ 昼です。 ここで、$ s_1,\ldots,s_N $ が�牀�なることが隠�^されます。

ニワンゴ埴はこのプレイリストを壅伏しながら、恬�Iをしていました。(すなわち、プレイリストの畠爆が��桑宥りに $ 1 $ 指ずつ、�gに俚峭を豫むことなく壅伏されました。) しかし、恬�I嶄に肖蓄りをしてしまい、畠爆の壅伏が�Kわったあとに軟きました。 ���hから、タイトルが $ X $ の爆の壅伏が�Kわるタイミングでニワンゴ埴が媒てしまったことがわかりました。

ニワンゴ埴が媒ている�gに爆が壅伏された�r�gが採昼あったかを箔めてください。

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる。

> $ N $ $ s_1 $ $ t_1 $ $ \vdots $ $ s_{N} $ $ t_N $ $ X $

## 補竃鯉塀
基えを竃薦せよ。

## 籾朕寄吭
Niwango 幹秀阻 $N$ 遍梧爆議殴慧双燕。及 $i$ 遍梧爆議炎籾才隔偬扮寂蛍艶葎 $s_i$ 才 $t_i$ 昼。隠屬$s_1$��$\dots$��$s_N$ 脅頁音揖議。

Niwango 壓殴慧緩殴慧双燕扮屎壓恂匯乂垢恬。 ��匆祥頁傍��侭嗤梧爆脅梓殴慧双燕嶄議乏會殴慧阻匯肝��岻寂短嗤販採壙唯。��徽頁��麿壓垢恬嶄祥鋒彭阻��殴慧頼侭嗤梧爆朔祥佰阻。 功象麿議芝村��潤惚窟�嵋�壓兆葎 $X$ 議梧爆議恷朔鋒彭阻。

臥孀 Niwango 秘鋒扮殴慧蝶乂梧爆議隔偬扮寂。

```input1
3
dwango 2
sixth 5
prelims 25
dwango
```

```output1
30
```

```input2
1
abcde 1000
abcde
```

```output2
0
```

```input3
15
ypnxn 279
kgjgwx 464
qquhuwq 327
rxing 549
pmuduhznoaqu 832
dagktgdarveusju 595
wunfagppcoi 200
dhavrncwfw 720
jpcmigg 658
wrczqxycivdqn 639
mcmkkbnjfeod 992
htqvkgkbhtytsz 130
twflegsjz 467
dswxxrxuzzfhkp 989
szfwtzfpnscgue 958
pmuduhznoaqu
```

```output3
6348
```

## 戻幣
### 崙�s

- $ 1\ \leq\ N\ \leq\ 50 $
- $ s_i,X $ は哂弌猟忖のみからなる�Lさ $ 1 $ 參貧 $ 100 $ 參和の猟忖双
- $ s_1,\ldots,s_N $ は�牀�なる
- $ s_i\ =\ X $ なる屁方 $ i $ が贋壓する
- $ 1\ \leq\ t_i\ \leq\ 1000 $
- $ t_i $ は屁方

### Sample Explanation 1

\- ニワンゴ埴が媒ている�gに壅伏された爆は `sixth` と `prelims` です。 - これらの壅伏�r�gの�t才である $ 30 $ が基えです。

### Sample Explanation 2

\- ニワンゴ埴が媒ている�gに壅伏された爆はありません。 - 壅伏�r�gの�t才は $ 0 $ となります。

