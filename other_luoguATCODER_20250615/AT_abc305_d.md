# AT_abc305_d [ABC305D] Sleep Log

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc305/tasks/abc305_d

高橋くんは睡眠記録をつけています。 睡眠記録は奇数長の数列 $ A=(A\ _\ 1(=0),\ A\ _\ 2,\ldots,A\ _\ N) $ で表され、奇数番目は起床時刻を、偶数番目は就寝時刻を表しています。 より厳密には、睡眠記録をつけている間に高橋くんは次のような睡眠をとりました。

- すべての $ 1\leq\ i\leq\dfrac{N-1}2 $ を満たす整数 $ i $ について、睡眠記録をつけ始めてから $ A\ _\ {2i} $ 分後ちょうどに寝て、$ A\ _\ {2i+1} $ 分後ちょうどに起きた。
- それ以外の時間に寝ることも起きることもなかった。
 
次の $ Q $ 個の質問に答えてください。 $ i $ 番目の質問では、$ 0\leq\ l\ _\ i\leq\ r\ _\ i\leq\ A\ _\ N $ を満たす整数の組 $ (l\ _\ i,r\ _\ i) $ が与えられます。

- 睡眠記録をつけ始めてから $ l\ _\ i $ 分後ちょうどから $ r\ _\ i $ 分後ちょうどまでの $ r\ _\ i-l\ _\ i $ 分のうち、高橋くんが寝ていたのは何分間ですか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A\ _\ 1 $ $ A\ _\ 2 $ $ \ldots $ $ A\ _\ N $ $ Q $ $ l\ _\ 1 $ $ r\ _\ 1 $ $ l\ _\ 2 $ $ r\ _\ 2 $ $ \vdots $ $ l\ _\ Q $ $ r\ _\ Q $

## 输出格式

答えを $ Q $ 行で出力せよ。 $ i $ 行目には $ i $ 番目の質問の答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7
0 240 720 1320 1440 1800 2160
3
480 1920
720 1200
0 2160
```

### 输出 #1

```
480
0
960
```

## 输入输出样例 #2

### 输入 #2

```
21
0 20 62 192 284 310 323 324 352 374 409 452 486 512 523 594 677 814 838 946 1000
10
77 721
255 541
478 970
369 466
343 541
42 165
16 618
222 592
730 983
338 747
```

### 输出 #2

```
296
150
150
49
89
20
279
183
61
177
```

## 说明/提示

### 制約

- $ 3\leq\ N\lt2\times10^5 $
- $ N $ は奇数
- $ 0=A\ _\ 1\lt\ A\ _\ 2\lt\cdots\lt\ A\ _\ N\leq10^9 $
- $ 1\leq\ Q\leq2\times10^5 $
- $ 0\leq\ l\ _\ i\leq\ r\ _\ i\leq\ A\ _\ N\ (1\leq\ i\leq\ Q) $
- 入力はすべて整数
 
### Sample Explanation 1

高橋くんは、以下の図のように睡眠をとりました。 ![](https://img.atcoder.jp/abc305/fe8152a63de7fea649d1d02197649a6a.png) それぞれの質問の答えは以下のようになります。 - 睡眠記録をつけ始めてから $ 480 $ 分後から $ 1920 $ 分後の間、高橋くんは $ 480 $ 分後から $ 720 $ 分後、$ 1320 $ 分後から $ 1440 $ 分後、$ 1800 $ 分後から $ 1920 $ 分後の $ 3 $ つの睡眠をとりました。睡眠時間の合計は $ 240+120+120=480 $ 分です。 - 睡眠記録をつけ始めてから $ 720 $ 分後から $ 1200 $ 分後の間、高橋くんは睡眠をとりませんでした。睡眠時間の合計は $ 0 $ 分です。 - 睡眠記録をつけ始めてから $ 0 $ 分後から $ 2160 $ 分後の間、高橋くんは $ 240 $ 分後から $ 720 $ 分後、$ 1320 $ 分後から $ 1440 $ 分後、$ 1800 $ 分後から $ 2160 $ 分後の $ 3 $ つの睡眠をとりました。睡眠時間の合計は $ 480+120+360=960 $ 分です。 よって、それぞれの行に $ 480,0,960 $ と出力してください。