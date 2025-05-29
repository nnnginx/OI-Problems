## 题目描述
[problemUrl]: https://atcoder.jp/contests/dwacon6th-prelims/tasks/dwacon6th_prelims_a

ニワンゴ君は $ N $ 曲からなるプレイリストを作りました。 $ i $ 番目の曲はタイトルが $ s_i $ で、再生時間が $ t_i $ 秒です。 ここで、$ s_1,\ldots,s_N $ が相異なることが保証されます。

ニワンゴ君はこのプレイリストを再生しながら、作業をしていました。(すなわち、プレイリストの全曲が順番通りに $ 1 $ 回ずつ、間に休止を挟むことなく再生されました。) しかし、作業中に居眠りをしてしまい、全曲の再生が終わったあとに起きました。 記録から、タイトルが $ X $ の曲の再生が終わるタイミングでニワンゴ君が寝てしまったことがわかりました。

ニワンゴ君が寝ている間に曲が再生された時間が何秒あったかを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ t_1 $ $ \vdots $ $ s_{N} $ $ t_N $ $ X $

## 输出格式
答えを出力せよ。

## 题目大意
Niwango 创建了 $N$ 首歌曲的播放列表。第 $i$ 首歌曲的标题和持续时间分别为 $s_i$ 和 $t_i$ 秒。保证$s_1$，$\dots$，$s_N$ 都是不同的。

Niwango 在播放此播放列表时正在做一些工作。 （也就是说，所有歌曲都按播放列表中的顺序播放了一次，之间没有任何暂停。）但是，他在工作中就睡着了，播放完所有歌曲后就醒了。 根据他的记录，结果发现他在名为 $X$ 的歌曲的最后睡着了。

查找 Niwango 入睡时播放某些歌曲的持续时间。

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

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ s_i,X $ は英小文字のみからなる長さ $ 1 $ 以上 $ 100 $ 以下の文字列
- $ s_1,\ldots,s_N $ は相異なる
- $ s_i\ =\ X $ なる整数 $ i $ が存在する
- $ 1\ \leq\ t_i\ \leq\ 1000 $
- $ t_i $ は整数

### Sample Explanation 1

\- ニワンゴ君が寝ている間に再生された曲は `sixth` と `prelims` です。 - これらの再生時間の総和である $ 30 $ が答えです。

### Sample Explanation 2

\- ニワンゴ君が寝ている間に再生された曲はありません。 - 再生時間の総和は $ 0 $ となります。

