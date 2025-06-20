# AT_abc030_c [ABC030C] 飛行機乗り

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc030/tasks/abc030_c

ウナギの高橋くんは飛行機に乗ることが趣味です。今回は空港Aと空港Bを往復することにしました。

空港Aから空港Bの飛行機には $ X $ 時間かかり、空港Bから空港Aへの飛行機には $ Y $ 時間かかります。 空港Aから空港Bへの飛行機は $ N $ 本あり、$ i $ 番目の便は $ a_i $ 時に出発します。 空港Bから空港Aへの飛行機は $ M $ 本あり、$ j $ 番目の便は $ b_j $ 時に出発します。

ある飛行機には、出発する空港に出発する時刻以前にいれば乗ることができます。出発する時刻ちょうどに到着した場合も、すぐに飛行機に乗って出発できます。 高橋くんははじめ空港Aに $ 0 $ 時にいます。 空港Aと空港Bの間を最大何往復できるか調べてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X $ $ Y $ $ a_1 $ $ a_2 $ .. $ a_N $ $ b_1 $ $ b_2 $ .. $ b_M $

- $ 1 $ 行目には、空港Aから空港Bへの本数 $ N\ (\ 1\ ≦\ N\ ≦\ 10^5) $、空港Bから空港Aへの本数 $ M\ (\ 1\ ≦\ M\ ≦\ 10^5) $ が空白区切りで与えられる。
- $ 2 $ 行目には、空港Aから空港Bへの飛行機にかかる時間 $ X\ (\ 1\ ≦\ X\ ≦\ 10^9) $、空港Bから空港Aへの飛行機にかかる時間 $ Y\ (\ 1\ ≦\ Y\ ≦\ 10^9) $ が空白区切りで与えられる。
- $ 3 $ 行目には、$ N $ 個の空港Aから飛行機が出発する時刻を表す整数 $ a_i $ が空白を区切りとして与えられる。
- $ 4 $ 行目には、$ M $ 個の空港Bから飛行機が出発する時刻を表す整数 $ b_j $ が空白を区切りとして与えられる。
- $ 1\ ≦\ a_i\ ≦\ 10^9\ (1\ ≦\ i\ ≦\ N) $ であることが保証される。
- $ 1\ ≦\ b_j\ ≦\ 10^9\ (1\ ≦\ j\ ≦\ M) $ であることが保証される。
- $ a_i\ <\ a_{i+1}\ (1\ ≦\ i\ ≦\ N-1) $ であることが保証される。
- $ b_i\ <\ b_{j+1}\ (1\ ≦\ j\ ≦\ M-1) $ であることが保証される。

## 输出格式

高橋くんが空港Aと空港Bの間を最大何往復できるかを $ 1 $ 行に出力せよ。

末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
3 4
2 3
1 5 7
3 8 12 13
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
1 1
1 1
1
1
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
6 7
5 3
1 7 12 19 20 26
4 9 15 23 24 31 33
```

### 输出 #3

```
3
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ 30 $ 点分のテストケースにおいて、$ 1\ ≦\ a_i\ ≦\ 10^5,\ 1\ ≦\ b_j\ ≦\ 10^5\ (\ 1\ ≦\ i\ ≦\ N,\ 1\ ≦\ j\ ≦\ M) $ を満たす。

### Sample Explanation 1

$ 1 $ 時の空港Aを出発する飛行機に乗り、$ 3 $ 時に到着しますが、すぐに $ 3 $ 時の空港Bを出発する飛行機に乗り、$ 6 $ 時に空港Aに到着します。 次に、$ 7 $ 時の空港Aを出発する飛行機に乗り、$ 9 $ 時に到着、$ 12 $ 時の空港Bを出発する飛行機に乗ると、合計 $ 2 $ 往復できます。$ 3 $ 往復する手段はありません。

### Sample Explanation 2

空港Bに行くと空港Aに帰れないので、$ 1 $ 度も往復できません。