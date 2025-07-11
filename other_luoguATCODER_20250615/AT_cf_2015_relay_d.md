# AT_cf_2015_relay_d ピザ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-relay/tasks/cf_2015_relay_d

二等辺三角形の形をしたピザを切って $ N $ 人に配分します。 ピザは底辺と平行な等間隔の直線で切ります。 すると各ピースの面積比は $ 1:3:5:... $ となります。 それぞれの人にいくつかのピースを配って同じ面積になるようにした時、ピザは少なくともいくつのピースに分割する必要があるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

- $ 1 $ 行目には、人数を表す整数 $ N\ (1\ ≦\ N\ ≦\ 1,000) $ が与えられる。

## 输出格式

ピザを少なくともいくつのピースに分割する必要があるかを $ 1 $ 行に出力せよ。出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
2
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
3
```

### 输出 #3

```
6
```

## 说明/提示

### Sample Explanation 1

$ 1 $ 人に配る場合は、$ 1 $ つのピースのままで良いです。

### Sample Explanation 2

$ 1 $ 人目に面積比が $ 3 $ と $ 5 $ のピースを、$ 2 $ 人目に面積比が $ 1 $ と $ 7 $ のピースを配ると、面積が等しくなります。