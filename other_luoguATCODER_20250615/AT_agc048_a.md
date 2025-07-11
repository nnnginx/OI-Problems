# AT_agc048_a [AGC048A] atcoder < S

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc048/tasks/agc048_a

英小文字からなる文字列 $ S $ が与えられます． すぬけくんは，$ S $ の**隣り合う** $ 2 $ 文字をスワップするという操作を行うことができます． 例えば，$ S= $`agc` なら，$ 1 $ 回の操作で，$ S $ を `gac` (`a` と `g` をスワップ) もしくは `acg` (`g` と `c` をスワップ) に変換できます．

すぬけくんはこの操作を $ 0 $ 回以上繰り返し， 辞書順で `atcoder` $ <\ S $ となるようにしたいです．

 辞書順で $ x&amp;lt\ y $ の定義 文字列 $ x,y $ が辞書順で $ x&amp;lt\ y $ であるとは，以下のうちいずれかの条件を満たすことを意味します．

- ある整数 $ i $ ($ 1\ \leq\ i\ \leq\ \mathrm{min}(|x|,|y|) $) が存在して，$ x,y $ は先頭の $ i-1 $ 文字が一致しており，かつ， $ x $ の $ i $ 文字目は $ y $ の $ i $ 文字目よりアルファベット順で真に小さい．
- $ |x|&amp;lt\ |y| $ であり，$ y $ の先頭の $ |x| $ 文字は $ x $ と等しい．

目標が達成可能かどうか判定し，可能な場合は必要な操作回数の最小値を求めてください．

$ 1 $ つの入力ファイルにつき，$ T $ 個のテストケースを解いてください．

## 输入格式

入力は以下の形式で標準入力から与えられる． 入力の $ 1 $ 行目は以下のとおりである．

> $ T $

そして，$ T $ 個のテストケースが続く． これらはそれぞれ以下の形式で与えられる．

> $ S $

## 输出格式

各テストケースについて，目標が達成不可能な場合は $ -1 $，可能な場合は必要な操作回数の最小値を出力せよ． 各テストケースごとに改行せよ．

## 输入输出样例 #1

### 输入 #1

```
3
atcodeer
codeforces
aaa
```

### 输出 #1

```
1
0
-1
```

## 说明/提示

### 制約

- $ 1\ \leq\ T\ \leq\ 100 $
- $ 1\ \leq\ |S|\ \leq\ 1000 $
- $ S $ は英小文字からなる文字列．

### Sample Explanation 1

\- $ 1 $ 番目のテストケース: 例えば，末尾の $ 2 $ 文字をスワップすることで，$ S= $`atcodere` $ > $ `atcoder` となります． - $ 2 $ 番目のテストケース: 操作を行うまでもなく，$ S= $`codeforces` $ > $ `atcoder` です． - $ 3 $ 番目のテストケース: どのように操作を行っても $ S\ > $ `atcoder` にはなりません．