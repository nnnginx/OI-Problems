# AT_abc375_g [ABC375G] Road Blocked 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc375/tasks/abc375_g

AtCoder国には $ 1 $ から $ N $ の番号がついた $ N $ 個の都市と、$ 1 $ から $ M $ の番号がついた $ M $ 本の道路があります。  
 道路 $ i $ は都市 $ A_i $ と都市 $ B_i $ を双方向に結び長さは $ C_i $ です。

各 $ i=1,\ldots,M $ について、以下の $ 2 $ つの値が異なるかどうか判定してください。

- 全ての道路が通行可能なときの、都市 $ 1 $ から都市 $ N $ への最短距離
- 道路 $ i $ 以外の $ M-1 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ N $ への最短距離
 
ただし、一方では都市 $ 1 $ から都市 $ N $ に到達可能で、他方では到達不可能なとき、両者の値は異なるとみなします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ C_1 $ $ \vdots $ $ A_M $ $ B_M $ $ C_M $

## 输出格式

$ M $ 行出力せよ。$ i $ 行目には、「全ての道路が通行可能なときの、都市 $ 1 $ から都市 $ N $ への最短距離」と「道路 $ i $ 以外の $ M-1 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ N $ への最短距離」が異なるとき `Yes`、同じとき `No` と出力せよ。

ただし、一方では都市 $ 1 $ から都市 $ N $ に到達可能で、他方では到達不可能なとき、両者の値は異なるとみなす。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 2 5
1 3 10
2 3 6
```

### 输出 #1

```
No
Yes
No
```

## 输入输出样例 #2

### 输入 #2

```
4 6
2 3 1
2 4 1
3 4 1
1 2 1
1 3 1
1 4 1
```

### 输出 #2

```
No
No
No
No
No
Yes
```

## 输入输出样例 #3

### 输入 #3

```
2 1
1 2 1
```

### 输出 #3

```
Yes
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 2\times\ 10^5 $
- $ 1\leq\ A_i\ <\ B_i\ \leq\ N $
- $ (A_i,B_i) $ は相異なる
- $ 1\ \leq\ C_i\ \leq\ 10^9 $
- 全ての道路が通行可能なとき、都市 $ 1 $ から都市 $ N $ へは到達可能
- 入力は全ては整数である
 
### Sample Explanation 1

全ての道路が通行可能なとき、都市 $ 1 $ から都市 $ 3 $ への最短距離は $ 10 $ です。 - 道路 $ 1 $ 以外の $ 2 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ 3 $ への最短距離 は $ 10 $ です - 道路 $ 2 $ 以外の $ 2 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ 3 $ への最短距離 は $ 11 $ です - 道路 $ 3 $ 以外の $ 2 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ 3 $ への最短距離 は $ 10 $ です

### Sample Explanation 2

全ての道路が通行可能なとき、都市 $ 1 $ から都市 $ 4 $ への最短距離は $ 1 $ です。 道路 $ 6 $ 以外の $ 5 $ 本の道路が通行可能なときの、都市 $ 1 $ から都市 $ 4 $ への最短距離 は $ 2 $ です。

### Sample Explanation 3

道路 $ 1 $ 以外の $ 0 $ 本の道路が通行可能なとき、都市 $ 1 $ から都市 $ 2 $ へは到達できません。