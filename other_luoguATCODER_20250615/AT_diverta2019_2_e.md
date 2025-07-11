# AT_diverta2019_2_e Balanced Piles

## 题目描述

[problemUrl]: https://atcoder.jp/contests/diverta2019-2/tasks/diverta2019_2_e

$ N $ 個のマスが横一列に並んでおり、左から順に $ 1 $ から $ N $ までの番号がつけられています。高橋君はこれらのマスに積み木を積もうとしています。 まだそれぞれのマスには積み木が $ 1 $ つも積まれていません。

積み木をバランス良く積みたい高橋君は、以下の操作を繰り返して全てのマスに積み木がちょうど $ H $ 個ずつ積まれている状態にしようとしています。

- $ 1 $ マスに積まれている積み木の最大値を $ M $ 個、最小値を $ m $ 個とする。$ m $ 個の積み木が置かれているマスを $ 1 $ つ選び (複数ある場合はどれを選んでもよい)、そのマスに積まれた積み木が $ M $ 個以上 $ M\ +\ D $ 個以下になるように積み木を正の個数積む。

高橋君のために、この操作を繰り返して全てのマスに積み木がちょうど $ H $ 個積まれている状態にする方法が何通りあるか数えてあげてください。答えは非常に大きくなる場合があるので、$ 10^9+7 $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ H $ $ D $

## 输出格式

全てのマスに積み木がちょうど $ H $ 個積まれている状態にする方法の個数を $ 10^9+7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 2 1
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
2 30 15
```

### 输出 #2

```
94182806
```

## 输入输出样例 #3

### 输入 #3

```
31415 9265 3589
```

### 输出 #3

```
312069529
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ 1\ \leq\ D\ \leq\ H\ \leq\ 10^6 $
- 入力は全て整数である

### Sample Explanation 1

(マス $ 1 $ に積まれた積み木の個数, マス $ 2 $ に積まれた積み木の個数) は次のように変化させることができます。 - $ (0,\ 0) $ -&gt; $ (0,\ 1) $ -&gt; $ (1,\ 1) $ -&gt; $ (1,\ 2) $ -&gt; $ (2,\ 2) $ - $ (0,\ 0) $ -&gt; $ (0,\ 1) $ -&gt; $ (1,\ 1) $ -&gt; $ (2,\ 1) $ -&gt; $ (2,\ 2) $ - $ (0,\ 0) $ -&gt; $ (0,\ 1) $ -&gt; $ (2,\ 1) $ -&gt; $ (2,\ 2) $ - $ (0,\ 0) $ -&gt; $ (1,\ 0) $ -&gt; $ (1,\ 1) $ -&gt; $ (1,\ 2) $ -&gt; $ (2,\ 2) $ - $ (0,\ 0) $ -&gt; $ (1,\ 0) $ -&gt; $ (1,\ 1) $ -&gt; $ (2,\ 1) $ -&gt; $ (2,\ 2) $ - $ (0,\ 0) $ -&gt; $ (1,\ 0) $ -&gt; $ (1,\ 2) $ -&gt; $ (2,\ 2) $ よって、全てのマスに積み木がちょうど $ 2 $ 個積まれている状態にする方法の個数は $ 6 $ 通りです。

### Sample Explanation 3

個数を $ 10^9+7 $ で割った余りを出力することに注意してください。