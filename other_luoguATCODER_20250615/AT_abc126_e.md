# AT_abc126_e [ABC126E] 1 or 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc126/tasks/abc126_e

$ N $ 枚のカードが一列に伏せられており、各カードには整数 $ 1 $ または $ 2 $ が書かれています。

$ i $ 番目のカードに書かれている整数を $ A_i $ とします。

あなたの目的は $ A_1,\ A_2,\ ...,\ A_N $ を当てることです。

次のことが分かっています。

- $ i\ =\ 1,\ 2,\ ...,\ M $ について $ A_{X_i}\ +\ A_{Y_i}\ +\ Z_i $ は偶数である。

あなたは魔法使いです。次の魔法を何度でも使うことができます。

**魔法**: コストを $ 1 $ 払う。カードを $ 1 $ 枚選び、そのカードに書かれた整数 $ A_i $ を知る。

最小で何コスト払えば、$ A_1,\ A_2,\ ...,\ A_N $ 全てを確実に当てることができるでしょうか。

なお、与えられる入力には矛盾がないことが保証されます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X_1 $ $ Y_1 $ $ Z_1 $ $ X_2 $ $ Y_2 $ $ Z_2 $ $ \vdots $ $ X_M $ $ Y_M $ $ Z_M $

## 输出格式

$ A_1,\ A_2,\ ...,\ A_N $ 全てを確実に当てるために払う必要のあるコストの合計の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 1
1 2 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6 5
1 2 1
2 3 2
1 3 3
4 5 4
5 6 5
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
100000 1
1 100000 100
```

### 输出 #3

```
99999
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ X_i\ <\ Y_i\ \leq\ N $
- $ 1\ \leq\ Z_i\ \leq\ 100 $
- $ (X_i,\ Y_i) $ の組は互いに異なる。
- 与えられる入力には矛盾がない(すなわち、条件を満たす $ A_1,\ A_2,\ ...,\ A_N $ が存在する)。

### Sample Explanation 1

$ 1 $ 枚目と $ 3 $ 枚目のカードに対してそれぞれ $ 1 $ 回ずつ魔法を使えば、$ A_1,\ A_2,\ A_3 $ 全てを当てることができます。