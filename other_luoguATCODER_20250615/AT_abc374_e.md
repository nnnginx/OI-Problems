# AT_abc374_e [ABC374E] Sensor Optimization Dilemma 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc374/tasks/abc374_e

ある製品の製造には $ 1,2,\dots,N $ の番号が付いた $ N $ 個の工程が必要です。

各工程 $ i $ について、それを処理する $ 2 $ 種類の機械 $ S_i,T_i $ が売られています。

- 機械 $ S_i $ : $ 1 $ 台につき $ 1 $ 日あたり製品 $ A_i $ 個分の処理ができ、 $ 1 $ 台 $ P_i $ 円で導入できる
- 機械 $ T_i $ : $ 1 $ 台につき $ 1 $ 日あたり製品 $ B_i $ 個分の処理ができ、 $ 1 $ 台 $ Q_i $ 円で導入できる

それぞれの機械は $ 0 $ 台以上何台でも導入できます。

機械の導入の結果、工程 $ i $ を $ 1 $ 日あたり製品 $ W_i $ 個分処理できるようになったとします。  
このとき、製造能力を $ W $ の最小値、すなわち $ \displaystyle\ \min^{N}_{i=1}\ W_i $ と定義します。

全体の予算が $ X $ 円のとき、達成可能な製造能力の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ A_1 $ $ P_1 $ $ B_1 $ $ Q_1 $ $ A_2 $ $ P_2 $ $ B_2 $ $ Q_2 $ $ \vdots $ $ A_N $ $ P_N $ $ B_N $ $ Q_N $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 22
2 5 3 6
1 1 3 3
1 3 2 4
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
1 10000000
100 1 100 1
```

### 输出 #2

```
1000000000
```

## 输入输出样例 #3

### 输入 #3

```
1 1
1 10000000 1 10000000
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
10 7654321
8 6 9 1
5 6 4 3
2 4 7 9
7 8 9 1
7 9 1 6
4 8 9 1
2 2 8 9
1 6 2 6
4 2 3 4
6 6 5 2
```

### 输出 #4

```
894742
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ N\ \le\ 100 $
- $ 1\ \le\ A_i,B_i\ \le\ 100 $
- $ 1\ \le\ P_i,Q_i,X\ \le\ 10^7 $

### Sample Explanation 1

例えば、次の通り機械を導入することで製造能力を $ 4 $ にすることができ、これが達成可能な最大値です。 - 工程 $ 1 $ に対し機械 $ S_1 $ を $ 2 $ 台導入する。 - $ 1 $ 日あたり製品 $ 4 $ 個分の処理に相当し、導入に合計 $ 10 $ 円かかる。 - 工程 $ 2 $ に対し機械 $ S_2 $ を $ 1 $ 台導入する。 - $ 1 $ 日あたり製品 $ 1 $ 個分の処理に相当し、導入に合計 $ 1 $ 円かかる。 - 工程 $ 2 $ に対し機械 $ T_2 $ を $ 1 $ 台導入する。 - $ 1 $ 日あたり製品 $ 3 $ 個分の処理に相当し、導入に合計 $ 3 $ 円かかる。 - 工程 $ 3 $ に対し機械 $ T_3 $ を $ 2 $ 台導入する。 - $ 1 $ 日あたり製品 $ 4 $ 個分の処理に相当し、導入に合計 $ 8 $ 円かかる。

### Sample Explanation 3

正の製造能力が得られない場合もあります。