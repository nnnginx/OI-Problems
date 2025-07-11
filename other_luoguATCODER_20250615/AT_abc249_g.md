# AT_abc249_g [ABC249G] Xor Cards

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc249/tasks/abc249_g

$ N $ 枚のカードがあり、$ 1,\ \dots,\ N $ の番号が付けられています。カード $ i\ \,\ (1\ \leq\ i\ \leq\ N) $ の表には整数 $ A_i $、裏には整数 $ B_i $ が書かれています。

選んだカードの表に書かれた整数の排他的論理和が $ K $ 以下となるように $ 1 $ 枚以上の好きな枚数のカードを選ぶとき、選んだカードの裏に書かれた整数の排他的論理和としてあり得る最大値を求めてください。

 排他的論理和とは 整数 $ a,\ b $ の排他的論理和 $ a\ \oplus\ b $ は、以下のように定義されます。 - $ a\ \oplus\ b $ を二進表記した際の $ 2^k\ \,\ (k\ \geq\ 0) $ の位の数は、$ a,\ b $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。

 例えば、$ 3\ \oplus\ 5\ =\ 6 $ となります（二進表記すると $ 011\ \oplus\ 101\ =\ 110 $）。  
 一般に $ k $ 個の整数 $ p_1,\ \dots,\ p_k $ の排他的論理和は $ (\cdots\ ((p_1\ \oplus\ p_2)\ \oplus\ p_3)\ \oplus\ \cdots\ \oplus\ p_k) $ と定義され、これは $ p_1,\ \dots,\ p_k $ の順番によらないことが証明できます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_N $ $ B_N $

## 输出格式

問題文中の条件を満たすようにカードを選ぶとき、選んだカードの裏に書かれた整数の排他的論理和としてあり得る最大値を出力せよ。ただし、条件を満たすようにカードを選ぶことができないときは $ -1 $ と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 2
1 1
3 2
2 2
0 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
1 2
3 4
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
10 326872757
487274679 568989827
267359104 968688210
669234369 189421955
1044049637 253386228
202278801 233212012
436646715 769734012
478066962 376960084
491389944 1033137442
214977048 1051768288
803550682 1053605300
```

### 输出 #3

```
1064164329
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 0\ \leq\ K\ \lt\ 2^{30} $
- $ 0\ \leq\ A_i,\ B_i\ \lt\ 2^{30}\ \,\ (1\ \leq\ i\ \leq\ N) $
- 入力は全て整数

### Sample Explanation 1

カード $ 1,\ 2 $ を選ぶことで、表に書かれた整数の排他的論理和は $ 2 $、裏に書かれた整数の排他的論理和は $ 3 $ となり、これが最大です。

### Sample Explanation 2

条件を満たすようにカードを選ぶことはできません。