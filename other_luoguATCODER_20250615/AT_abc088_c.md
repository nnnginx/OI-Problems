# AT_abc088_c [ABC088C] Takahashi&#39;s Information

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc088/tasks/abc088_c

$ 3\ \times\ 3 $ のグリッドがあります. 上から $ i $ 番目で左から $ j $ 番目のマスを $ (i,\ j) $ で表すとき, マス $ (i,\ j) $ には数 $ c_{i,\ j} $ が書かれています.  
 高橋君によると, 整数 $ a_1,\ a_2,\ a_3,\ b_1,\ b_2,\ b_3 $ の値が決まっており, マス $ (i,\ j) $ には数 $ a_i\ +\ b_j $ が書かれているらしいです.  
 高橋君の情報が正しいか判定しなさい.

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ c_{1,1} $ $ c_{1,2} $ $ c_{1,3} $ $ c_{2,1} $ $ c_{2,2} $ $ c_{2,3} $ $ c_{3,1} $ $ c_{3,2} $ $ c_{3,3} $

## 输出格式

高橋君の情報が正しい場合 `Yes`, そうでない場合 `No` と出力してください.

## 输入输出样例 #1

### 输入 #1

```
1 0 1
2 1 2
1 0 1
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
2 2 2
2 1 2
2 2 2
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
0 8 8
0 8 8
0 8 8
```

### 输出 #3

```
Yes
```

## 输入输出样例 #4

### 输入 #4

```
1 8 6
2 9 7
0 7 7
```

### 输出 #4

```
No
```

## 说明/提示

### 制約

- $ c_{i,\ j}\ (1\ \leq\ i\ \leq\ 3,\ 1\ \leq\ j\ \leq\ 3) $ は $ 0 $ 以上 $ 100 $ 以下の整数

### Sample Explanation 1

$ a_1=0,a_2=1,a_3=0,b_1=1,b_2=0,b_3=1 $ などの組み合わせがありうるので, 高橋君の情報は正しいです.

### Sample Explanation 2

このグリッドの場合、高橋君の情報は間違っています.