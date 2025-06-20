# AT_keyence2019_d Double Landscape

## 题目描述

[problemUrl]: https://atcoder.jp/contests/keyence2019/tasks/keyence2019_d

$ N $ 行 $ M $ 列のグリッドに，$ 1 $ から $ N\ \times\ M $ までの整数を重複のないように $ 1 $ つずつ書き込むことを考えます． ここで，普通に書き込むのでは面白くないと思った高橋君は，以下の条件を満たすように数を書き込むことにしました．

- $ i $ 行目に書き込まれている値のうち，最大の値は $ A_i $ $ (1\ \leq\ i\ \leq\ N) $
- $ j $ 列目に書き込まれている値のうち，最大の値は $ B_j $ $ (1\ \leq\ j\ \leq\ M) $

高橋君のために，この条件を満たすような書き込み方の個数を $ 10^9\ +\ 7 $ で割ったあまりを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ ... $ $ A_{N} $ $ B_1 $ $ B_2 $ $ ... $ $ B_{M} $

## 输出格式

条件を満たすような書き込み方の個数を $ 10^9\ +\ 7 $ で割ったあまりを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2 2
4 3
3 4
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3 3
5 9 7
3 6 9
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
2 2
4 4
4 4
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
14 13
158 167 181 147 178 151 179 182 176 169 180 129 175 168
181 150 178 179 167 180 176 169 182 177 175 159 173
```

### 输出 #4

```
343772227
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ M\ \leq\ 1000 $
- $ 1\ \leq\ A_i\ \leq\ N\ \times\ M $
- $ 1\ \leq\ B_j\ \leq\ N\ \times\ M $
- $ A_i,\ B_j $ は整数

### Sample Explanation 1

$ (A_1,\ A_2)\ =\ (4,\ 3) $，$ (B_1,\ B_2)\ =\ (3,\ 4) $ であり，この場合は以下の $ 2 $ 通りの書き込み方があります． - $ 1 $ 行 $ 1 $ 列目に $ 1 $，$ 1 $ 行 $ 2 $ 列目に $ 4 $，$ 2 $ 行 $ 1 $ 列目に $ 3 $，$ 2 $ 行 $ 2 $ 列目に $ 2 $ - $ 1 $ 行 $ 1 $ 列目に $ 2 $，$ 1 $ 行 $ 2 $ 列目に $ 4 $，$ 2 $ 行 $ 1 $ 列目に $ 3 $，$ 2 $ 行 $ 2 $ 列目に $ 1 $

### Sample Explanation 2

どのような書き込み方をしても条件を満たすことができないので，$ 0 $ を出力します．