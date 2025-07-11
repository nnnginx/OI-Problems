# AT_abc190_e [ABC190E] Magical Ornament

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc190/tasks/abc190_e

AtCoder 王国には $ 1,\ 2,\ \dots,\ N $ の番号がついた $ N $ 種類の魔法石が流通しています。  
 高橋くんは、魔法石を一列に並べて飾りを作ろうとしています。  
 魔法石には隣り合わせにできる組とできない組があります。 隣り合わせにできる組は $ ( $魔法石 $ A_1, $ 魔法石 $ B_1),\ ( $魔法石 $ A_2, $ 魔法石 $ B_2),\ \dots,\ ( $魔法石 $ A_M, $ 魔法石 $ B_M) $ の $ M $ 組で、それ以外の組は隣り合わせることができません。(これらの組において、石の順序は不問です。)  
 魔法石 $ C_1,\ C_2,\ \dots,\ C_K $ をそれぞれ $ 1 $ 個以上含む魔法石の列を作ることができるか判定し、作れる場合はそのような列を作るのに必要な魔法石の個数の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \hspace{7mm}\vdots $ $ A_M $ $ B_M $ $ K $ $ C_1 $ $ C_2 $ $ \cdots $ $ C_K $

## 输出格式

魔法石 $ C_1,\ C_2,\ \dots,\ C_K $ を含む魔法石の列を作るのに必要な魔法石の個数の最小値を出力せよ。  
 作ることができない場合、代わりに `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
1 4
2 4
3 4
3
1 2 3
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
4 3
1 4
2 4
1 2
3
1 2 3
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
10 10
3 9
3 8
8 10
2 10
5 8
6 8
5 7
6 7
1 6
2 4
4
1 2 7 9
```

### 输出 #3

```
11
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ <\ = N\ <\ =\ 10^5 $
- $ 0\ <\ = M\ <\ =\ 10^5 $
- $ 1\ <\ =\ A_i\ <\ B_i\ <\ =\ N $
- $ i\ ≠\ j $ ならば $ (A_i,\ B_i)\ ≠\ (A_j,\ B_j) $
- $ 1\ <\ =\ K\ <\ =\ 17 $
- $ 1\ <\ =\ C_1\ <\ C_2\ <\ \dots\ <\ C_K\ <\ =\ N $

### Sample Explanation 1

例えば、魔法石を $ [1,\ 4,\ 2,\ 4,\ 3] $ と並べると、魔法石 $ 1,\ 2,\ 3 $ を含む長さ $ 5 $ の列を作ることができます。

### Sample Explanation 3

例えば、魔法石を $ [1,\ 6,\ 7,\ 5,\ 8,\ 3,\ 9,\ 3,\ 8,\ 10,\ 2] $ と並べると、魔法石 $ 1,\ 2,\ 7,\ 9 $ を含む長さ $ 11 $ の列を作ることができます。