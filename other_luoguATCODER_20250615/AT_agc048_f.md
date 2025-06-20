# AT_agc048_f [AGC048F] 01 Record

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc048/tasks/agc048_f

すぬけくんは大きな黒板をもらいました． これに喜んだすぬけくんは，まず，黒板にいくつかの正整数を書きました． 次にすぬけくんは，黒板に書かれている整数がなくなるまで，以下の操作を繰り返し行いました．

- 黒板に書かれている整数を $ 1 $ つ選び，消す． 消した整数を $ x $ とする． 次に，$ x $ を $ 2 $ で割ったあまりをノートに記録する． 最後に，$ x\ \geq\ 2 $ である場合は，新たに $ x-1 $ を黒板に書き加える．

すぬけくんの記録は，`0` と `1` からなる文字列 $ S $ によって表されます． これは，すぬけくんが $ i $ 回目の操作で選んだ整数を $ 2 $ で割ったあまりが $ S_i $ であることを表します．

すぬけくんは，最初に黒板に書いた正整数の組み合わせを忘れてしまいました． 文字列 $ S $ の情報から，最初に黒板に書いた正整数の組み合わせとしてありうるものが何通りあるか求めてください． ここで，正整数の組み合わせ $ a $ と $ b $ が異なるとは，ある整数 $ v $ が存在して，$ a $ に含まれる $ v $ の個数と $ b $ に含まれる $ v $ の個数が異なることを意味します． なお，答えは非常に大きくなることがあるので，$ 10^9+7 $ で割ったあまりを求めてください． また，すぬけくんの記録が間違っており，条件を満たす正整数の組み合わせが存在しないこともありますが，その場合は単に $ 0 $ と答えてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ S $

## 输出格式

最初に黒板に書いた正整数の組み合わせとしてありうるものの数を $ 10^9+7 $ で割ったあまりを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
101
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
100
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
010101
```

### 输出 #3

```
3
```

## 输入输出样例 #4

### 输入 #4

```
11101000111110111101001011110010111110101111110111
```

### 输出 #4

```
3904
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 300 $
- $ S $ は `0` と `1` からなる文字列．

### Sample Explanation 1

最初に黒板に書いた整数の組み合わせとしてあり得るのは，$ \{1,2\},\ \{3\} $ の $ 2 $ つです．

### Sample Explanation 2

最初に黒板に書いた整数の組み合わせとしてあり得るものはありません．

### Sample Explanation 3

最初に黒板に書いた整数の組み合わせとしてあり得るのは，$ \{2,2,2\},\ \{2,4\},\ \{6\} $ の $ 3 $ つです．