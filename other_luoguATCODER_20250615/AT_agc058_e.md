# AT_agc058_e [AGC058E] Nearer Permutation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc058/tasks/agc058_e

この問題では，順列と言った際には，$ (1,2,\cdots,N) $ の順列を指すものとします．

$ 2 $ つの順列 $ p,q $ に対し，それらの距離 $ d(p,q) $ を次のように定義します．

- $ p $ の中で隣接 $ 2 $ 項を swap することを繰り返し，$ p $ を $ q $ に一致させることを考える．この時必要な最小の操作回数を $ d(p,q) $ とする．

さらに，順列 $ x $ に対し，順列 $ f(x) $ を次のように定義します．

- $ y=(1,2,\cdots,N) $ とする．ここで，順列 $ z $ であって，$ d(x,z)\ \leq\ d(y,z) $ を満たすものを考える． これらの中で辞書順最小のものを $ f(x) $ とする．

例えば，$ x=(2,3,1) $ の場合，$ d(x,z)\ \leq\ d(y,z) $ を満たす順列としては，$ z=(2,1,3),(2,3,1),(3,1,2),(3,2,1) $ が考えられます． このうち辞書順最小なのは $ (2,1,3) $ なので， $ f(x)=(2,1,3) $ となります．

順列 $ A=(A_1,A_2,\cdots,A_N) $ が与えられます． $ f(x)=A $ を満たす順列 $ x $ が存在するかどうか判定してください．

$ 1 $ つの入力ファイルにつき，$ T $ 個のテストケースを解いてください．

 数列の辞書順とは？ 相異なる数列 $ S $ と数列 $ T $ の大小を判定するアルゴリズムを以下に説明します。

以下では $ S $ の $ i $ 番目の要素を $ S_i $ のように表します。また、 $ S $ が $ T $ より辞書順で小さい場合は $ S\ \lt\ T $ 、大きい場合は $ S\ \gt\ T $ と表します。

1. $ S $ と $ T $ のうち長さが短い方の文字列の長さを $ L $ とします。$ i=1,2,\dots,L $ に対して $ S_i $ と $ T_i $ が一致するか調べます。
2. $ S_i\ \neq\ T_i $ である $ i $ が存在する場合、そのような $ i $ のうち最小のものを $ j $ とします。そして、$ S_j $ と $ T_j $ を比較して、 $ S_j $ が $ T_j $ より（数として）小さい場合は $ S\ \lt\ T $ 、大きい場合は $ S\ \gt\ T $ と決定して、アルゴリズムを終了します。
3. $ S_i\ \neq\ T_i $ である $ i $ が存在しない場合、 $ S $ と $ T $ の長さを比較して、$ S $ が $ T $ より短い場合は $ S\ \lt\ T $ 、長い場合は $ S\ \gt\ T $ と決定して、アルゴリズムを終了します。

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ T $ $ case_1 $ $ case_2 $ $ \vdots $ $ case_T $

各ケースは以下の形式で与えられる．

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

各ケースに対し，$ f(x)=A $ を満たす順列 $ x $ が存在するならば `Yes` を，存在しないならば `No` を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
2
1 2
2
2 1
```

### 输出 #1

```
Yes
Yes
```

## 输入输出样例 #2

### 输入 #2

```
6
3
1 2 3
3
1 3 2
3
2 1 3
3
2 3 1
3
3 1 2
3
3 2 1
```

### 输出 #2

```
Yes
Yes
Yes
Yes
No
No
```

## 输入输出样例 #3

### 输入 #3

```
24
4
1 2 3 4
4
1 2 4 3
4
1 3 2 4
4
1 3 4 2
4
1 4 2 3
4
1 4 3 2
4
2 1 3 4
4
2 1 4 3
4
2 3 1 4
4
2 3 4 1
4
2 4 1 3
4
2 4 3 1
4
3 1 2 4
4
3 1 4 2
4
3 2 1 4
4
3 2 4 1
4
3 4 1 2
4
3 4 2 1
4
4 1 2 3
4
4 1 3 2
4
4 2 1 3
4
4 2 3 1
4
4 3 1 2
4
4 3 2 1
```

### 输出 #3

```
Yes
Yes
Yes
Yes
Yes
Yes
Yes
Yes
Yes
Yes
No
No
No
No
No
No
No
No
No
No
No
No
No
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ T\ \leq\ 150000 $
- $ 2\ \leq\ N\ \leq\ 300000 $
- $ (A_1,A_2,\cdots,A_N) $ は $ (1,2,\cdots,N) $ の順列
- $ 1 $ つの入力ファイルにつき，$ N $ の総和は $ 300000 $ を超えない
- 入力される値はすべて整数である

### Sample Explanation 1

例えば $ A=(2,1) $ の場合は，$ x=(2,1) $ とすると $ f(x)=A $ となります．

### Sample Explanation 2

例えば $ A=(2,3,1) $ の場合は，$ x=(3,2,1) $ とすると，$ f(x)=A $ となります．