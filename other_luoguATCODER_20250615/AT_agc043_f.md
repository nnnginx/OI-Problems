# AT_agc043_f [AGC043F] Jewelry Box

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc043/tasks/agc043_f

$ 1 $ から $ N $ までの番号のついた $ N $ 軒の宝石店があります．

宝石店 $ i $ ($ 1\ \leq\ i\ \leq\ N $) では，$ K_i $ 種類の宝石が売られています． このうち，$ j $ ($ 1\ \leq\ j\ \leq\ K_i $) 種類目の宝石は，大きさが $ S_{i,j} $，値段が $ P_{i,j} $ で，在庫が $ C_{i,j} $ 個あります．

**よい** 宝石箱とは，以下の条件をすべて満たす宝石箱です．

- 宝石箱の中には，各宝石店で買った宝石が $ 1 $ 個ずつ入っている．
- 次の $ M $ 個の条件をすべて満たす．
  - $ i $ ($ 1\ \leq\ i\ \leq\ M $) 番目の条件: $ ( $宝石店 $ V_i $ で買った宝石の大きさ$ )\leq\ ( $宝石店 $ U_i $ で買った宝石の大きさ$ )+W_i $

次の $ Q $ 個の質問に答えてください． $ i $ ($ 1\ \leq\ i\ \leq\ Q $) 番目の質問では，整数 $ A_i $ が与えられるので，$ A_i $ 個のよい宝石箱を準備するとき，買う宝石の値段の合計の最小値を求めてください． ただし，$ A_i $ 個のよい宝石箱が準備できない場合はその旨を答えてください．

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ 宝石店$ \ 1\ $の情報 宝石店$ \ 2\ $の情報 $ \vdots $ 宝石店$ \ N\ $の情報 $ M $ $ U_1 $ $ V_1 $ $ W_1 $ $ U_2 $ $ V_2 $ $ W_2 $ $ \vdots $ $ U_M $ $ V_M $ $ W_M $ $ Q $ $ A_1 $ $ A_2 $ $ \vdots $ $ A_Q $

宝石店 $ i $ ($ 1\ \leq\ i\ \leq\ N $) の情報は，以下の形式で与えられる．

> $ K_i $ $ S_{i,1} $ $ P_{i,1} $ $ C_{i,1} $ $ S_{i,2} $ $ P_{i,2} $ $ C_{i,2} $ $ \vdots $ $ S_{i,K_i} $ $ P_{i,K_i} $ $ C_{i,K_i} $

## 输出格式

$ Q $ 行出力せよ． そのうち $ i $ 行目には，$ A_i $ 個のよい宝石箱を準備するときに買う宝石の値段の合計の最小値を出力せよ． ただし，$ A_i $ 個のよい宝石箱を準備することが不可能な場合は，$ -1 $ を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3
2
1 10 1
3 1 1
3
1 10 1
2 1 1
3 10 1
2
1 1 1
3 10 1
2
1 2 0
2 3 0
3
1
2
3
```

### 输出 #1

```
3
42
-1
```

## 输入输出样例 #2

### 输入 #2

```
5
5
86849520 30 272477201869
968023357 28 539131386006
478355090 8 194500792721
298572419 6 894877901270
203794105 25 594579473837
5
730211794 22 225797976416
842538552 9 420531931830
871332982 26 81253086754
553846923 29 89734736118
731788040 13 241088716205
5
903534485 22 140045153776
187101906 8 145639722124
513502442 9 227445343895
499446330 6 719254728400
564106748 20 333423097859
5
332809289 8 640911722470
969492694 21 937931959818
207959501 11 217019915462
726936503 12 382527525674
887971218 17 552919286358
5
444983655 13 487875689585
855863581 6 625608576077
885012925 10 105520979776
980933856 1 711474069172
653022356 19 977887412815
10
1 2 231274893
2 3 829836076
3 4 745221482
4 5 935448462
5 1 819308546
3 5 815839350
5 3 513188748
3 1 968283437
2 3 202352515
4 3 292999238
10
510266667947
252899314976
510266667948
374155726828
628866122125
628866122123
1
628866122124
510266667949
30000000000000
```

### 输出 #2

```
26533866733244
13150764378752
26533866733296
19456097795056
-1
33175436167096
52
33175436167152
26533866733352
-1
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 30 $
- $ 1\ \leq\ K_i\ \leq\ 30 $
- $ 1\ \leq\ S_{i,j}\ \leq\ 10^9 $
- $ 1\ \leq\ P_{i,j}\ \leq\ 30 $
- $ 1\ \leq\ C_{i,j}\ \leq\ 10^{12} $
- $ 0\ \leq\ M\ \leq\ 50 $
- $ 1\ \leq\ U_i,V_i\ \leq\ N $
- $ U_i\ \neq\ V_i $
- $ 0\ \leq\ W_i\ \leq\ 10^9 $
- $ 1\ \leq\ Q\ \leq\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 3\ \times\ 10^{13} $
- 入力は全て整数である．

### Sample Explanation 1

宝石店 $ i $ で売られている $ j $ 種類目の宝石を宝石 $ (i,j) $ で表すことにします． 各クエリの答えは，以下のようになります． - $ A_1=1 $: 宝石 $ (1,2),(2,2),(3,1) $ を使う宝石箱を準備すると，コストが $ 1+1+1=3 $ となり，最小． - $ A_2=2 $: 宝石 $ (1,1),(2,1),(3,1) $ を使う宝石箱と，宝石 $ (1,2),(2,3),(3,2) $ を使う宝石箱を準備すると， コストが $ (10+10+1)+(1+10+10)=42 $ となり，最小． - $ A_3=3 $: $ 3 $ つの良い宝石箱を準備することはできない．