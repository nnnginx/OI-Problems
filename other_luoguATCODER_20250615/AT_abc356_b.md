# AT_abc356_b [ABC356B] Nutrients

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc356/tasks/abc356_b

健康に気を使っている高橋君は、$ M $ 種類の栄養素について、食事によって十分な量を摂取できているか気になりました。

$ i $ 番目の栄養素は $ 1 $ 日あたり $ A_i $ 以上摂取することが目標です。

高橋君は今日 $ N $ 品の食品を食べ、$ i $ 品目の食品からは栄養素 $ j $ を $ X_{i,j} $ 摂取しました。

$ M $ 種類全ての栄養素で目標を達成しているかどうかを判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ \ldots $ $ A_M $ $ X_{1,1} $ $ \ldots $ $ X_{1,M} $ $ \vdots $ $ X_{N,1} $ $ \ldots $ $ X_{N,M} $

## 输出格式

$ M $ 種類全ての栄養素で目標を達成しているなら `Yes`、そうでないならば `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3
10 20 30
20 0 10
0 100 100
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
2 4
10 20 30 40
20 0 10 30
0 100 100 0
```

### 输出 #2

```
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ M\ \leq\ 100 $
- $ 0\ \leq\ A_i,X_{i,j}\ \leq\ 10^7 $
- 入力は全て整数である
 
### Sample Explanation 1

栄養素 $ 1 $ は $ 1 $ 品目から $ 20 $、$ 2 $ 品目から $ 0 $ 摂取したため、合わせて $ 20 $ 摂取しており、$ 10 $ 以上摂取するという目標を達成しています。 栄養素 $ 2,3 $ についても同様に目標を達成しています。

### Sample Explanation 2

栄養素 $ 4 $ について目標を達成していません。