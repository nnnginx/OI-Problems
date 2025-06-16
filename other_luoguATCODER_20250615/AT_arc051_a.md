# AT_arc051_a [ARC051A] 塗り絵

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc051/tasks/arc051_a

白く塗られた二次元平面を考えます。

まず、$ (x_1,\ y_1) $ からの距離が $ r $ 以下の部分を赤く塗ります。

そのあと、 $ x_2\ ≦\ x\ ≦\ x_3,\ y_2\ ≦\ y\ ≦\ y_3 $ を満たす $ (x,\ y) $ を青く塗ります。

なお、赤く塗られた後、更に青く塗られた部分は紫色になるとします。

赤く塗られた部分と青く塗られた部分が存在するかどうかをそれぞれ判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ x_1 $ $ y_1 $ $ r $ $ x_2 $ $ y_2 $ $ x_3 $ $ y_3 $

## 输出格式

$ 2 $ 行出力せよ。

$ 1 $ 行目には赤く塗られた部分が存在するならば `YES`、そうでないなら `NO` を出力。

$ 2 $ 行目には青く塗られた部分が存在するならば `YES`、そうでないなら `NO` を出力する。

## 输入输出样例 #1

### 输入 #1

```
-1 -1 2
2 3 4 5
```

### 输出 #1

```
YES
YES
```

## 输入输出样例 #2

### 输入 #2

```
0 1 1
-2 0 4 3
```

### 输出 #2

```
NO
YES
```

## 输入输出样例 #3

### 输入 #3

```
0 0 5
-2 -2 2 1
```

### 输出 #3

```
YES
NO
```

## 输入输出样例 #4

### 输入 #4

```
0 0 2
0 0 4 4
```

### 输出 #4

```
YES
YES
```

## 输入输出样例 #5

### 输入 #5

```
0 0 5
-4 -4 4 4
```

### 输出 #5

```
YES
YES
```

## 说明/提示

### 制約

- $ -100\ ≦\ x_1,\ y_1\ ≦\ 100 $
- $ -100\ ≦\ x_2\ <\ x_3\ ≦\ 100 $
- $ -100\ ≦\ y_2\ <\ y_3\ ≦\ 100 $
- $ 1\ ≦\ r\ ≦\ 100 $
- 与えられる数は全て整数である。

### Sample Explanation 1

!\[A\_img1\](https://arc051.contest.atcoder.jp/img/arc/051/tonarinokyakuhayokukakikuukyakuda/axis1.png) 赤い部分も青い部分もあります

### Sample Explanation 2

!\[A\_img2\](https://arc051.contest.atcoder.jp/img/arc/051/tonarinokyakuhayokukakikuukyakuda/axis2.png) 赤く塗られた部分は存在しません。

### Sample Explanation 3

!\[A\_img3\](https://arc051.contest.atcoder.jp/img/arc/051/tonarinokyakuhayokukakikuukyakuda/axis3.png) 青く塗られた部分は存在しません。

### Sample Explanation 4

!\[A\_img4\](https://arc051.contest.atcoder.jp/img/arc/051/tonarinokyakuhayokukakikuukyakuda/axis4.png) 円と長方形が重なっていますが赤く塗られた部分も青く塗られた部分も存在します。

### Sample Explanation 5

!\[A\_img5\](https://arc051.contest.atcoder.jp/img/arc/051/tonarinokyakuhayokukakikuukyakuda/axis5.png)