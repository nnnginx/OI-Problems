# AT_agc014_b [AGC014B] Unplanned Queries

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc014/tasks/agc014_b

高橋君は木の問題が苦手です。そこで、青木君は高橋君の練習相手になってあげることにしました。

まず、高橋君は $ N $ 頂点からなる木を用意し、頂点に $ 1 $ から $ N $ の番号を付けました。 そして、各辺に $ 0 $ と書きました。

次に、青木君は高橋君に $ M $ 個のクエリを与えました。$ i $ 個目のクエリは以下のような内容です。

- 頂点 $ a_i $ と頂点 $ b_i $ を結ぶパス上の辺すべてに対して、書かれている数を $ 1 $ 増やす。

全てのクエリを終えた後、高橋君は青木君にどの辺を見ても書かれている数が偶数になったと伝えました。 しかし、青木君は最初に高橋君が用意していた木を確認していなかったので、 高橋君が正しくクエリを処理できたか分かりませんでした。

青木君を助けるために、高橋くんの言う性質を満たす木が存在するかどうかを判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_1 $ $ b_1 $ : $ a_M $ $ b_M $

## 输出格式

高橋くんの言う性質を満たす木が存在するならば `YES` を、存在しないならば `NO` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 4
1 2
2 4
1 3
3 4
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
5 5
1 2
3 5
5 1
3 4
2 3
```

### 输出 #2

```
NO
```

## 说明/提示

### 制約

- $ 2\ ≦\ N\ ≦\ 10^5 $
- $ 1\ ≦\ M\ ≦\ 10^5 $
- $ 1\ ≦\ a_i,b_i\ ≦\ N $
- $ a_i\ ≠\ b_i $

### Sample Explanation 1

例えば、頂点 $ 1 $ と頂点 $ 2,3,4 $ が辺で結ばれているような木を高橋君が持っている場合は、高橋くんの言っていることは正しいです。 この場合、クエリをすべて終えた後各辺に書かれている数はどれも $ 2 $ になります。