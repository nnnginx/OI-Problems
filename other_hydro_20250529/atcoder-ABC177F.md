## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_f

縦 $ H+1 $ マス横 $ W $ マスのマス目があります。

あなたは一番上のいずれかのマスから始めて右か下に一マス移動することを繰り返します。ただし、$ 1 $ 以上 $ H $ 以下のそれぞれの整数 $ i $ について、グリッドの上から $ i $ マス目の左から $ A_i $ マス目、$ A_i\ +\ 1 $ マス目、$ \ldots $、$ B_i $ マス目のマスからは下に移動することができません。

$ 1 $ 以上 $ H $ 以下のそれぞれの整数 $ k $ について、上から $ k+1 $ マス目のいずれかのマス目まで移動するための最小の移動回数を求めてください。(出発するマスは各場合について個別に選ぶことができます。) 一番上のどのマスから始めても上から $ k+1 $ マス目のいずれのマス目にも移動できない場合、代わりに `-1` を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ : $ $ A_H $ $ B_H $

## 输出格式
$ H $ 行出力せよ。$ i $ 行目には、$ k=i $ のときの答えを出力せよ。

## 题目大意
### 题目大意

有一个 $(H+1)$ 行 $W$ 列的矩阵，你每步可以在矩阵中向右或向下移动一个格子。其中，在第 $i\,(1 \le i \le H)$ 行中，你无法从左至右第 $A_i$ 至 $B_i$ 个格子向下走。对于每一个 $k\,(1 \le k \le H)$，求出你从第 $1$ 行的任意一个格子出发移动到第 $(k+1)$ 行的最少步数，若无法移动到则输出 `-1`。

数据范围：$1 \le H,W \le 2\times 10^5$，$1 \le A_i \le B_i \le W$。

### 输入格式

第一行两个整数 $H,W$，接下来 $H$ 行每行两个整数 $A_i,B_i$。

### 输出格式

共 $H$ 行，每行一个整数，第 $i$ 行的数字表示从第 $1$ 行移动到第 $(i+1)$ 行需要的最少步数，若无法移动到则为 `-1`。

### 样例解释

$k=1$ 时，其中一种答案最小的移动顺序为 $(1,1)\rightarrow (2,1)$；

$k=2$ 时，一种移动顺序为 $(1,1)\rightarrow (2,1)\rightarrow (2,2)\rightarrow (3,2)$；

$k=3$ 时，一种移动顺序为 $(1,1)\rightarrow (2,1)\rightarrow (2,2)\rightarrow (3,2)\rightarrow (3,3)\rightarrow (3,4)\rightarrow (4,4)$；

$k=4$ 时，无法从第 $1$ 行移动到第 $5$ 行。

（翻译 by @CarroT1212）

```input1
4 4
2 4
1 1
2 3
2 4
```

```output1
1
3
6
-1
```

## 提示
### 制約

- $ 1\ \leq\ H,W\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ B_i\ \leq\ W $

### Sample Explanation 1

上から $ i $ マス目、左から $ j $ マス目のマスをマス $ (i,j) $ とします。 $ k=1 $ のとき、マス $ (1,1) $ → $ (2,1) $ のように $ 1 $ 回で移動できます。 $ k=2 $ のとき、マス $ (1,1) $ → $ (2,1) $ → $ (2,2) $ → $ (3,2) $ のように $ 3 $ 回で移動できます。 $ k=3 $ のとき、マス $ (1,1) $ → $ (2,1) $ → $ (2,2) $ → $ (3,2) $ → $ (3,3) $ → $ (3,4) $ → $ (4,4) $ のように $ 6 $ 回で移動できます。 $ k=4 $ のとき、上から $ 5 $ マス目のマスに移動する方法はありません。

