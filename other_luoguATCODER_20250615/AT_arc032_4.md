# AT_arc032_4 [ARC032D] アットコーダーモンスターズ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc032/tasks/arc032_4

アットコーダーモンスターズと言うゲームは、モンスターのチームを編成してバトルするゲームです。

あなたはモンスターを売っているお店にいます。 このお店では、$ N $ 匹のモンスターが横一列に並べられています。そして、各モンスター $ A_i\ (1\ ≦\ i\ ≦N) $ には以下に示す $ 2 $ つの能力値が存在しています。

- モンスター $ M_i $ のこうげきの能力を表す値 $ {M_i}_{ATK} $
- モンスター $ M_i $ のぼうぎょの能力を表す値 $ {M_i}_{DEF} $

いま、$ N $ 匹のモンスターの中から異なるちょうど $ K $ 匹のモンスターを選んで購入し、それらでチームを編成しようとしています。 しかし、ある能力値について、それらがかけ離れたモンスター同士がいるとチームとして安定しないことが分かっているので、できるだけ安定したチームを作りたいと思っています。

より厳密に、チームに含まれる $ 2 $ 匹のモンスター $ X $ と $ Y $ についてその不安定度 $ S_{X,Y} $ を、

- $ S_{X,Y} $ = max{ $ |X_{ATK}\ -\ Y_{ATK}| $, $ |X_{DEF}\ -\ Y_{DEF}| $ }

と定義したとき、チームの不安定度は、チームに含まれる全てのモンスターのペアについて計算して得られる不安定度の最大値です。 チームに含まれるモンスターが $ 1 $ 匹の時、チームの不安定度は $ 0 $ です。

あなたは、チームの不安定度を最小化するような異なる $ K $ 匹のモンスターを購入しようと思っています。 さらに、チームの不安定度を最小とするようなモンスターの選び方の総数も求めたいと思っています。

あなたは、達成できるチームの不安定度の最小値と、それを達成するモンスターの選び方の総数を $ 1,000,000,007 $ で割った余りを出力しなければなりません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ {M_1}_{ATK} $ $ {M_1}_{DEF} $ $ {M_2}_{ATK} $ $ {M_2}_{DEF} $ : $ {M_N}_{ATK} $ $ {M_N}_{DEF} $

- $ 1 $ 行目には、お店に並んでいるモンスターの数と購入したいモンスターの数を表す $ 2 $ つの整数 $ N\ (1\ ≦\ N\ ≦\ 100,000) $ と $ K\ (1\ ≦\ K\ ≦\ N) $ がスペース区切りで与えられる.
- $ 2 $ 行目から $ N $ 行には、お店に並んでいるモンスターの能力値の情報が与えられる。そのうち $ i $ 行目には、$ i $ 番目のモンスターの能力値を表す $ 2 $ つの整数 $ {M_i}_{ATK},\ {M_i}_{DEF}\ (0\ ≦\ {M_i}_{ATK},\ {M_i}_{DEF}\ ≦\ 3000) $ がスペース区切りで与えられる。

## 输出格式

$ 1 $ 行目には、達成できるチームの不安定度の最小値を出力せよ。

$ 2 $ 行目には、チームの不安定度を最小化するようなモンスターの選び方の総数を $ 1000000007 $ で割った余りを出力せよ。

末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
4 3
0 0
1 1
3 3
2 2
```

### 输出 #1

```
2
2
```

## 输入输出样例 #2

### 输入 #2

```
4 2
1 1000
10 100
100 10
1000 1
```

### 输出 #2

```
90
1
```

## 输入输出样例 #3

### 输入 #3

```
3 1
1 1
2 2
3 3
```

### 输出 #3

```
0
3
```

## 输入输出样例 #4

### 输入 #4

```
40 18
0 0
0 0
0 0
0 0
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
3000 3000
```

### 输出 #4

```
0
75135237
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ 10 $ 点分のテストケースにおいて、$ 1≦N≦20 $ を満たす。

### Sample Explanation 1

モンスターは以下のように並んでおり、$ 3 $ 匹を選ぶときの不安定度の最小値は $ 2 $ である。また、選び方は $ 2 $ 通りある。 !\[\](http://arc032.contest.atcoder.jp/img/arc/032/D\_sample1.png)