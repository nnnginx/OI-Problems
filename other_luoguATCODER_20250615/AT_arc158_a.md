# AT_arc158_a [ARC158A] +3 +5 +7

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc158/tasks/arc158_a

整数 $ x_1,\ x_2,\ x_3 $ が与えられます．あなたはこれらの整数に対して，次の操作を何度でも行うことができます（$ 0 $ 回でもよい）：

- $ (1,2,3) $ の順列 $ (i,j,k) $ をひとつ選ぶ．つまり $ 1\leq\ i,j,k\leq\ 3 $ であるような整数の組 $ (i,j,k) $ であって $ i\neq\ j,\ i\neq\ k,\ j\neq\ k $ となるものを選ぶ．
- その後，$ x_i $ を $ x_i+3 $，$ x_j $ を $ x_j+5 $，$ x_k $ を $ x_k+7 $ で同時に置き換える．
 
あなたの目的は，$ x_1=x_2=x_3 $ が成り立つようにすることです．このことが可能であるか否かを判定してください．可能な場合には，それを達成するための最小の操作回数を出力してください．

$ T $ 個のテストケースが与えられるので，それぞれについて答えを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられます．

> $ T $ $ \text{case}_1 $ $ \vdots $ $ \text{case}_T $

各テストケースは以下の形式で与えられます．

> $ x_1 $ $ x_2 $ $ x_3 $

## 输出格式

$ T $ 行出力してください．$ i $ 行目には $ i $ 番目のテストケースについて，次の値を出力してください．

- $ x_1=x_2=x_3 $ が成り立つようにすることが可能ならば，それを達成するための最小の操作回数．
- $ x_1=x_2=x_3 $ が成り立つようにすることが不可能ならば，$ -1 $．

## 输入输出样例 #1

### 输入 #1

```
4
2 8 8
1 1 1
5 5 10
10 100 1000
```

### 输出 #1

```
2
0
-1
315
```

## 说明/提示

### 制約

- $ 1\leq\ T\leq\ 2\times\ 10^5 $
- $ 1\leq\ x_1,\ x_2,\ x_3\ \leq\ 10^9 $
 
### Sample Explanation 1

ひとつめのテストケースについて，次のように操作を行うことで $ x_1=x_2=x_3 $ が成り立つようにできます． - $ (i,j,k)\ =\ (3,2,1) $ として操作を行う．$ (x_1,x_2,x_3) $ は $ (9,13,11) $ に置き換わる． - $ (i,j,k)\ =\ (2,3,1) $ として操作を行う．$ (x_1,x_2,x_3) $ は $ (16,16,16) $ に置き換わる．