# AT_cf_2015_relay_g 主菜と副菜

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-relay/tasks/cf_2015_relay_g

$ N $ 種類の主菜と $ M $ 種類の副菜から料理を選んでコースを作ります。 主菜は $ 1 $ 種類しか選ぶことができませんが、副菜は何種類でも選ぶことができます。 また、副菜は $ 1 $ つも選ばなくても構いません。 主菜・副菜ともにコースに入れられるのは $ 1 $ 種類につき $ 1 $ つまでです。

- $ i $ 番目の主菜は値段が $ A_i $ で、お客さんの評価が $ B_i $ です。
- $ i $ 番目の副菜は値段が $ C_i $ で、お客さんの評価が $ D_i $ です。

コース全体の値段と評価は、主菜と副菜の合計で決まります。 コースの値段を $ L $ 以下にする時、コースの評価は最大でいくつになるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ L $ $ A_1 $ $ B_1 $ : $ A_N $ $ B_N $ $ C_1 $ $ D_1 $ : $ C_M $ $ D_M $

- $ 1 $ 行目には、$ 3 $ つの整数 $ N\ (1\ ≦\ N\ ≦\ 10,000) $, $ M\ (1\ ≦\ M\ ≦\ 1,000) $, $ L\ (1\ ≦\ L\ ≦\ 10,000) $ が空白区切りで与えられる。
- $ 2 $ 行目からの $ N $ 行には、主菜の情報が与えられる。このうち $ i\ (1\ ≦\ i\ ≦\ N) $ 行目には、$ i $ 番目の主菜の値段と評価を表す整数 $ A_i\ (1\ ≦\ A_i\ ≦\ 10,000) $, $ B_i\ (1\ ≦\ B_i\ ≦\ 10,000) $ が与えられる。
- $ N+2 $ 行目からの $ M $ 行には、副菜の情報が与えられる。このうち $ i\ (1\ ≦\ i\ ≦\ M) $ 行目には、$ i $ 番目の副菜の値段と評価を表す整数 $ C_i\ (1\ ≦\ C_i\ ≦\ 10,000) $, $ D_i\ (1\ ≦\ D_i\ ≦\ 10,000) $ が与えられる。
- 必ずコースを作れることが保証される。

## 输出格式

コースの評価の最大値を $ 1 $ 行に出力せよ。出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
2 2 10
2 3
3 6
3 5
5 5
```

### 输出 #1

```
13
```

## 输入输出样例 #2

### 输入 #2

```
3 3 10
1 1
2 3
3 5
4 8
5 10
6 12
```

### 输出 #2

```
19
```

## 输入输出样例 #3

### 输入 #3

```
3 3 10
1 1
11 11
11 11
11 11
11 11
11 11
```

### 输出 #3

```
1
```