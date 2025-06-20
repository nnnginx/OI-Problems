# AT_dwacon6th_final_a 2525敷き詰め

## 题目描述

[problemUrl]: https://atcoder.jp/contests/dwacon6th-final/tasks/dwacon6th_final_a

ニワンゴ君は $ H $ 行 $ W $ 列のマス目を見つけました。 ニワンゴ君は下記の条件を満たすように全てのマスに `2` か `5` を書き込む方法を知りたいです。

- `2` が書かれたマスだけに着目し、**上下左右斜め** に隣接するマス同士に辺を張ったグラフを考えたとき、連結成分のサイズは全て $ 2 $
- `5` が書かれたマスだけに着目し、**上下左右** に隣接するマス同士に辺を張ったグラフを考えたとき、連結成分のサイズは全て $ 5 $

条件を満たすような書き込み方が存在するかどうかを判定し、存在するならばその一例を示してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $

## 输出格式

条件を満たすような書き込み方が存在するならば `Yes` を、しないならば `No` を出力してください。 存在する場合、書き込み方を2行目以降に以下の形式で出力してください。 $ c_{i,j} $ は、 $ i $ 行、 $ j $ 列目のマスに書き込んだ整数です。

> $ c_{11} $ $ \cdots $ $ c_{1W} $ $ \vdots $ $ c_{H1} $ $ \cdots $ $ c_{HW} $

## 输入输出样例 #1

### 输入 #1

```
1 2
```

### 输出 #1

```
Yes
22
```

## 输入输出样例 #2

### 输入 #2

```
1 1
```

### 输出 #2

```
No
```

## 说明/提示

### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ H,W\ \leq\ 2525 $

### Sample Explanation 1

\- `22` が条件を満たす唯一の書き込み方です。 - `55` は連結成分のサイズが全て $ 5 $ という条件に違反することに注意してください。

### Sample Explanation 2

\- 条件を満たす書き込み方が存在しない場合、`No` を出力してください。