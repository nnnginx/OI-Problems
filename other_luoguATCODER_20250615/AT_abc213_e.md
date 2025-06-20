# AT_abc213_e [ABC213E] Stronger Takahashi

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc213/tasks/abc213_e

$ H $ 行 $ W $ 列の格子状の区画に区切られた街があります。上から $ i $ 行目、左から $ j $ 列目の区画は、$ S_{i,j} $ が `.` のとき道、`#` のとき塀です。

高橋君は自分の家から魚屋に買い物に行くことにしました。高橋君の家は街の左上隅の区画にあり、魚屋は街の右下隅の区画にあります。

高橋君は、自分がいる区画から上下左右に隣接する道の区画に移動することができます。街の外に出ることはできません。  
 塀の区画に移動することはできませんが、高橋君は非常に腕力が強いため、パンチを $ 1 $ 回繰り出すことで任意の $ 2\times\ 2 $ の区画内の塀を壊して道にすることができます。

高橋君が魚屋にたどり着くためには、最低何回パンチを繰り出せばよいか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_{1,1}\ \ldots\ S_{1,W} $ $ \vdots $ $ S_{H,1}\ \ldots\ S_{H,W} $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 5
..#..
#.#.#
##.##
#.#.#
..#..
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
5 7
.......
######.
.......
.######
.......
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8 8
.#######
########
########
########
########
########
########
#######.
```

### 输出 #3

```
5
```

## 说明/提示

### 制約

- $ 2\ \leq\ H,W\ \leq\ 500 $
- $ H,W $ は整数
- $ S_{i,j} $ は `.` または `#`
- $ S_{1,1} $ と $ S_{H,W} $ は `.`

### Sample Explanation 1

例えば、以下の `\*` で表す $ 2\times\ 2 $ の区画にある塀を破壊すると魚屋にたどり着くことができます。 ``` ..#.. #.\*\*# ##\*\*# #.#.# ..#.. ``` 破壊対象の $ 2\ \times\ 2 $ の区画の全てが塀である必要はありません。

### Sample Explanation 2

遠回りが必要ですが、塀を破壊することなく魚屋にたどり着くことができます。