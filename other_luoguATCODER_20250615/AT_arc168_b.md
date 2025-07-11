# AT_arc168_b [ARC168B] Arbitrary Nim

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc168/tasks/arc168_b

石の山が $ N $ 個あり，$ i $ 番目 ($ 1\ \leq\ i\ \leq\ N $) の山には $ A_i $ 個の石が積まれています．

あなたは今から正整数 $ k $ を選びます． その後，Alice と Bob がこの山を使って以下のようなゲームを行います．

- Alice から始めて両者は交互に手番をプレイする．
- 各手番では，プレイヤーは空でない山を一つ選び，その山から $ 1 $ 個以上 $ k $ 個以下の好きな個数の石を取り除く．
 
自分の手番で操作が行えなくなった人が負けで，負けなかった人が勝ちです．

あなたは正整数 $ k $ を選ぶとき，Alice に必勝法が存在するようにしたいです． そのような $ k $ が存在するか判定してください． 存在する場合は，そのような $ k $ の最大値が存在するか判定してください． 最大値が存在する場合は，その値を答えてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

Alice に必勝法が存在するような $ k $ が存在しない場合，$ 0 $ を出力せよ．

Alice に必勝法が存在するような $ k $ が存在するが，その最大値が存在しない場合，$ -1 $ を出力せよ．

Alice に必勝法が存在するような $ k $ が存在し，その最大値も存在する場合，その値を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3
1 2 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4
1 2 3 4
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
2
100 100
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 250000 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- 入力される値はすべて整数．
 
### Sample Explanation 1

例えば，$ k=2 $ とすると Alice に必勝法が存在します． $ 3\ \leq\ k $ を選んだ場合は Alice に必勝法が存在しないので，$ k=2 $ が答えです．

### Sample Explanation 2

例えば，すべての $ k=100,200,300,\cdots $ に対して Alice に必勝法が存在します． よって $ k $ の最大値は存在しないため，$ -1 $ を出力します．

### Sample Explanation 3

どのような $ k $ を選んでも Alice に必勝法は存在しません． よって $ 0 $ を出力します．