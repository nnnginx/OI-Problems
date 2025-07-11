# AT_abc293_d [ABC293D] Tying Rope

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc293/tasks/abc293_d

一方の端が赤に塗られており、もう一方の端が青に塗られているロープが $ N $ 本あります。ロープには $ 1 $ から $ N $ までの番号がつけられています。

これからロープの端を結ぶ操作を $ M $ 回行います。$ i $ 回目の操作ではロープ $ A_i $ の色 $ B_i $ の端とロープ $ C_i $ の色 $ D_i $ の端を結びます。ただし、色 `R` は赤を意味し、色 `B` は青を意味します。各ロープについて、同じ色の端が複数回結ばれることはありません。

すべての操作を終えた後に、ひとつながりになっているロープの組について環状になっているものとそうでないものの個数を出力してください。

ただし、ひとつながりになっているロープの組 $ \lbrace\ v_0,\ v_1,\ \ldots,\ v_{x-1}\ \rbrace $ が環状になっているとは、$ v $ の要素の順序を適切に入れ替えることで各 $ 0\ \leq\ i\ <\ x $ についてロープ $ v_i $ とロープ $ v_{(i+1)\ \bmod\ x} $ が結ばれているようにできることをいいます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ C_1 $ $ D_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ D_2 $ $ \vdots $ $ A_M $ $ B_M $ $ C_M $ $ D_M $

## 输出格式

ひとつながりになっているロープの組について、環状になっているものの個数を $ X $、そうでないものの個数を $ Y $ として $ X $ と $ Y $ をこの順に空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 3
3 R 5 B
5 R 3 B
4 R 2 B
```

### 输出 #1

```
1 2
```

## 输入输出样例 #2

### 输入 #2

```
7 0
```

### 输出 #2

```
0 7
```

## 输入输出样例 #3

### 输入 #3

```
7 6
5 R 3 R
7 R 4 R
4 B 1 R
2 R 3 B
2 B 5 B
1 B 7 B
```

### 输出 #3

```
2 1
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i,\ C_i\ \leq\ N $
- $ (A_i,\ B_i)\ \neq\ (A_j,\ B_j),\ (C_i,\ D_i)\ \neq\ (C_j,\ D_j) $ $ (i\ \neq\ j) $
- $ (A_i,\ B_i)\ \neq\ (C_j,\ D_j) $
- $ N,\ M,\ A_i,\ C_i $ は整数
- $ B_i,\ D_i $ は `R` か `B` のいずれか
 
### Sample Explanation 1

ひとつながりになっているロープの組は $ \lbrace\ 1\ \rbrace $、$ \lbrace\ 2,4\ \rbrace $、$ \lbrace\ 3,5\ \rbrace $ の $ 3 $ つです。 ロープ $ \lbrace\ 3,5\ \rbrace $ の組は環状になっており、ロープ $ \lbrace\ 1\ \rbrace $ と $ \lbrace\ 2,4\ \rbrace $ の組は環状になっていません。したがって、$ X\ =\ 1,\ Y\ =\ 2 $ です。