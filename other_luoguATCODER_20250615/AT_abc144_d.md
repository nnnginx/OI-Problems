# AT_abc144_d [ABC144D] Water Bottle

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc144/tasks/abc144_d

高橋君は、底面が $ 1 $ 辺 $ a~\mathrm{cm} $ の正方形であり、高さが $ b~\mathrm{cm} $ であるような直方体型の水筒を持っています。(水筒の厚みは無視できます。)

この水筒の中に体積 $ x~\mathrm{cm}^3 $ の水を入れ、底面の正方形の $ 1 $ 辺を軸として、この水筒を徐々に傾けます。

水を溢れさせずに水筒を傾けることができる最大の角度を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ x $

## 输出格式

水を溢れさせずに水筒を傾けることができる最大の角度を度数法で出力せよ。 出力は、ジャッジの出力との絶対誤差または相対誤差が $ 10^{-6} $ 以下のとき正解と判定される。

## 输入输出样例 #1

### 输入 #1

```
2 2 4
```

### 输出 #1

```
45.0000000000
```

## 输入输出样例 #2

### 输入 #2

```
12 21 10
```

### 输出 #2

```
89.7834636934
```

## 输入输出样例 #3

### 输入 #3

```
3 1 8
```

### 输出 #3

```
4.2363947991
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ <\ =\ a\ \leq\ 100 $
- $ 1\ <\ =\ b\ \leq\ 100 $
- $ 1\ <\ =\ x\ <\ =\ a^2b $

### Sample Explanation 1

水筒は立方体であり、水は半分まで入っています。この水筒を $ 45 $° より大きく傾けると水が溢れます。

### Sample Explanation 2

水筒はほぼ空であり、水が溢れるときにはほぼ水平になっています。

### Sample Explanation 3

水筒はほぼ満杯であり、ほぼ垂直の状態で水が溢れます。