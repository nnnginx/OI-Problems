# AT_agc040_b [AGC040B] Two Contests

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc040/tasks/agc040_b

$ 1 $ から $ 10^9 $ までの番号のついた $ 10^9 $ 人が参加する大会があります． この大会では，$ 2 $ 回のコンテストが行われます．

コンテストで出題する問題として，$ 1 $ から $ N $ までの番号のついた $ N $ 問が準備されています． 問題 $ i $ が出題された場合，番号が $ L_i $ 以上 $ R_i $ 以下の参加者は全員正解し，逆にそれ以外の参加者は誰も解けません．

これらの $ N $ 問を，$ 2 $ 回のコンテストに分けて出題します． どの問題も，ちょうど $ 1 $ 回のコンテストで出題されなくてはいけません． また，どちらのコンテストも，少なくとも $ 1 $ 問以上の問題が出題される必要があります．

それぞれのコンテストの**楽しさ**は，そのコンテストの全ての問題を解く参加者の人数です． $ 2 $ 回のコンテストの楽しさの和としてありうる最大の値を求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ \vdots $ $ L_N $ $ R_N $

## 输出格式

$ 2 $ 回のコンテストの楽しさの和としてありうる最大の値を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
4
4 7
1 4
5 8
2 5
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
4
1 20
2 19
3 18
4 17
```

### 输出 #2

```
34
```

## 输入输出样例 #3

### 输入 #3

```
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

### 输出 #3

```
540049931
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ L_i\ \leq\ R_i\ \leq\ 10^9 $
- 入力される値はすべて整数である．

### Sample Explanation 1

以下のようにするのが最適です． - $ 1 $ 回目のコンテストで問題 $ 1,3 $ を出題する．人 $ 5,6,7 $ がこのコンテストの問題を全て解くので，コンテストの楽しさは $ 3 $ である． - $ 2 $ 回目のコンテストで問題 $ 2,4 $ を出題する．人 $ 2,3,4 $ がこのコンテストの問題を全て解くので，コンテストの楽しさは $ 3 $ である． - $ 2 $ 回のコンテストの楽しさの和が $ 6 $ になる．楽しさの和を $ 6 $ より大きくすることは出来ない．