# AT_arc047_a [ARC047A] タブの開きすぎ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc047/tasks/arc047_a

高橋君はブラウザでネットサーフィンをするのが大好きです。

しかし、タブを開きすぎる癖があるので、よくブラウザがクラッシュします。

高橋君が使っているブラウザは開かれているタブが $ L $ 個を超えるとクラッシュします。

ブラウザはクラッシュすると自動で再起動して、$ 1 $ 個のタブが開いている状態になります。

初め、高橋君のブラウザは $ 1 $ 個のタブが開かれている状態です。

そのあとの高橋君の「新しいタブを開く」と「タブを閉じる」の履歴が与えられるので、高橋君が何回ブラウザをクラッシュさせるかを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ L $ $ S $

- $ 1 $ 行目には高橋君が行った行動の個数を表す整数 $ N(1\ ≦\ N\ ≦\ 10^5) $ とブラウザがクラッシュする基準を表す整数 $ L(1\ ≦\ L\ ≦\ 10^5) $ が空白区切りで与えられる。
- $ 2 $ 行目には高橋君の行動の履歴を表す `+` と `-` のみからなる $ N $ 文字の文字列 $ S $ が与えられる。
- $ S $ は高橋君の行動を時系列順にならべたものであり、 `+` は新しいタブを開くことを、 `-` はあるタブを閉じることを表す。
- タブが $ 1 $ 個のときにタブを閉じることは無い。

## 输出格式

高橋君がブラウザをクラッシュさせる回数を表す整数を $ 1 $ 行に出力せよ。 出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
6 2
+++-++
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
20 20
++-+-+++--+++++-++++
```

### 输出 #2

```
0
```

## 说明/提示

### Sample Explanation 1

\- 最初のタブの個数は $ 1 $ 個です。 - $ 1 $ 回目の操作が終わったあとのタブの個数は $ 2 $ 個です。 - $ 2 $ 回目の操作が終わるとタブが $ 3 $ 個になりますが $ L $ より大きいのでブラウザはクラッシュして、タブは $ 1 $ 個になります。 - $ 3 $ 回目の操作が終わったあとのタブの個数は $ 2 $ 個です。 - $ 4 $ 回目の操作が終わったあとのタブの個数は $ 1 $ 個です。 - $ 5 $ 回目の操作が終わったあとのタブの個数は $ 2 $ 個です。 - $ 6 $ 回目の操作が終わるとタブが $ 3 $ 個になりますが $ L $ より大きいのでブラウザはクラッシュして、タブは $ 1 $ 個になります。 よって合計で $ 2 $ 回、ブラウザはクラッシュします。