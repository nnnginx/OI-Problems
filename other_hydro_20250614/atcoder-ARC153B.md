## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc153/tasks/arc153_b

縦 $ H $ 行，横 $ W $ 列のグリッドがあります．はじめ，上から $ i $ 行目，左から $ j $ 列目のマスには英小文字 $ A_{i,j} $ が書かれています．

このグリッドに対して $ Q $ 回の操作を行います．$ i $ 回目の操作では，$ 1\leq\ a_i\ \leq\ H-1 $, $ 1\leq\ b_i\leq\ W-1 $ を満たす整数 $ a_i,\ b_i $ が与えられ，次を行います．

- グリッド内の長方形領域 $ R_1,\ R_2,\ R_3,\ R_4 $ を次で定める：
  - 上から $ a_i $ 行，左から $ b_i $ 列の部分を $ R_1 $ とする．
  - 上から $ a_i $ 行，右から $ W-b_i $ 列の部分を $ R_2 $ とする．
  - 下から $ H-a_i $ 行，左から $ b_i $ 列の部分を $ R_3 $ とする．
  - 下から $ H-a_i $ 行，右から $ W-b_i $ 列の部分を $ R_4 $ とする．
- $ R_1,\ R_2,\ R_3,\ R_4 $ のそれぞれを $ 180 $ 度回転する．
 
ただし，グリッド内の長方形領域 $ R $ の $ 180 $ 度回転とは，$ R $ において上から $ i $ 番目，左から $ j $ 番目のマスに書かれた文字を，$ R $ において 下から $ i $ 番目，右から $ j $ 番目のマスに移すことをいいます．入出力例の図も参考にしてください．

$ Q $ 回すべての操作を行ったとき，操作後のグリッドの状態を出力してください．

## 输入格式
入力は以下の形式で標準入力から与えられます．

> $ H $ $ W $ $ A_{1,1}\cdots\ A_{1,\ W} $ $ \vdots $ $ A_{H,1}\cdots\ A_{H,\ W} $ $ Q $ $ a_1 $ $ b_1 $ $ \vdots $ $ a_Q $ $ b_Q $

## 输出格式
操作後のマス $ (i,j) $ に書かれている文字を $ B_{i,j} $ とするとき，操作後のグリッドの状態を，次の形式で出力してください．

> $ B_{1,1}\cdots\ B_{1,\ W} $ $ \vdots $ $ B_{H,1}\cdots\ B_{H,\ W} $

## 题目大意
有一个 $H$ 行 $W$ 列的矩阵，矩阵中每个位置都有一个小写字母。每次操作给出 $a,b$，含义是在第 $a,a+1$ 行之间切一刀，再在 $b,b+1$ 列之间切一刀，这样能得到四个矩阵；每个矩阵旋转半周，最后把四个矩阵拼起来得到新矩阵。

有 $n$ 次操作，每次形如 $a_i,b_i$，希望输出操作后的矩阵。

```input1
4 5
abcde
fghij
klmno
pqrst
1
3 3
```

```output1
mlkon
hgfji
cbaed
rqpts
```

```input2
3 7
atcoder
regular
contest
2
1 1
2 5
```

```output2
testcon
oderatc
ularreg
```

```input3
2 2
ac
wa
3
1 1
1 1
1 1
```

```output3
ac
wa
```

## 提示
### 制約

- $ 2\leq\ H,\ W $ かつ $ HW\ \leq\ 5\times\ 10^5 $
- $ A_{i,j} $ は英小文字
- $ 1\leq\ Q\leq\ 2\times\ 10^5 $
- $ 1\leq\ a_i\leq\ H\ -\ 1 $
- $ 1\leq\ b_i\leq\ W\ -\ 1 $
 
### Sample Explanation 1

グリッドの状態は次の図のように変化します． !\[\](https://img.atcoder.jp/arc153/5503f0a5f92e488238556b943aa1d6b7.png)

### Sample Explanation 2

グリッドの状態は次の図のように変化します． !\[\](https://img.atcoder.jp/arc153/353f0b30a9561e38967fb3aedf5767c5.png)

### Sample Explanation 3

グリッドの状態は次の図のように変化します． !\[\](https://img.atcoder.jp/arc153/655a0ac98f0625e806f6abc97853a437.png)

