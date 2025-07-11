# AT_abc228_c [ABC228C] Final Day

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc228/tasks/abc228_c

$ N $ 人の生徒が $ 4 $ 日間にわたる試験を受けています。

それぞれの日に行われる試験は $ 300 $ 点満点です。すなわち、$ 4 $ 日間を通した試験の満点は $ 1200 $ 点です。

現在 $ 3 $ 日目までの試験が終わり、これから $ 4 $ 日目の試験が行われようとしています。$ i\ \,\ (1\ \leq\ i\ \leq\ N) $ 番目の生徒は $ j\ \,\ (1\ \leq\ j\ \leq\ 3) $ 日目の試験で $ P_{i,\ j} $ 点獲得しました。

それぞれの生徒について、$ 4 $ 日目の試験後に上位 $ K $ 位以内に入っていることがあり得るかどうか判定してください。  
 ただし、$ 4 $ 日目の試験後の生徒の順位は、その生徒よりも $ 4 $ 日間の合計点が高い生徒の人数に $ 1 $ を加えた値として定めます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ P_{1,1} $ $ P_{1,2} $ $ P_{1,3} $ $ \vdots $ $ P_{N,1} $ $ P_{N,2} $ $ P_{N,3} $

## 输出格式

$ N $ 行出力せよ。$ i\ \,\ (1 \leq\ i\ \leq\ N) $ 行目には、$ i $ 番目の生徒が $ 4 $ 日目の試験後に上位 $ K $ 位以内に入っていることがあり得るならば `Yes` と、そうでないならば `No` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 1
178 205 132
112 220 96
36 64 20
```

### 输出 #1

```
Yes
Yes
No
```

## 输入输出样例 #2

### 输入 #2

```
2 1
300 300 300
200 200 200
```

### 输出 #2

```
Yes
Yes
```

## 输入输出样例 #3

### 输入 #3

```
4 2
127 235 78
192 134 298
28 56 42
96 120 250
```

### 输出 #3

```
Yes
Yes
No
Yes
```

## 说明/提示

### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 10^5 $
- $ 0\ \leq\ P_{i,\ j}\ \leq\ 300\ \,\ (1\ \leq\ i\ \leq\ N,\ 1\ \leq\ j\ \leq\ 3) $
- 入力は全て整数である。

### Sample Explanation 1

$ 4 $ 日目に全員が $ 100 $ 点を取ると、$ 1 $ 番目の生徒が $ 1 $ 位になります。 $ 4 $ 日目に $ 2 $ 番目の生徒が $ 100 $ 点を取り、それ以外の生徒が $ 0 $ 点を取ると、$ 2 $ 番目の生徒が $ 1 $ 位になります。 $ 3 $ 番目の生徒が $ 1 $ 位になることはあり得ません。