# AT_abc229_h [ABC229H] Advance or Eat

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc229/tasks/abc229_h

$ N $ 行 $ N $ 列のグリッドがあり、各マスには白い駒が $ 1 $ 個置かれているか、黒い駒が $ 1 $ 個置かれているか、何も置かれていないかのいずれかです。  
 上から $ i $ 行目、左から $ j $ 列目のマスの状態は $ S_{i,j} $ で表され、`W` のとき白い駒が置かれていて、`B` のとき黒い駒が置かれていて、`.` のときは何も置かれていない空マスです。

高橋君とすぬけ君がゲームをします。高橋君からはじめて、交互にターンが回ってきます。

高橋君のターンには、

- $ 1 $ つ上に空マスがあるような**白**い駒を $ 1 $ つ選び、上に進める
- 好きな**黒**い駒を $ 1 $ つ食べる

のいずれかの操作をします。

すぬけ君のターンには、

- $ 1 $ つ上に空マスがあるような**黒**い駒を $ 1 $ つ選び、上に進める
- 好きな**白**い駒を $ 1 $ つ食べる

のいずれかの操作をします。

操作ができなくなった方が負けとします。両者が最適に行動するとき、どちらが勝ちますか？

なお「駒を上に進める」とは、$ i $ 行 $ j $ 列目の駒を $ i-1 $ 行 $ j $ 列目に移動させることを指します。  
 高橋君とすぬけ君は同じ向きから盤面を見ていて、「上」というのは両者にとって同じ向きであることに注意してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_{1,1}S_{1,2}\ldots\ S_{1,N} $ $ S_{2,1}S_{2,2}\ldots\ S_{2,N} $ $ \vdots $ $ S_{N,1}S_{N,2}\ldots\ S_{N,N} $

## 输出格式

高橋君が勝つならば `Takahashi` と、すぬけ君が勝つならば `Snuke` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
BB.
.B.
...
```

### 输出 #1

```
Takahashi
```

## 输入输出样例 #2

### 输入 #2

```
2
..
WW
```

### 输出 #2

```
Snuke
```

## 输入输出样例 #3

### 输入 #3

```
4
WWBW
WWWW
BWB.
BBBB
```

### 输出 #3

```
Snuke
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 8 $
- $ N $ は整数
- $ S_{i,j} $ は `W` または `B` または `.` である

### Sample Explanation 1

はじめに高橋君が $ 1 $ 行 $ 1 $ 列目の黒い駒を食べると、盤面は下のようになります。 ``` .B. .B. ... ``` このときすぬけ君は操作を行うことができないので、高橋君の勝ちです。 盤面の外に駒を動かすことや、他の駒があるマスに駒を移動させることはできないことに注意してください。