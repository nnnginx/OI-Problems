# AT_pakencamp_2018_day2_f 同一経路　(Samepath)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/pakencamp-2018-day2/tasks/pakencamp_2018_day2_f

PAKEN 市長の E869120 氏は、市にいくつかのチェックポイントと、$ 2 $ つのチェックポイントを結ぶいくつかの一方通行の道路を建設することを計画しました。  
 チェックポイントの数を $ N $ とし、チェックポイントを $ 1,\ 2,\ 3,\ ...,\ N $ と番号付けするものとします。

太古の時代から、この市のラッキーナンバーは $ K $ とされています。  
 そのため、市長は以下のような条件を満たすものを建設することに決めました。

- チェックポイント $ 1 $ から $ N $ まで行く方法の通り数が、ちょうど $ K $ 通りである。
- チェックポイント $ 1 $ から $ N $ まで行く方法のうち、どの経路を選んで通っても、通る道路の本数は変わらない。

例えば、$ K\ =\ 5 $ のとき、以下のチェックポイントと道路の配置は条件を満たします。何故なら、チェックポイント $ 1 $ から $ N $ まで行く方法の総数は $ K\ =\ 5 $ 通りであり、全ての行き方についてちょうど $ 3 $ 本の道を通るからです。  
![ ](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_pakencamp_2018_day2_f/4379b80366668b54888c35cd5a034042900da91b.png)

コストの関係上、市長はできるだけチェックポイントの数 $ N $ をできるだけ小さくしたいです。

このような条件を建設の仕方を $ 1 $ つ構成してください。**ただし、チェックポイント $ a $ から $ b $ まで直接行く道路は $ a\ <\ b $ でないと建てられず、複数の「同じ 2 つのチェックポイントを結ぶ道路」を建ててはいけないものとします。**

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式

出力は以下の形式で行うこと。

> $ N $ $ M $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ $ a_3 $ $ b_3 $ ... $ a_M $ $ b_M $

- $ 1 $ 行目には、チェックポイントの数 $ N $ と、道路の数 $ M $ を空白区切りで出力してください。
- $ 2 $ 行目から $ M $ 行にわたって、道の情報を出力してください。ただし、$ a_i,\ b_i $ は、「$ i $ 番目の道路がチェックポイント $ a_i $ から $ b_i $ へ直接結ぶ」ことを表します。**このとき $ a_i\ <\ b_i $ でなければなりません。**
- 最後に改行をしてください。 ただし、**$ N $ は $ 200 $ 以下でなければなりません。** そうでない場合、Wrong Answer となります。  
  **また、$ (a_i,\ b_i)\ \neq\ (a_j,\ b_j)\ (i\ \neq\ j) $ かつ $ a_i\ <\ b_i $ でなければなりません。**

## 输入输出样例 #1

### 输入 #1

```
5
```

### 输出 #1

```
7 10
1 2
1 3
1 4
2 5
3 5
3 6
4 5
4 6
5 7
6 7
```

## 输入输出样例 #2

### 输入 #2

```
20
```

### 输出 #2

```
16 24
1 2
2 3
3 4
5 6
6 7
7 8
9 10
10 11
11 12
13 14
14 15
15 16
1 5
5 9
9 13
2 6
6 10
10 14
3 7
7 11
11 15
4 8
8 12
12 16
```

## 输入输出样例 #3

### 输入 #3

```
104
```

### 输出 #3

```
21 75
1 2
1 3
2 4
2 5
2 6
2 7
3 4
3 5
3 6
3 7
4 8
4 9
4 10
4 11
4 12
4 13
4 14
4 15
4 16
4 17
4 18
4 19
4 20
5 8
5 9
5 10
5 11
5 12
5 13
5 14
5 15
5 16
5 17
5 18
5 19
5 20
6 8
6 9
6 10
6 11
6 12
6 13
6 14
6 15
6 16
6 17
6 18
6 19
6 20
7 8
7 9
7 10
7 11
7 12
7 13
7 14
7 15
7 16
7 17
7 18
7 19
7 20
8 21
9 21
10 21
11 21
12 21
13 21
14 21
15 21
16 21
17 21
18 21
19 21
20 21
```

## 说明/提示

### 制約

- $ K $ は $ 1 $ 以上 $ 10^{18} $ 以下の整数

### 小課題

小課題 $ 1 $ \[$ 8 $ 点\]

- $ K\ \leq\ 150 $ を満たす。

小課題 $ 2 $ \[$ 12 $ 点\]

- $ K\ \leq\ 8\ 000 $ を満たす。

小課題 $ 3 $ \[$ 80 $ 点\]

- 追加の制約はない。

ただし、小課題 $ 3 $ について、採点は以下のように行われます。そこでは、$ L $ を「全てのテストケースにおける $ N $ の最大値」とします。

- $ 161\ \leq\ L\ \leq\ 200 $ の場合、$ 15 $ 点
- $ 152\ \leq\ L\ \leq\ 160 $ の場合、$ 55\ -\ (L\ -\ 150)\ *\ 2 $ 点
- $ L\ =\ 151 $ の場合、$ 65 $ 点
- $ L\ \leq\ 150 $ の場合、$ 80 $ 点満点

### Sample Explanation 1

以下の図において、チェックポイント $ 1 $ から $ 7 $ まで行くのに $ 5 $ 通りの方法が存在し、全て同じ本数 ($ 3 $ 本) の道路を通るため、条件を満たします。 !\[ \](https://img.atcoder.jp/pakencamp-2018-day2/457542e86b6cd161655104d58029b46e.png)

### Sample Explanation 2

以下の図において、チェックポイント $ 1 $ から $ 16 $ まで行くのに $ 20 $ 通りの方法が存在し、全て同じ本数 ($ 6 $ 本) の道路を通るため、条件を満たします。 !\[ \](https://img.atcoder.jp/pakencamp-2018-day2/e4a27202d79a6c7e86e60ae6e1d14799.png)

### Sample Explanation 3

この入力は、小課題 $ 1 $ の制約を満たします。