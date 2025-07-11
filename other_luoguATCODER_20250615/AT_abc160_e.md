# AT_abc160_e [ABC160E] Red and Green Apples

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc160/tasks/abc160_e

あなたは、$ X $ 個の赤色のリンゴと $ Y $ 個の緑色のリンゴを食べようとしています。  
 あなたは $ A $ 個の赤色のリンゴを持っており、美味しさはそれぞれ $ p_1,p_2,\ \dots\ ,p_A $ です。  
 あなたは $ B $ 個の緑色のリンゴを持っており、美味しさはそれぞれ $ q_1,q_2,\ \dots\ ,q_B $ です。  
 あなたは $ C $ 個の無色のリンゴを持っており、美味しさはそれぞれ $ r_1,r_2,\ \dots\ ,r_C $ です。  
 無色のリンゴは食べる前に着色することで、赤色のリンゴもしくは緑色のリンゴと見なすことができます。  
 以上のリンゴの中から、できるだけ美味しさの総和が大きくなるように食べるリンゴを選びます。  
 $ 0 $ 個以上の無色のリンゴに適切に着色したとき、食べる $ X+Y $ 個のリンゴの美味しさの総和が最大でいくつになるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ X $ $ Y $ $ A $ $ B $ $ C $ $ p_1 $ $ p_2 $ $ ... $ $ p_A $ $ q_1 $ $ q_2 $ $ ... $ $ q_B $ $ r_1 $ $ r_2 $ $ ... $ $ r_C $

## 输出格式

リンゴの美味しさの総和の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 2 2 2 1
2 4
5 1
3
```

### 输出 #1

```
12
```

## 输入输出样例 #2

### 输入 #2

```
2 2 2 2 2
8 6
9 1
2 1
```

### 输出 #2

```
25
```

## 输入输出样例 #3

### 输入 #3

```
2 2 4 4 4
11 12 13 14
21 22 23 24
1 2 3 4
```

### 输出 #3

```
74
```

## 说明/提示

### 制約

- $ 1\ \leq\ X\ \leq\ A\ \leq\ 10^5 $
- $ 1\ \leq\ Y\ \leq\ B\ \leq\ 10^5 $
- $ 1\ \leq\ C\ \leq\ 10^5 $
- $ 1\ \leq\ p_i\ \leq\ 10^9 $
- $ 1\ \leq\ q_i\ \leq\ 10^9 $
- $ 1\ \leq\ r_i\ \leq\ 10^9 $
- 入力はすべて整数である。

### Sample Explanation 1

以下のようにすることで、食べるリンゴの美味しさの総和を最大にすることができます。 - $ 2 $ 番目の赤色のリンゴを食べる。 - $ 1 $ 番目の緑色のリンゴを食べる。 - $ 1 $ 番目の無色のリンゴを緑色に着色し、食べる。