## 籾朕宙峰
[problemUrl]: https://atcoder.jp/contests/agc040/tasks/agc040_b

$ 1 $ から $ 10^9 $ までの桑催のついた $ 10^9 $ 繁が歌紗する寄氏があります�� この寄氏では��$ 2 $ 指のコンテストが佩われます��

コンテストで竃�}する���}として��$ 1 $ から $ N $ までの桑催のついた $ N $ ��が���笋気譴討い泙坑� ���} $ i $ が竃�}された��栽��桑催が $ L_i $ 參貧 $ R_i $ 參和の歌紗宀は畠�T屎盾し��剃にそれ參翌の歌紗宀は�lも盾けません��

これらの $ N $ ��を��$ 2 $ 指のコンテストに蛍けて竃�}します�� どの���}も��ちょうど $ 1 $ 指のコンテストで竃�}されなくてはいけません�� また��どちらのコンテストも��富なくとも $ 1 $ ��參貧の���}が竃�}される駅勣があります��

それぞれのコンテストの**�Sしさ**は��そのコンテストの畠ての���}を盾く歌紗宀の繁方です�� $ 2 $ 指のコンテストの�Sしさの才としてありうる恷寄の�､鯒鵑瓩討�ださい��

## 補秘鯉塀
秘薦は參和の侘塀で���僻訌Δ�ら嚥えられる��

> $ N $ $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ \vdots $ $ L_N $ $ R_N $

## 補竃鯉塀
$ 2 $ 指のコンテストの�Sしさの才としてありうる恷寄の�､魍�薦せよ��

## 籾朕寄吭
公協 $n$ 倖曝寂 $[l_i,r_i]$��低俶勣繍麿断蛍撹曾怏��耽怏音嬬葎腎��協吶耽怏議幡峙葎凪嶄侭嗤曝寂議住鹿議海業��低俶勣恷寄晒曾倖怏議幡峙才。

```input1
4
4 7
1 4
5 8
2 5
```

```output1
6
```

```input2
4
1 20
2 19
3 18
4 17
```

```output2
34
```

```input3
10
457835016 996058008
456475528 529149798
455108441 512701454
455817105 523506955
457368248 814532746
455073228 459494089
456651538 774276744
457667152 974637457
457293701 800549465
456580262 636471526
```

```output3
540049931
```

## 戻幣
### 崙�s

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ L_i\ \leq\ R_i\ \leq\ 10^9 $
- 秘薦される�､呂垢戮噸�方である��

### Sample Explanation 1

參和のようにするのが恷�mです�� - $ 1 $ 指朕のコンテストで���} $ 1,3 $ を竃�}する��繁 $ 5,6,7 $ がこのコンテストの���}を畠て盾くので��コンテストの�Sしさは $ 3 $ である�� - $ 2 $ 指朕のコンテストで���} $ 2,4 $ を竃�}する��繁 $ 2,3,4 $ がこのコンテストの���}を畠て盾くので��コンテストの�Sしさは $ 3 $ である�� - $ 2 $ 指のコンテストの�Sしさの才が $ 6 $ になる���Sしさの才を $ 6 $ より寄きくすることは竃栖ない��

