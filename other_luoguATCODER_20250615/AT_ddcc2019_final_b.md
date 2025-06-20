# AT_ddcc2019_final_b 大吉数列 (Array of Fortune)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ddcc2019-final/tasks/ddcc2019_final_b

以下の条件を満たす長さ $ N $ の数列 $ A $ = {$ A_1,\ A_2,\ A_3,\ ...,\ A_N $} を「大吉数列」とします。

- $ A $ には $ 1 $ 以上 $ N $ 以下の整数がちょうど $ 1 $ 回ずつ出現する。
- $ a_i\ \geq\ a_j\ +\ K $ を満たす $ (i,\ j) $ の組 ($ i\ <\ j $) がちょうど $ R $ 個存在する。

数列君は、大吉数列を見つけようと思いましたが、すぐには見つけられませんでした。  
 彼のために、大吉数列を $ 1 $ つ構成してください。  
 大吉数列が $ 1 $ つも存在しない場合は、`No Luck` と出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ R $

## 输出格式

大吉数列が存在しない場合、`No Luck` と出力せよ。  
 大吉数列が存在する場合、大吉数列として考えられるものを以下の形式で $ 1 $ つ出力せよ。

> $ A_1 $ $ A_2 $ $ A_3 $ $ ... $ $ A_N $

大吉数列が複数存在する場合は、そのうちのどれを出力しても正解となる。

## 输入输出样例 #1

### 输入 #1

```
5 2 4
```

### 输出 #1

```
3 4 1 5 2
```

## 输入输出样例 #2

### 输入 #2

```
7 1 21
```

### 输出 #2

```
7 6 5 4 3 2 1
```

## 输入输出样例 #3

### 输入 #3

```
10 3 22
```

### 输出 #3

```
6 7 8 9 10 1 2 3 4 5
```

## 输入输出样例 #4

### 输入 #4

```
10 5 45
```

### 输出 #4

```
No Luck
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100\ 000 $
- $ 1\ \leq\ K\ \leq\ N\ -\ 1 $
- $ 0\ \leq\ R\ \leq\ N\ \times\ (N\ -\ 1)\ /\ 2 $
- 入力値はすべて整数

### 小課題

この問題は小課題に分けられている。

小課題 $ 1 $ \[$ 200 $ 点\]

- $ N\ \leq\ 100 $ を満たす。

小課題 $ 2 $ \[$ 400 $ 点\]

- 追加の制約はない。

### Sample Explanation 1

数列 $ A\ =\ {3,\ 4,\ 1,\ 5,\ 2} $ に対して、$ a_i\ \geq\ a_j\ +\ 2 $ を満たす $ (i,\ j) $ の組 $ (i\ <\ j) $ は以下のちょうど $ 4 $ 個存在します。 - $ (i,\ j)\ =\ (1,\ 3),\ (2,\ 3),\ (2,\ 5),\ (4,\ 5) $ よって、数列 $ A $ は大吉数列の一つです。 この他に、例えば以下のような出力も正解となります。 ``` 5 1 3 4 2 ```