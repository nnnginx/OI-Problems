# AT_agc022_f [AGC022F] Checkers

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc022/tasks/agc022_f

$ X\ =\ 10^{100} $ とします。イナバは $ N $ 個の駒を数直線上に置いていて、$ i $ 個目の駒は座標 $ X^{i} $ にあります。

$ 1 $ 秒ごとに、イナバは $ 2 $ 個の駒 $ A $、$ B $ を選び、$ A $ を $ B $ に関して対称な点に動かし、その後 $ B $ を取り除きます（$ A $、$ B $ が同じ位置にあっても構わず、$ A $ が移動後に他の駒と同じ位置にあっても構いません）。

$ N\ -\ 1 $ 秒後には、駒が $ 1 $ 個だけ残ります。その駒の位置としてありうるものは何通りあるか、その数を $ 10^{9}\ +\ 7 $ で割った余りを求めてください。

## 输入格式

入力は標準入力から以下の形式で与えられる。

> $ N $

## 输出格式

最後に残る駒の位置としてありうるものの数を $ 10^{9}\ +\ 7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
```

### 输出 #1

```
12
```

## 输入输出样例 #2

### 输入 #2

```
4
```

### 输出 #2

```
84
```

## 输入输出样例 #3

### 输入 #3

```
22
```

### 输出 #3

```
487772376
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ N $ は整数である。

### Sample Explanation 1

駒が $ 3 $ 個あり、それぞれ座標 $ 10^{100},\ 10^{200},\ 10^{300} $ に置かれています。これらをそれぞれ $ A $、$ B $、$ C $ と呼びます。 考えられる駒の動かし方（$ 12 $ 通り）のうち $ 2 $ つを示します。 - 最初の $ 1 $ 秒で $ A $ に $ B $ を飛び越えさせ、次の $ 1 $ 秒で $ A $ に $ C $ を飛び越えさせる。$ A $ の最終的な位置は $ 2\ \times\ 10^{300}\ -\ 2\ \times\ 10^{200}\ +\ 10^{100} $ となる。 - 最初の $ 1 $ 秒で $ C $ に $ A $ を飛び越えさせ、次の $ 1 $ 秒で $ B $ に $ C $ を飛び越えさせる。$ B $ の最終的な位置は $ -2\ \times\ 10^{300}\ -\ 10^{200}\ +\ 4\ \times\ 10^{100} $ となる。 駒の動かし方は合計で $ 3\ \times\ 2\ \times\ 2\ =\ 12 $ 通りあり、そのすべてで最後の駒は異なる位置に残ります。

### Sample Explanation 3

答えを $ 10^{9}\ +\ 7 $ で割った余りを出力することを忘れずに。