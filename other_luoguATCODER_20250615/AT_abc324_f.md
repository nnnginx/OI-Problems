# AT_abc324_f [ABC324F] Beautiful Path

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc324/tasks/abc324_f

$ N $ 個の頂点と $ M $ 本の辺からなる有向グラフがあります。各辺には**美しさ**と**コスト**の $ 2 $ つの正整数値が定められています。

$ i\ =\ 1,\ 2,\ \ldots,\ M $ について、$ i $ 番目の辺は頂点 $ u_i $ から頂点 $ v_i $ への有向辺であり、その美しさは $ b_i $ 、コストは $ c_i $ です。 ここで、$ u_i\ \lt\ v_i $ が制約として保証されます。

頂点 $ 1 $ から頂点 $ N $ へのパス $ P $ を $ 1 $ つ選んだときの、下記の値としてあり得る最大値を求めてください。

- $ P $ 上のすべての辺の美しさの総和を、$ P $ 上のすべての辺のコストの総和で割った値
 
ここで、与えられるグラフにおいて頂点 $ 1 $ から頂点 $ N $ へのパスが $ 1 $ 個以上存在することが制約として保証されます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ b_1 $ $ c_1 $ $ u_2 $ $ v_2 $ $ b_2 $ $ c_2 $ $ \vdots $ $ u_M $ $ v_M $ $ b_M $ $ c_M $

## 输出格式

答えを出力せよ。出力された値と真の値の相対誤差もしくは絶対誤差が $ 10^{-9} $ 以下のとき、正答と判定される。

## 输入输出样例 #1

### 输入 #1

```
5 7
1 2 3 6
1 3 9 5
2 3 1 5
2 4 5 3
2 5 1 9
3 4 4 8
4 5 2 7
```

### 输出 #1

```
0.7500000000000000
```

## 输入输出样例 #2

### 输入 #2

```
3 3
1 3 1 1
1 3 2 1
1 3 3 1
```

### 输出 #2

```
3.0000000000000000
```

## 输入输出样例 #3

### 输入 #3

```
10 20
3 4 1 2
7 9 4 5
2 4 4 5
4 5 1 4
6 9 4 1
9 10 3 2
6 10 5 5
5 6 1 2
5 6 5 2
2 3 2 3
6 10 4 4
4 6 3 4
4 8 4 1
3 5 3 2
2 4 3 2
3 5 4 2
1 5 3 4
1 2 4 2
3 7 2 2
7 8 1 3
```

### 输出 #3

```
1.8333333333333333
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i\ \lt\ v_i\ \leq\ N $
- $ 1\ \leq\ b_i,\ c_i\ \leq\ 10^4 $
- 頂点 $ 1 $ から頂点 $ N $ へのパスが存在する
- 入力される値はすべて整数
 
### Sample Explanation 1

パス $ P $ として、 $ 2,\ 6,\ 7 $ 番目の辺をこの順に通り頂点 $ 1\ \rightarrow\ 3\ \rightarrow\ 4\ \rightarrow\ 5 $ とたどるバスを選んだとき、「 $ P $ 上のすべての辺の美しさの総和を $ P $ 上のすべての辺のコストの総和で割った値」 は、 $ (b_2\ +\ b_6\ +\ b_7)\ /\ (c_2\ +\ c_6\ +\ c_7)\ =\ (9\ +\ 4\ +\ 2)\ /\ (5\ +\ 8\ +\ 7)\ =\ 15\ /\ 20\ =\ 0.75 $ であり、これがあり得る最大値です。