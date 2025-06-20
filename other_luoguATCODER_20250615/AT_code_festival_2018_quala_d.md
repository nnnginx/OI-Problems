# AT_code_festival_2018_quala_d 通勤

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2018-quala/tasks/code_festival_2018_quala_d

高橋くんの家は $ x $ 軸上の点 $ 0 $ に、AtCoder 社のオフィスは $ x $ 軸上の点 $ D $ にあります。 また、$ x $ 軸上には $ N $ 個のガソリンスタンドがあり、これらの座標は $ X_1,\ X_2,\ ...,\ X_N $ です。

高橋くんは毎日家からオフィスまで自動車で移動します。 この自動車の燃料タンクの容量は $ F $ リットルであり、距離 $ 1 $ 移動するごとに燃料を $ 1 $ リットル消費します。 高橋くんは燃料タンクが満タンの状態で家を出発し、ガソリンスタンドを通るごとに以下のようにして自動車の燃料を補給します。

- 燃料が $ T $ リットル以上残っている場合、燃料を補給しない。
- そうでない場合、燃料タンクが満タンになるまで燃料を補給する。

オフィスへの移動の際、自動車は $ x $ 軸正方向にしか進むことができません。ガソリンスタンドでもオフィスでもない場所で燃料タンクが空になった場合、オフィスへの移動は失敗となります。

あなたは $ N $ 個のガソリンスタンドのうちのいくつか ($ 0 $ 個でも構いません) を書店に建て替えようとしています。 書店に建て替えるガソリンスタンドの集合であって、建て替えのあとも高橋くんが上記の方法で家からオフィスまで自動車で移動できるようなものの個数を $ 10^9\ +\ 7 $ で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ D $ $ F $ $ T $ $ N $ $ X_1 $ $ X_2 $ $ ... $ $ X_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 8 5 2
3 7
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
8 8 5 5
1 2 3 4 5
```

### 输出 #2

```
32
```

## 输入输出样例 #3

### 输入 #3

```
100 50 30 1
40
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
1000 752 687 10
94 186 299 395 406 430 772 782 807 999
```

### 输出 #4

```
1002
```

## 说明/提示

### 制約

- $ 0\ <\ T\ \leq\ F\ \leq\ 10^9 $
- $ 1\ \leq\ N\ \leq\ 100,000 $
- $ 0\ <\ X_1\ <\ X_2\ <\ ...\ <\ X_N\ <\ D\ \leq\ 10^9 $
- 入力値はすべて整数である。

### Sample Explanation 1

座標 $ X_1\ =\ 3,\ X_2\ =\ 7 $ のガソリンスタンドにそれぞれ $ 1,\ 2 $ の番号をつけたとき、条件を満たす集合は $ \{\} $, $ \{1\} $ の $ 2 $ 個となります。