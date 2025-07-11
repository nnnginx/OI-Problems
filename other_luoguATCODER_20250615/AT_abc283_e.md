# AT_abc283_e [ABC283E] Don‘t Isolate Elements

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc283/tasks/abc283_e

各要素の値が $ 0 $ または $ 1 $ である $ H $ 行 $ W $ 列の行列 $ A $ が与えられます。 $ 1\ \leq\ i\ \leq\ H $ かつ $ 1\ \leq\ j\ \leq\ W $ を満たす整数の組 $ (i,j) $ について、$ A $ の $ i $ 行目 $ j $ 列目の要素を $ A_{i,j} $ で表します。

行列 $ A $ に対し、以下の操作を $ 0 $ 回以上の好きな回数行うことができます。

- $ 1\ \leq\ i\ \leq\ H $ を満たす整数 $ i $ を選び、$ 1\ \leq\ j\ \leq\ W $ を満たす全ての整数 $ j $ に対して $ A_{i,j} $ の値を $ 1-A_{i,j} $ で置き換える。
 
また、$ A_{i,j} $ は行列において上下左右に同じ値が存在しない、すなわち $ 4 $ つの整数組 $ (x,y)\ =\ (i-1,j),(i+1,j),(i,j-1),(i,j+1) $ のいずれかであって、 $ 1\ \leq\ x\ \leq\ H,\ 1\ \leq\ y\ \leq\ W $ かつ $ A_{i,j}\ =\ A_{x,y} $ を満たすものが存在しないとき、またそのときに限り**孤立した要素**であると定義されます。

操作を繰り返し行列 $ A $ の任意の要素が孤立した要素でない状態にすることが可能か判定し、可能な場合は行う操作回数の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ A_{1,1} $ $ A_{1,2} $ $ \ldots $ $ A_{1,W} $ $ A_{2,1} $ $ A_{2,2} $ $ \ldots $ $ A_{2,W} $ $ \vdots $ $ A_{H,1} $ $ A_{H,2} $ $ \ldots $ $ A_{H,W} $

## 输出格式

操作を繰り返すことにより孤立した要素が存在しないようにできる場合は操作回数の最小値を、できない場合は `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 1 0
1 0 1
1 0 0
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
4 4
1 0 0 0
0 1 1 1
0 0 1 0
1 1 0 1
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
2 3
0 1 0
0 1 1
```

### 输出 #3

```
-1
```

## 说明/提示

### 制約

- $ 2\ \leq\ H,W\ \leq\ 1000 $
- $ A_{i,j}\ =\ 0 $ または $ A_{i,j}\ =\ 1 $
- 入力はすべて整数
 
### Sample Explanation 1

$ i\ =\ 1 $ を選択し操作を行うと、$ A\ =\ ((0,0,1),(1,0,1),(1,0,0)) $ となり、孤立した要素は存在しなくなります。