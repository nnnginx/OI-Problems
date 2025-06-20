# AT_abc149_b [ABC149B] Greedy Takahashi

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc149/tasks/abc149_b

高橋君は $ A $ 枚、青木君は $ B $ 枚のクッキーを持っています。

高橋君は以下の行動を $ K $ 回繰り返します。

- もし高橋君がクッキーを $ 1 $ 枚以上持っているなら、高橋君のクッキーを $ 1 $ 枚食べる。
- そうでなく、もし青木君がクッキーを $ 1 $ 枚以上持っているなら、青木君のクッキーを $ 1 $ 枚食べる。
- 高橋君も青木君もクッキーを持っていないなら、何もしない。

高橋君と青木君が最終的に持っているクッキーの枚数をそれぞれ求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ K $

## 输出格式

高橋君と青木君のそれぞれが最終的に持っているクッキーの枚数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3 3
```

### 输出 #1

```
0 2
```

## 输入输出样例 #2

### 输入 #2

```
500000000000 500000000000 1000000000000
```

### 输出 #2

```
0 0
```

## 说明/提示

### 制約

- $ 0\ \leq\ A\ \leq\ 10^{12} $
- $ 0\ \leq\ B\ \leq\ 10^{12} $
- $ 0\ \leq\ K\ \leq\ 10^{12} $
- 入力中のすべての値は整数である。

### Sample Explanation 1

高橋君は次のように行動します。 - 高橋君はクッキーを $ 2 $ 枚持っているので、自分のクッキーを $ 1 $ 枚食べる。 - 高橋君はクッキーを $ 1 $ 枚持っているので、自分のクッキーを $ 1 $ 枚食べる。 - 高橋君はクッキーを持っておらず、青木君はクッキーを $ 3 $ 枚持っているので、青木君のクッキーを $ 1 $ 枚食べる。 したがって、最終的に持っているクッキーの枚数は、高橋君が $ 0 $ 枚、青木君が $ 2 $ 枚になります。

### Sample Explanation 2

オーバーフローに注意してください。