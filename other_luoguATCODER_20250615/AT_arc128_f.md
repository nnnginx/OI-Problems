# AT_arc128_f [ARC128F] Game against Robot

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc128/tasks/arc128_f

$ 1 $ から $ N $ までの番号のついた $ N $ 枚のカードがあり，カード $ i $ には整数 $ A_i $ が書かれています． なお，$ N $ は偶数です．

すぬけくんとロボットがゲームをします． ゲームは，以下のように進行します．

- ゲームマスターが $ (1,2,\cdots,N) $ の順列 $ (p_1,p_2,\cdots,p_N) $ を宣言する． この順列はすぬけくんとロボット両方に知らされる．
- その後，すぬけくんからはじめて，両者が交互に手番をプレイする． 各手番では以下のことが起こる．
  - すぬけくんの手番: 残っているカードの中から好きなものを一つ選び，食べる．
  - ロボットの手番: 残っているカードのうち，$ p_i $ が最大となるカード $ i $ を選び，燃やす．
- カードがなくなったらゲームは終了する．

最終的なゲームのスコアは，すぬけくんが食べたカードに書かれた整数の総和です． すぬけくんは，ゲームのスコアを最大化するように最適な行動をします．

順列 $ p $ は $ N! $ 通り考えられますが，これらすべてについてゲームのスコアを求め，その総和を $ 998244353 $ で割った余りを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
1 2
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4
1 100 10000 1000000
```

### 输出 #2

```
24200400
```

## 输入输出样例 #3

### 输入 #3

```
10
866111664 178537096 844917655 218662351 383133839 231371336 353498483 865935868 472381277 579910117
```

### 输出 #3

```
710984634
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^6 $
- $ N $ は偶数
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- 入力される値はすべて整数である

### Sample Explanation 1

順列 $ p $ に依らず，すぬけくんはカード $ 2 $ を食べます．

### Sample Explanation 2

例えば $ p=(3,1,4,2) $ であるとき，ゲームは以下のように進行します． - すぬけくんがカード $ 3 $ を食べる． - ロボットがカード $ 1 $ を燃やす． - すぬけくんがカード $ 4 $ を食べる． - ロボットがカード $ 2 $ を燃やす． このとき，ゲームのスコアは $ 1010000 $ になります．