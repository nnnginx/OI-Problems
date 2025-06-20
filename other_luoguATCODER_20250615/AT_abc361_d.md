# AT_abc361_d [ABC361D] Go Stone Puzzle

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc361/tasks/abc361_d

$ N+2 $ 個のマスが横一列に並んでいます。左から $ i $ 番目のマスをマス $ i $ と表します。

マス $ 1 $ からマス $ N $ には石が $ 1 $ 個ずつ置かれています。  
 各 $ 1\leq\ i\ \leq\ N $ について、$ S_i $ が `W` のときマス $ i $ に置かれている石の色は白であり、$ S_i $ が `B` のときマス $ i $ に置かれている石の色は黒です。  
 マス $ N+1,N+2 $ には何も置かれていません。

あなたは以下の操作を好きな回数($ 0 $ 回でもよい)行うことができます。

- 石が $ 2 $ 個並んでいる箇所を選び、その $ 2 $ 個の石を順序を保って空きマスに移す。  
   より正確には次の通り。$ 1 $ 以上 $ N+1 $ 以下の整数 $ x $ であって、マス $ x,x+1 $ の両方に石が置かれているものを選ぶ。石の置かれていないマスを $ k,k+1 $ とする。マス $ x,x+1 $ にある石をそれぞれマス $ k,k+1 $ に移動する。
 
以下の状態にすることが可能か判定し、可能なら操作回数の最小値を求めてください。

- マス $ 1 $ からマス $ N $ には石が $ 1 $ 個ずつ置かれており、各 $ 1\leq\ i\ \leq\ N $ について、$ T_i $ が `W` のときマス $ i $ に置かれている石の色は白、$ T_i $ が `B` のときマス $ i $ に置かれている石の色は黒である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ T $

## 输出格式

目的の状態にすることが可能なら操作回数の最小値を出力せよ。不可能ならかわりに `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
BWBWBW
WWWBBB
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
6
BBBBBB
WWWWWW
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
14
BBBWBWWWBBWWBW
WBWWBBWWWBWBBB
```

### 输出 #3

```
7
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 14 $
- $ N $ は整数である
- $ S,T $ は `B` および `W` のみからなる長さ $ N $ の文字列である
 
### Sample Explanation 1

石が置かれていないマスを `.` と表します。以下のようにして $ 4 $ 回の操作で目的の状態にすることができ、これが最小回数です。 - `BWBWBW..` - `BW..BWBW` - `BWWBB..W` - `..WBBBWW` - `WWWBBB..`