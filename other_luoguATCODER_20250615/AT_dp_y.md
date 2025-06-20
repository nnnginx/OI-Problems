# AT_dp_y Grid 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_y

縦 $ H $ 行、横 $ W $ 列のグリッドがあります。 上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,\ j) $ で表します。

グリッドのうち、$ N $ 個のマス $ (r_1,\ c_1),\ (r_2,\ c_2),\ \ldots,\ (r_N,\ c_N) $ は壁のマスであり、それら以外のマスはすべて空マスです。 マス $ (1,\ 1) $ および $ (H,\ W) $ は空マスであることが保証されています。

太郎君は、マス $ (1,\ 1) $ から出発し、右または下に隣り合う空マスへの移動を繰り返すことで、マス $ (H,\ W) $ まで辿り着こうとしています。

マス $ (1,\ 1) $ から $ (H,\ W) $ までの太郎君の経路は何通りでしょうか？ $ 10^9\ +\ 7 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ N $ $ r_1 $ $ c_1 $ $ r_2 $ $ c_2 $ $ : $ $ r_N $ $ c_N $

## 输出格式

マス $ (1,\ 1) $ から $ (H,\ W) $ までの太郎君の経路は何通りか？ $ 10^9\ +\ 7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 4 2
2 2
1 4
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5 2 2
2 1
4 2
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
5 5 4
3 1
3 5
1 3
5 3
```

### 输出 #3

```
24
```

## 输入输出样例 #4

### 输入 #4

```
100000 100000 1
50000 50000
```

### 输出 #4

```
123445622
```

## 说明/提示

### 制約

- 入力はすべて整数である。
- $ 2\ \leq\ H,\ W\ \leq\ 10^5 $
- $ 1\ \leq\ N\ \leq\ 3000 $
- $ 1\ \leq\ r_i\ \leq\ H $
- $ 1\ \leq\ c_i\ \leq\ W $
- マス $ (r_i,\ c_i) $ はすべて相異なる。
- マス $ (1,\ 1) $ および $ (H,\ W) $ は空マスである。

### Sample Explanation 1

経路は次図の $ 3 $ 通りです。 !\[\](https://img.atcoder.jp/dp/grid\_1\_0\_muffet.png)

### Sample Explanation 2

経路が存在しない場合もあります。

### Sample Explanation 4

答えを $ 10^9\ +\ 7 $ で割った余りを出力することを忘れずに。