# AT_utpc2020_a Row of Tents

## 题目描述

[problemUrl]: https://atcoder.jp/contests/utpc2020/tasks/utpc2020_a

 UT 大学にはテント列というサークル紹介イベントがあります。長さ $ L $ の道があり、 umg くんは位置 $ 0 $ から位置 $ L $ まで一方通行で歩きます。 umg くんには気力というパラメータがあり、その初期値を $ T $ とします。ここで、$ T $ は整数値とします。 umg くんは、距離 $ 1 $ 歩くごとに、気力が $ T $ 未満である場合は 気力が $ 1 $ 回復します。気力が $ T $ である場合は回復しません。

道上には $ N $ 個のテントがあり、$ i $ 番目のテントは位置 $ X_i $ にあります。 umg くんは $ i $ 番目のテントに着くとサークル勧誘にあい、気力が $ A_i $ 減少します。もしここで気力が $ 0 $ 未満になると、 umg くんはその場で倒れてしまいます。

 umg くんが途中で倒れずに位置 $ L $ までたどり着くのに必要な、気力の初期値 $ T $ の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ L $ $ X_1 $ $ A_1 $ $ X_2 $ $ A_2 $ $ \vdots $ $ X_N $ $ A_N $

## 输出格式

答えを $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 7
1 5
4 4
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
8 11
2 6
3 10
4 8
5 7
7 7
8 1
9 9
10 2
```

### 输出 #2

```
42
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ N\ \lt\ L\ \leq\ 10^9 $
- $ 0\lt\ X_1\ \lt\ X_2\ \lt\ \cdots\ \lt\ X_N\ \lt\ L $
- $ 1\ \leq\ A_i\ \leq\ 10^9\ (1\leq\ i\ \leq\ N) $

### Sample Explanation 1

気力の初期値 $ T=6 $ でスタートした場合は以下のような気力の変動になります。 - $ 1 $ 番目のテントにたどり着いて気力が $ 5 $ 減少し、気力が $ 1 $ になる。 - $ 2 $ 番目のテントにたどり着くまでに気力が $ 3 $ 回復し、気力が $ 4 $ になる。 - $ 2 $ 番目のテントにたどり着いて気力が $ 4 $ 減少し、気力が $ 0 $ になる。 - 位置 $ 7 $ にたどり着くまでに気力が $ 3 $ 回復し、気力 $ 3 $ の状態でテント列を終える。 気力の初期値 $ T=5 $ でスタートすると、$ 2 $ 番目のテントで気力が $ 0 $ 未満になってしまうので、答えは $ 6 $ となります。