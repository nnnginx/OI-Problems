# AT_arc169_e [ARC169E] Avoid Boring Matches

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc169/tasks/arc169_e

$ 1 $ から $ 2^N $ までの番号のついた $ 2^N $ 人の参加者がいる大会があります．

大会は次のように進行します．

- まず最初に，それぞれの参加者に赤または青の帽子をかぶせる． ここで，各参加者にかぶせる帽子の色は文字列 $ S $ によって与えられる． 具体的には，$ S $ の $ i $ 文字目 ($ 1\ \leq\ i\ \leq\ 2^N $) が `R` のときは赤い帽子を，`B` のときは青い帽子を参加者 $ i $ にかぶせる．
- その後，参加者が $ 1 $ 人になるまで以下の操作を繰り返す．
  
  
  - 現在の参加者の人数を $ 2k $ 人とする．参加者を $ k $ 個の $ 2 $ 人組に分ける． この組分けはあなたが自由に選ぶことができる． そしてそれぞれの組で試合を行い，勝者は残り，敗者は大会から去る． なお，参加者は強さ順に番号づけられているため，必ず番号の**小さい**参加者が勝利する．
 
あなたは，赤い帽子をかぶった参加者同士の試合を**つまらない**試合と呼んでいます． あなたの目標は，大会中につまらない試合が発生しないように各組分けを行うことです．

目標が達成可能であるか否かは文字列 $ S $ に依存します． そこであなたは，大会の開始前に $ S $ に細工することにしました． 具体的には，あなたは次の操作を $ 0 $ 回以上行えます．

- $ S $ 中の隣接する $ 2 $ 文字を選び，入れ替える．
 
操作の結果目標を達成することが可能かどうか判定してください． また，可能な場合は必要な最小の操作回数を求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $

## 输出格式

目標を達成することが不可能な場合は $ -1 $ を出力せよ． 可能な場合は必要な最小の操作回数を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
RRBB
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
1
RR
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
4
RBBRRBRBBRBBBRBR
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
5
RBRRBRRRBRRRRRRRRRBBBBBBBBBBBBBB
```

### 输出 #4

```
11
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 18 $
- $ S $ は `R`, `B` からなる長さ $ 2^N $ の文字列．
- 入力される値はすべて整数．
 
### Sample Explanation 1

操作を $ 1 $ 回も行わないと，目標を達成することができません． $ S $ の $ 2 $ 文字目と $ 3 $ 文字目を入れ替える操作を行い，$ S= $`RBRB` とすると，以下のようにして目標を達成できます． - 参加者 $ 1,2,3,4 $ にそれぞれ 赤,青,赤,青 の帽子をかぶせる． - $ 4 $ 人の参加者を $ 2 $ つの組 $ (1,4),(2,3) $ に分ける． ここでつまらない試合は発生しない． 試合の結果，参加者 $ 1,2 $ が勝ち残る． - $ 2 $ 人の参加者を $ 1 $ つの組 $ (1,2) $ に分ける． ここでつまらない試合は発生しない． 試合の結果，参加者 $ 1 $ が勝ち残る． よって答えは $ 1 $ です．