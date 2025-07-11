# AT_arc072_c [ARC072E] Alice in linear land

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc072/tasks/arc072_c

Aliceは数直線の上に住んでいます。今日はある不思議な乗り物に乗って目的地まで行くことを考えました。 はじめ、Aliceは目的地から $ D $ 離れたところにいます。Aliceが乗り物にある数 $ x $ を入力すると、現在地から目的地に向かって $ x $ 進んだところが現在地より目的地に近いとき移動し、そうでないときは動きません。現在地から目的地までの距離が $ x $ 未満のとき、$ x $ 進んだところは目的地を通りすぎていることに注意してください。また、目的地を通り過ぎると進行方向が変わること、進行方向は何度も変わることがあることに注意してください。

Aliceは乗り物に $ N $ 回だけ数を入力し、$ i $ 番目に入力する数は $ d_i $ の予定でした。Aliceは入力する予定数の書かれたリストを作っておき、その数を $ 1 $ つずつ入力します。

しかしイタズラ好きの魔法使いが現れ、Aliceが $ N $ 回の入力による移動を終えても目的地にたどり着かないよう、リストの数を $ 1 $ つだけ書き換えることを考えました。

魔法使いはイタズラの実行のため以下の $ Q $ 個の計画を考えています。

- $ q_i $ 回目に入力する数のみをある正整数に変更することで、Aliceが目的地にたどり着かないようにする

$ Q $ 個の計画それぞれが実行可能であるか答えるプログラムを書いてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ D $ $ d_1 $ $ d_2 $ $ ... $ $ d_N $ $ Q $ $ q_1 $ $ q_2 $ $ ... $ $ q_Q $

## 输出格式

$ i $ 番目の計画が実行可能なら`YES`、そうでないなら`NO`と $ i $ 行目に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 10
3 4 3 3
2
4 3
```

### 输出 #1

```
NO
YES
```

## 输入输出样例 #2

### 输入 #2

```
5 9
4 4 2 3 2
5
1 4 2 3 5
```

### 输出 #2

```
YES
YES
YES
YES
YES
```

## 输入输出样例 #3

### 输入 #3

```
6 15
4 3 5 4 2 1
6
1 2 3 4 5 6
```

### 输出 #3

```
NO
NO
YES
NO
NO
YES
```

## 说明/提示

### 制約

- $ 1≦\ N\ ≦\ 5*10^5 $
- $ 1≦\ Q\ ≦\ 5*10^5 $
- $ 1≦\ D\ ≦\ 10^9 $
- $ 1≦\ d_i\ ≦\ 10^9(1≦i≦N) $
- $ 1≦\ q_i\ ≦\ N(1≦i≦Q) $
- $ d_i,\ D $は整数である

### Sample Explanation 1

$ 3 $ 番目までの入力でAliceはすでに目的地にたどり着いているため、$ 1 $ 番目の計画の答えは`NO`です。 例えば、$ 3 $ 番目の入力を $ 5 $ にすると、Aliceは以下のような移動をし、目的地にたどり着くことはできないため、$ 2 $ 番目の計画の答えは`YES`です。 !\[\](https://atcoder.jp/img/arc072/f6a4307ef86847bc8fa68d0952f7127c.png)

### Sample Explanation 2

もともと入力する予定のままでもAliceは目的地にたどり着けないため、すべての計画は実行可能です。