# AT_abc192_e [ABC192E] Train

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc192/tasks/abc192_e

AtCoder国には $ 1 $ から $ N $ の番号がついた $ N $ 個の都市と、$ 1 $ から $ M $ の番号がついた $ M $ 本の鉄道があります。

鉄道 $ i $ は都市 $ A_i $ と都市 $ B_i $ の間を結んでおり、時刻が $ K_i $ の倍数になる毎に、双方の都市からそれぞれ他方の都市への列車が発車します。この列車は出発から到着までに $ T_i $ の時間がかかります。

あなたはいま都市 $ X $ にいます。時刻 $ 0 $ またはそれ以降に都市 $ X $ を発車する列車に乗って移動を開始するとき、都市 $ Y $ には最速でいつたどり着けるか求めてください。都市 $ Y $ にたどり着くことが出来ない場合はそのことを報告してください。  
 ただし、乗り換えにかかる時間は無視できるため、どの都市においても、あなたの乗っている列車の到着時刻と同時に発車する別の列車に乗り換えることが可能であるとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X $ $ Y $ $ A_1 $ $ B_1 $ $ T_1 $ $ K_1 $ $ \vdots $ $ A_M $ $ B_M $ $ T_M $ $ K_M $

## 输出格式

都市 $ Y $ にたどり着くことができる最も早い時刻を出力せよ。ただし、都市 $ Y $ にたどり着くことが出来ない場合はかわりに `-1` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2 1 3
1 2 2 3
2 3 3 4
```

### 输出 #1

```
7
```

## 输入输出样例 #2

### 输入 #2

```
3 2 3 1
1 2 2 3
2 3 3 4
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
3 0 3 1
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
9 14 6 7
3 1 4 1
5 9 2 6
5 3 5 8
9 7 9 3
2 3 8 4
6 2 6 4
3 8 3 2
7 9 5 2
8 4 1 9
7 1 6 9
3 9 9 3
7 5 1 5
8 2 9 7
4 9 4 4
```

### 输出 #4

```
26
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ X,Y\ \leq\ N $
- $ X\ \neq\ Y $
- $ 1\ \leq\ A_i,B_i\ \leq\ N $
- $ A_i\ \neq\ B_i $
- $ 1\ \leq\ T_i\ \leq\ 10^9 $
- $ 1\ \leq\ K_i\ \leq\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

まず、時刻 $ 0 $ に鉄道 $ 1 $ に乗って、都市 $ 1 $ から都市 $ 2 $ へ移動します。都市 $ 2 $ には時刻 $ 2 $ に到着します。 その後、時刻 $ 4 $ に鉄道 $ 2 $ に乗って、都市 $ 2 $ から都市 $ 3 $ へ移動します。都市 $ 3 $ には時刻 $ 7 $ に到着します。 これより早く都市 $ 3 $ に着く方法はありません。

### Sample Explanation 2

まず、時刻 $ 0 $ に鉄道 $ 2 $ に乗って、都市 $ 3 $ から都市 $ 2 $ へ移動します。都市 $ 2 $ には時刻 $ 3 $ に到着します。 その後、時刻 $ 3 $ に鉄道 $ 1 $ に乗って、都市 $ 2 $ から都市 $ 1 $ へ移動します。都市 $ 1 $ には時刻 $ 5 $ に到着します。