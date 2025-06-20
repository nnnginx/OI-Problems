# AT_discovery_2016_qual_d DDPC特別ビュッフェ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/discovery2016-qual/tasks/discovery_2016_qual_d

$ A $ 君と $ B $ 君はDISCO presents ディスカバリーチャンネルプログラミングコンテスト 2016本戦のDDPC特別ビュッフェを楽しんでいます。 $ A $ 君のトレーには $ N $ 個の料理が、 $ B $ 君のトレーは $ M $ 個の料理が置かれています。 $ A $ 君のトレーにある $ i $ 番目の料理の美味しさは $ A_i $で、 $ B $ 君のトレーにある $ j $ 番目の料理の美味しさは $ B_j $ で表されます。

とっても仲良しな $ 2 $ 人はより昼食を楽しむため、$ A $ 君のトレーにある料理 $ 1 $ つと、 $ B $ 君のトレーにある料理 $ 1 $ つを交換するという操作をちょうど $ K $ 回行うことにしました。 $ A $ 君のトレーにある料理の美味しさの総和が $ a $ で、 $ B $ 君のトレーにある料理の美味しさの総和が $ b $ で表されるとき、 $ 2 $人の幸福度は $ a×b $ で表されます。

$ K $ 回交換を行ったあとのありうる幸福度のうち、最大の値を求めなさい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ A_2 $ … $ A_N $ $ B_1 $ $ B_2 $ … $ B_M $

- $ 1 $ 行目に $ A $ 君と $ B $ 君の持っている料理の数を表す整数 $ N,\ M\ (1≦N,M≦55) $ と料理の交換回数 $ K(1≦K≦999) $ が与えられる。
- $ 2 $ 行目に $ A $ 君のトレーに置かれている $ i $ 番目の料理の美味しさを表す整数 $ A_i\ (0≦A_i≦22,222) $ が空白区切りで与えられる。
- $ 3 $ 行目に $ B $ 君のトレーに置かれている $ j $ 番目の料理の美味しさを表す整数 $ B_j\ (0≦B_j≦22,222) $ が空白区切りで与えられる。

## 输出格式

ありうる $ 2 $ 人の幸福度の最大値を $ 1 $ 行に出力せよ。末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
3 2 1
2 2 3
3 2
```

### 输出 #1

```
36
```

## 输入输出样例 #2

### 输入 #2

```
3 2 2
2 2 2
3 3
```

### 输出 #2

```
36
```

## 说明/提示

### 部分点

この問題には部分点が設定されている。

- $ K=1 $ を満たすデータセットに正解した場合 $ 10 $ 点が与えられる。
- $ 0≦A_i,B_j≦55 $を満たすようなデータセットに正解した場合上記の部分点とは別に $ 20 $ 点が与えられる。
- 追加制約のないデータセットに正解した場合さらに $ 70 $ 点が得られ合計 $ 100 $ 点が得られる。

### Sample Explanation 1

\- $ A $ 君のトレーにある美味しさ $ 3 $ の料理と $ B $ 君のトレーにある美味しさ $ 2 $ の料理を交換すると $ 2 $ 人の幸福度は $ 36 $ となり、これが最大の幸福度です。

### Sample Explanation 2

\- $ 1 $ 回目の交換で $ A $ 君のトレーにある美味しさ $ 2 $ の料理と $ B $ 君のトレーにある美味しさ $ 3 $ の料理を交換し、 $ 2 $ 回目の交換で $ A $ 君のトレーにある美味しさ $ 3 $ の料理と $ B $ 君のトレーにある美味しさ $ 2 $ の料理を交換すると $ 2 $ 人の幸福度は $ 36 $ となり、これが最大の幸福度です。