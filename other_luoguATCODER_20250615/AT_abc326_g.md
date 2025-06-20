# AT_abc326_g [ABC326G] Unlock Achievement

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc326/tasks/abc326_g

$ 1 $ から $ N $ の番号がついた $ N $ 種類のスキルと、$ 1 $ から $ M $ の番号がついた $ M $ 種類のアチーブメントがあります。

各スキルには正整数のレベルが定まっており、最初全てのスキルのレベルは $ 1 $ です。

$ C_i $ 円のコストを払うことでスキル $ i $ のレベルを $ 1 $ 上げることができます。これは何度でも行なえます。

アチーブメント $ i $ は、$ j=1,\ldots,N $ の全てについて以下の条件を満たすと達成となり、$ A_i $ 円の報酬をもらえます。

- 条件：スキル $ j $ のレベルが $ L_{i,j} $ 以上である
 
スキルのレベルの上げ方を適切に選ぶとき、得られる報酬の合計から必要なコストの合計を引いた値の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ C_1 $ $ \ldots $ $ C_N $ $ A_1 $ $ \ldots $ $ A_M $ $ L_{1,1} $ $ \ldots $ $ L_{1,N} $ $ \vdots $ $ L_{M,1} $ $ \ldots $ $ L_{M,N} $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 2
10 20
100 50
3 1
1 4
```

### 输出 #1

```
80
```

## 输入输出样例 #2

### 输入 #2

```
2 2
10 20
100 50
3 2
1 4
```

### 输出 #2

```
70
```

## 输入输出样例 #3

### 输入 #3

```
10 10
10922 23173 32300 22555 29525 16786 3135 17046 11245 20310
177874 168698 202247 31339 10336 14825 56835 6497 12440 110702
2 1 4 1 3 4 4 5 1 4
2 3 4 4 5 3 5 5 2 3
2 3 5 1 4 2 2 2 2 5
3 5 5 3 5 2 2 1 5 4
3 1 1 4 4 1 1 5 3 1
1 2 3 2 4 2 4 3 3 1
4 4 4 2 5 1 4 2 2 2
5 3 1 2 3 4 2 5 2 2
5 4 3 4 3 1 5 1 5 4
2 3 2 5 2 3 1 2 2 4
```

### 输出 #3

```
66900
```

## 说明/提示

### 制約

- $ 1\ \leq\ N,M\ \leq\ 50 $
- $ 1\ \leq\ L_{i,j}\ \leq\ 5 $
- $ 1\ \leq\ A_i,C_i\ \leq\ 10^6 $
- 入力は全て整数である
 
### Sample Explanation 1

$ 2 $ 種類のスキルがあります。スキル $ 1 $ はレベルを上げるために $ 10 $ 円、スキル $ 2 $ は $ 20 $ 円かかります。 $ 2 $ 種類のアチーブメントがあります。 アチーブメント $ 1 $ は「スキル $ 1 $ をレベル $ 3 $ 以上、かつ、スキル $ 2 $ をレベル $ 1 $ 以上」にすると達成となり $ 100 $ 円もらえ、 アチーブメント $ 2 $ は「スキル $ 1 $ をレベル $ 1 $ 以上、かつ、スキル $ 2 $ をレベル $ 4 $ 以上」にすると達成となり $ 50 $ 円もらえます。 スキル $ 1 $ をレベル $ 3 $ に、スキル $ 2 $ をレベル $ 1 $ にすることで、報酬が $ 100 $ 円、コストが $ 20 $ 円となり、その差は $ 80 $ 円となります。

### Sample Explanation 2

スキル $ 1 $ をレベル $ 3 $ に、スキル $ 2 $ をレベル $ 4 $ にすることで、報酬が $ 150 $ 円、コストが $ 80 $ 円となり、その差は $ 70 $ 円となります。