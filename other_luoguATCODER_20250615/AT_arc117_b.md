# AT_arc117_b [ARC117B] ARC Wrecker

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc117/tasks/arc117_b

AtCoder 街道には $ N $ 個のビルが建設されています。最初、左から $ i $ 番目のビルは $ A_i $ 階建てです。

ARC 解体業者の社長である高橋君は、以下の操作を好きな回数だけ行うことができます。$ 1 $ 回も操作を行わないことも可能です。

- 好きな正の整数 $ X $ を選び、$ X $ 階の高さから大砲を発射する。そのとき、現時点で $ X $ 階建て以上であるすべてのビルについて、階数が $ 1 $ 減少する。

あり得る最終的なビルの景観の数を $ 10^{9}\ +\ 7 $ で割った余りを求めてください。

ただし、景観 A と景観 B が異なるとは、以下のことを指します。

- 景観 A における、左から $ i $ 番目のビルの高さを $ P_i $ とする。
- 景観 B における、左から $ i $ 番目のビルの高さを $ Q_i $ とする。
- $ P_i\ \neq\ Q_i $ となる $ i $ が $ 1 $ つでも存在する場合、景観 A と景観 B は異なる。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

答えを出力してください。

## 输入输出样例 #1

### 输入 #1

```
2
1 2
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
6
5 3 4 1 5 2
```

### 输出 #2

```
32
```

## 输入输出样例 #3

### 输入 #3

```
7
314 159 265 358 979 323 846
```

### 输出 #3

```
492018656
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100000 $
- $ 1\ \leq\ A_i\ \leq\ 10^{9} $
- 入力はすべて整数

### Sample Explanation 1

操作後のビルの高さとしてあり得るものは、以下の $ 4 $ 通りです。 - (ビル $ 1 $ の階数, ビル $ 2 $ の階数) = $ (0,\ 0) $ - (ビル $ 1 $ の階数, ビル $ 2 $ の階数) = $ (0,\ 1) $ - (ビル $ 1 $ の階数, ビル $ 2 $ の階数) = $ (1,\ 1) $ - (ビル $ 1 $ の階数, ビル $ 2 $ の階数) = $ (1,\ 2) $

### Sample Explanation 3

全部で $ 20192492160000 $ 通りの景観があり得ますが、それを $ 10^{9}\ +\ 7 $ で割った余りである $ 492018656 $ を出力すると正解になります。