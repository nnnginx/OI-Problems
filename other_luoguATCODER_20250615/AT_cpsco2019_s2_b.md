# AT_cpsco2019_s2_b Telephone Q

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cpsco2019-s2/tasks/cpsco2019_s2_b

夜のテレビ番組「こんばんはゴジラです」では、次のようなパネルめくりゲームを実施しています。

ゲームの参加者であるあなたは、初めに $ 0 $ 円を持っています。

各パネルには記号と非負整数が $ 1 $ つずつ書かれており、 $ i $ 番目のパネルに書かれた記号と非負整数はそれぞれ $ c_i,\ a_i $ です。

あなたが $ i $ 番目のパネルを開けたとき、以下のルールに従ってあなたの所持金が変化します。

- $ c_i= $ `+` のとき：所持金が $ a_i $ 円増える。
- $ c_i= $ `-` のとき：所持金が $ a_i $ 円減る。
- $ c_i= $ `*` のとき：所持金が $ a_i $ 倍になる。

あなたは、 $ N $ 枚のパネルのうち $ 0 $ 枚以上のパネルを、$ 1 $ 枚ずつ好きな順番で開けることができ、途中でいつでもゲームを終了することができます。また、ゲーム途中及び終了時に所持金が負の値になってもかまいません。

あらかじめどのパネルに何が書かれてあるかを知っているあなたは、ゲーム終了時の自分の所持金を最大化しようとしました。ゲーム終了時の所持金の最大値 $ M $ を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ c_1 $ $ a_1 $ $ : $ $ c_N $ $ a_N $

## 输出格式

ゲーム終了時の所持金の最大値 $ M $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
+ 100
- 80
* 3
+ 300
```

### 输出 #1

```
1200
```

## 输入输出样例 #2

### 输入 #2

```
3
- 314
- 159
- 265
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
4
* 8
+ 7
* 0
* 5
```

### 输出 #3

```
280
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 0\ \leq\ a_i\ \leq\ 1000 $
- $ c_i $ は`+`, `-`, `*` のいずれかである。
- ゲーム終了時の所持金の最大値 $ M $ は $ 10^9 $ を超えない。

### Sample Explanation 1

「 $ +100 $ 」,「 $ +300 $ 」,「 $ *3 $ 」のパネルを順に開けた後ゲームを終了することによって、 $ 1200 $ 円を得ることができます。

### Sample Explanation 2

$ 1 $ 枚もパネルを開かずにゲームを終了することもできます。