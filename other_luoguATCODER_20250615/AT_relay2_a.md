# AT_relay2_a Kaiden

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf17-relay-open/tasks/relay2_a

*ButCoder株式会社* は、プログラミングコンテストサイト「*ButCoder*」を運営しています。このサイトでは、ユーザーにはレーティングという技量を表す整数値が与えられ、その値はユーザーがコンテストに参加するたびに変動します。新規ユーザーのレーティングの初期値は $ 0 $ であり、レーティングが $ K $ 以上に達したユーザーは *皆伝* と呼ばれます。なお、レーティングは負になることもあります。

低橋くんというユーザーが ButCoder に新たに登録しました。彼のレーティングは、彼が奇数回目に参加するコンテスト（$ 1 $ 回目、$ 3 $ 回目、$ 5 $ 回目$ … $）では毎回 $ A $ 増加し、偶数回目に参加するコンテスト（$ 2 $ 回目、$ 4 $ 回目、$ 6 $ 回目$ … $）では毎回 $ B $ 減少することが予測されます。

この予測によると、彼が初めて皆伝になるのは何回のコンテストに参加した直後でしょうか、もしくは彼は永遠に皆伝になれないでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $ $ A $ $ B $

## 输出格式

低橋くんが永遠に皆伝にならないと予測される場合は、`-1` と出力せよ。そうでない場合は、彼が初めて皆伝になるまでのコンテストの回数の予測値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4000 2000 500
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
4000 500 2000
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
1000000000000000000 2 1
```

### 输出 #3

```
1999999999999999997
```

## 说明/提示

### 制約

- $ 1\ <\ =\ K,\ A,\ B\ <\ =\ 10^{18} $
- 入力値はすべて整数である。

### Sample Explanation 1

低橋くんがコンテストに参加するたびに、彼のレーティングは $ 0 $ → $ 2000 $ → $ 1500 $ → $ 3500 $ → $ 3000 $ → $ 5000 $ → … と変動することが予測されます。彼のレーティングが $ 4000 $ 以上に到達するのは、$ 5 $ 回目の参加の直後です。

### Sample Explanation 2

低橋くんがコンテストに参加するたびに、彼のレーティングは $ 0 $ → $ 500 $ → $ -1500 $ → $ -1000 $ → $ -3000 $ → $ -2500 $ → … と変動することが予測されます。彼が皆伝になることは永遠にありません。

### Sample Explanation 3

入力される値や出力すべき値は $ 32 $ bit 整数に収まらないことがあります。