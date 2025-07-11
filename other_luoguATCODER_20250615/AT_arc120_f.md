# AT_arc120_f [ARC120F] Wine Thief

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc120/tasks/arc120_f

**問題 F と問題 F2 は同じ問題ですが、制約と実行時間制限が異なります。**

高橋君の倉庫には $ N $ 本のワインがあり、左右方向 $ 1 $ 列に並んでいます。左から $ i $ 番目のワインの美味しさは $ A_i $ です。  
 青木君は今からこの $ N $ 本のうち、ちょうど $ K $ 本を選んで盗みます。しかし、高橋君は注意深いので、以下の条件が満たされると盗まれたことに気付いてしまいます。

- 連続で並ぶ $ D $ 本のワインであって、そのうち $ 2 $ 本以上盗まれているようなものが存在する (この問題では $ D\ =\ 2 $ です)

高橋君に気付かれないような全ての盗み方について、盗んだワインの美味しさの和を求め、それを足し合わせた値を求めてください。  
 なお、答えは非常に大きくなることがあるので、$ 998244353 $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ D $ $ A_1 $ $ A_2 $ $ A_3 $ $ \dots $ $ A_N $

## 输出格式

答えを $ 998244353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 2 2
1 4 2 3
```

### 输出 #1

```
14
```

## 输入输出样例 #2

### 输入 #2

```
5 3 2
4 7 5 3 8
```

### 输出 #2

```
17
```

## 输入输出样例 #3

### 输入 #3

```
12 4 2
107367523 266126484 149762920 57456082 857431610 400422663 768881284 494753774 152155823 740238343 871191740 450057094
```

### 输出 #3

```
136993014
```

## 说明/提示

### 制約

- $ D\ =\ 2 $
- $ 2\ \le\ N\ \le\ 3\ \times\ 10^5 $
- $ 1\ \le\ K\ \le\ \left\lceil\ \frac{N}{D}\ \right\rceil $ （$ \left\lceil\ x\ \right\rceil $ は $ x $ 以上の最小の整数を表す）
- $ 1\ \le\ A_i\ \lt\ 998244353 $
- 入力に含まれる値は全て整数

### Sample Explanation 1

盗み方と盗んだワインの美味しさの和は以下の通りです。 - 左から $ 1 $ 本目のワインと $ 3 $ 本目のワインを盗んだ場合 : 美味しさの和は $ 1\ +\ 2\ =\ 3 $ - 左から $ 1 $ 本目のワインと $ 4 $ 本目のワインを盗んだ場合 : 美味しさの和は $ 1\ +\ 3\ =\ 4 $ - 左から $ 2 $ 本目のワインと $ 4 $ 本目のワインを盗んだ場合 : 美味しさの和は $ 4\ +\ 3\ =\ 7 $ よって答えは $ 3\ +\ 4\ +\ 7\ =\ 14 $ となります。

### Sample Explanation 2

左から $ 1,\ 3,\ 5 $ 本目のワインを盗むほかありません。