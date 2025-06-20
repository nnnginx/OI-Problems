# AT_abc345_e [ABC345E] Colorful Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc345/tasks/abc345_e

$ N $ 個のボールが左右一列に並んでいます。  
左から $ i $ $ (1\leq\ i\leq\ N) $ 番目のボールは色 $ C_i $ で、価値は $ V_i $ です。

高橋君はこの列から **ちょうど** $ K $ 個のボールを取り除いたうえで、 残ったボールを元の順番で並べたときに同じ色のボールが隣り合わないようにしたいと考えています。 また、その条件のもとで、列に残ったボールの価値の総和をなるべく大きくしたいと考えています。

高橋君が、残ったボールの列において同じ色のボールが隣り合わないように $ K $ 個のボールを取り除くことができるか判定し、 できる場合は列に残ったボールの価値の総和としてあり得る最大の値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ C_1 $ $ V_1 $ $ C_2 $ $ V_2 $ $ \vdots $ $ C_N $ $ V_N $

## 输出格式

高橋君が同じ色のボールが隣り合わないように$ K $ 個のボールを取り除くことができる場合は、 列に残ったボールの価値の総和としてあり得る最大値を整数で出力せよ。 できない場合は、$ -1 $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 2
1 1
3 5
3 3
1 4
1 2
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
3 1
1 10
1 10
1 10
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
3 1
1 1
2 2
3 3
```

### 输出 #3

```
5
```

## 说明/提示

### 制約

- $ 1\leq\ K\ <\ N\leq\ 2\times\ 10^5 $
- $ K\leq\ 500 $
- $ 1\leq\ C_i\leq\ N $
- $ 1\leq\ V_i\leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

左から、$ 3,5 $ 番目のボールを取り除くと、残ったボールは左から順に色 $ 1,3,1 $ であるため、 どの隣り合う $ 2 $ つのボールの色も異なり、条件をみたしています。 このとき、列に残ったボールの価値の和は $ V_1+V_2+V_4=1+5+4=10 $ です。 他にも $ 5 $ つのボールから $ 2 $ つのボールを取り除く方法であって、同じ色のボールが隣り合わないようにできるものは存在しますが、 $ 3,5 $ 番目のボールを取り除いた時に残ったボールの価値の和は最大となります。 よって、$ 10 $ を出力します。

### Sample Explanation 2

どのようにボールを $ 1 $ つ取り除いても色 $ 1 $ のボールが隣り合ってしまいます。 よって、 $ -1 $ を出力します。

### Sample Explanation 3

必ずちょうど $ K $ 個のボールを取り除く必要があることに注意してください。