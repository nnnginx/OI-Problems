# AT_keyence2019_f Paper Cutting

## 题目描述

[problemUrl]: https://atcoder.jp/contests/keyence2019/tasks/keyence2019_f

縦の長さが $ H+1 $，横の長さが $ W+1 $ の長方形の紙が机に置かれています．$ xy $ 座標系を，紙の四隅の座標がそれぞれ $ (0,\ 0) $, $ (W\ +\ 1,\ 0) $, $ (0,\ H\ +\ 1) $, $ (W\ +\ 1,\ H\ +\ 1) $ となるように定めます．

この紙は，直線 $ x\ =\ 1,2,...,W $ と直線 $ y\ =\ 1,2,...,H $ に沿って切ることができます．これらの $ H\ +\ W $ 本の直線から $ K $ 本を選び，それらの直線に沿って何らかの順序で一回ずつ紙を切断していくという長さ $ K $ の操作列を考えます．

紙の $ 1 $ 回の切断のスコアを，その直後の時点で存在する紙の破片の個数とします．操作列のスコアは，$ K $ 回すべての切断のスコアの和です．

考えられる全ての長さ $ K $ の操作列のスコアの和を計算してください．この値は非常に大きくなることがあるので，$ 10^9\ +\ 7 $ で割った余りを出力してください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ H $ $ W $ $ K $

## 输出格式

スコアの和を $ 10^9\ +\ 7 $ で割った余りを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2 1 2
```

### 输出 #1

```
34
```

## 输入输出样例 #2

### 输入 #2

```
30 40 50
```

### 输出 #2

```
616365902
```

## 说明/提示

### 制約

- $ 1\ \leq\ H,W\ \leq\ 10^7 $
- $ 1\ \leq\ K\ \leq\ H\ +\ W $
- $ H,\ W,\ K $ は整数

### Sample Explanation 1

直線 $ x\ =\ 1 $ に沿った切断を $ x_1 $，直線 $ y\ =\ 1 $ に沿った切断を $ y_1 $，直線 $ y\ =\ 2 $ に沿った切断を $ y_2 $ と表記します．考えられる $ 6 $ 通りの操作列とそれぞれのスコアは次の通りです． - $ y_1,\ y_2 $: $ 2\ +\ 3\ =\ 5 $ - $ y_2,\ y_1 $: $ 2\ +\ 3\ =\ 5 $ - $ y_1,\ x_1 $: $ 2\ +\ 4\ =\ 6 $ - $ y_2,\ x_1 $: $ 2\ +\ 4\ =\ 6 $ - $ x_1,\ y_1 $: $ 2\ +\ 4\ =\ 6 $ - $ x_1,\ y_2 $: $ 2\ +\ 4\ =\ 6 $ これらの和は $ 34 $ です．

### Sample Explanation 2

スコアの和を $ 10^9\ +\ 7 $ で割った余りを出力することを忘れないでください．