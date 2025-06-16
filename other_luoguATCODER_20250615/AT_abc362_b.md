# AT_abc362_b [ABC362B] Right Triangle

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc362/tasks/abc362_b

$ xy $ 平面上に、同一直線上にない $ 3 $ 点 $ A(x_A,y_A),\ B(x_B,y_B),C(x_C,y_C) $ があります。三角形 $ ABC $ が直角三角形であるかどうか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ x_A $ $ y_A $ $ x_B $ $ y_B $ $ x_C $ $ y_C $

## 输出格式

三角形 $ ABC $ が直角三角形であるならば `Yes` を、そうでないならば `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
0 0
4 0
0 3
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
-4 3
2 1
3 4
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
2 4
-3 2
1 -2
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ -1000\leq\ x_A,y_A,x_B,y_B,x_C,y_C\leq\ 1000 $
- $ 3 $ 点 $ A,B,C $ は同一直線上にない
- 入力は全て整数
 
### Sample Explanation 1

三角形 $ ABC $ は直角三角形です。 !\[\](https://img.atcoder.jp/abc362/3f4a68afd7a43d159b7e7ef4cee6c646.png)

### Sample Explanation 2

三角形 $ ABC $ は直角三角形です。 !\[\](https://img.atcoder.jp/abc362/092af99ccc22b9235a87bc2b5f53bfa3.png)

### Sample Explanation 3

三角形 $ ABC $ は直角三角形ではありません。 !\[\](https://img.atcoder.jp/abc362/f7fbb440279967aee94ef846562d4b0e.png)