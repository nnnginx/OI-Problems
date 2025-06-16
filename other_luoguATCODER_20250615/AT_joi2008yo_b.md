# AT_joi2008yo_b JOIとIOI

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2008yo/tasks/joi2008yo_b

与えられた文字列内の連続する $ 3 $ 文字が，`JOI` または `IOI` という並びになっている個所がそれぞれ何個所あるのかを数え上げるプログラムを作成せよ．文字列はアルファベットの大文字だけからなる．例えば下図の「`JOIOIOI`」という文字列には `JOI` が $ 1 $ 個所，`IOI` が $ 2 $ 個所に含まれている．

![2008-yo-t2-sample.png](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_joi2008yo_b/b4202de9541777caaf09e0fb98aba7dc6657072a.png)

- - - - - -

## 输入格式

入力は $ 1 $ 行であり，$ 10\,000 $ 文字以下のアルファベットの大文字からなる．

## 输出格式

出力は $ 2 $ 行からなる．$ 1 $ 行目に見つかった `JOI` の個数，$ 2 $ 行目に見つかった `IOI` の個数をそれぞれ出力せよ．

- - - - - -

## 输入输出样例 #1

### 输入 #1

```
JOIJOI
```

### 输出 #1

```
2
0
```

## 输入输出样例 #2

### 输入 #2

```
JOIOIOIOI
```

### 输出 #2

```
1
3
```

## 输入输出样例 #3

### 输入 #3

```
JOIOIJOINXNXJIOIOIOJ
```

### 输出 #3

```
2
3
```

## 说明/提示

### Sample Explanation 1

\- - - - - -

### Sample Explanation 2

\- - - - - -