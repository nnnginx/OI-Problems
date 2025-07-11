# AT_abc035_c [ABC035C] オセロ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc035/tasks/abc035_c

黒の面に`0`、白の面に`1`が書かれた $ N $ 個のオセロの駒が、どの駒も黒の面が上を向くように一列に並べられています。その後、ある区間にある駒を全て裏返すという操作が $ Q $ 回だけ行なわれました。 具体的には $ i $ 回目の操作においては、左から $ l_i $ 番目の駒から $ r_i $ 番目の駒までの駒全てが裏返されました。

最終的な盤面を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ Q $ $ l_1 $ $ r_1 $ . . . $ l_Q $ $ r_Q $

- $ 1 $ 行目に駒の数と操作回数を表す $ 2 $ つの整数 $ N,Q\ (1≦N,Q≦200,000) $ が空白区切りで与えられる。
- $ 2 $ 行目から続く $ Q $ 行のうち $ i $ 行目においては、 $ i $ 回目の操作の範囲を表す $ 2 $ つの整数 $ l_i,\ r_i\ (1≦l_i≦r_i≦N) $ が空白区切りで与えられる。

## 输出格式

最終的な盤面を表す文字列 $ S $ を $ 1 $ 行に出力せよ。 $ S $ の左から $ i $ 文字目は左から $ i $ 番目の駒の上向きの面に書かれた数字となる。改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
5 4
1 4
2 5
3 3
1 5
```

### 输出 #1

```
01010
```

## 输入输出样例 #2

### 输入 #2

```
20 8
1 8
4 13
8 8
3 18
5 20
19 20
2 7
4 9
```

### 输出 #2

```
10110000011110000000
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ 1≦N,Q≦2,000 $ を満たすデータセットに正解した場合、 $ 60 $ 点が与えられる。
- 追加制約のないデータセットに正解した場合は、追加で $ 40 $ 点が与えられ、合計 $ 100 $ 点が得られる。

### Sample Explanation 1

\- 盤面ははじめ`00000`です。 - $ 1 $ 回目の操作により、 盤面は`11110`となります。 - $ 2 $ 回目の操作により、 盤面は`10001`となります。 - $ 3 $ 回目の操作により、 盤面は`10101`となります。 - $ 4 $ 回目の操作により、 盤面は`01010`となります。 - 最終的な盤面である`01010`が求める答えです。 - このケースは部分点の追加制約を満たします。

### Sample Explanation 2

\- このケースは部分点の追加制約を満たします。