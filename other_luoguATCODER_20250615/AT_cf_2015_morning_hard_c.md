# AT_cf_2015_morning_hard_c 数列の組み替え

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-morning-hard/tasks/cf_2015_morning_hard_c

りんごさんは長さ $ N $ の数列を持っています。数列は相異なる $ 1 $ ~ $ N $ の整数からなります。りんごさんはこの数列を $ K $ 箇所で切って $ K+1 $ 個の連続した部分に分割し、それらを好きな順番で連結することにより新たな数列を作ろうとしています。りんごさんが作ることのできる数列のうち辞書順最小のものを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ ... $ A_N $

- $ 1 $ 行目には、$ 2 $ つの整数 $ N\ (2\ ≦\ N\ ≦\ 10^5),\ K\ (1\ ≦\ K\ ≦\ N-1) $ が空白区切りで与えられる。これは、数列の長さが $ N $、数列を切る場所が $ K $ 箇所であることを表す。
- $ 2 $ 行目には、$ N $ 個の整数が空白区切りで与えられる。このうち $ i\ (1\ ≦\ i\ ≦\ N) $ 番目の整数 $ A_i\ (1\ ≦\ A_i\ ≦\ N) $ は、数列の $ i $ 番目の数を表す。ただし、$ A_i $ は全て相異なることが保証される。

## 输出格式

出力は $ N $ 行からなる。このうち $ i $ 行目には、りんごさんが作ることのできる数列のうち辞書順最小の数列の $ i $ 番目の数を表す $ 1 $ つの整数を出力せよ。出力の末尾にも改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
5 3
1 3 5 2 4
```

### 输出 #1

```
1
2
3
5
4
```

## 输入输出样例 #2

### 输入 #2

```
9 5
4 6 8 1 2 9 3 7 5
```

### 输出 #2

```
1
2
3
4
6
7
5
8
9
```

## 说明/提示

### Sample Explanation 1

$ 1\ |\ 3\ 5\ |\ 2\ |\ 4 $ と切って $ 1\ |\ 2\ |\ 3\ 5\ |\ 4 $ と並べ替えると辞書順最小の数列になります。