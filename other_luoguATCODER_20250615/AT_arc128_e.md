# AT_arc128_e [ARC128E] K Different Values

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc128/tasks/arc128_e

長さ $ N $ の整数列 $ A=(A_1,A_2,\cdots,A_N) $，及び整数 $ K $ が与えられます．

以下の条件を両方満たす整数列 $ x $ を作ることを考えます．

- 各整数 $ i $ ($ 1\ \leq\ i\ \leq\ N $) について，$ x $ はちょうど $ A_i $ 個の $ i $ を含む． また逆に，それ以外の整数を含まない．
- $ x $ の中で連続するどの $ K $ 個を見ても，その $ K $ 個の値はすべて異なる．

条件を満たす $ x $ を作ることが可能かどうか判定し，可能な場合は条件を満たす中で辞書順最小の $ x $ を求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

条件を満たす数列 $ x $ が作ることが不可能な場合，`-1` と出力せよ． 可能な場合，辞書順最小の $ x $ を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3 3
2 2 1
```

### 输出 #1

```
1 2 3 1 2
```

## 输入输出样例 #2

### 输入 #2

```
3 2
2 1 2
```

### 输出 #2

```
1 2 3 1 3
```

## 输入输出样例 #3

### 输入 #3

```
3 3
1 3 3
```

### 输出 #3

```
-1
```

## 说明/提示

### 制約

- $ 2\ \leq\ K\ \leq\ N\ \leq\ 500 $
- $ 1\ \leq\ A_i $
- $ \sum_{1\ \leq\ i\ \leq\ N}\ A_i\ \leq\ 200000 $
- 入力される値はすべて整数である

### Sample Explanation 1

$ x=(1,2,3,1,2),(2,1,3,2,1) $ の二つが条件を満たし，その中で辞書順最小の $ (1,2,3,1,2) $ が答えになります．