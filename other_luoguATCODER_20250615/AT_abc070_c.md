# AT_abc070_c [ABC070C] Multiple Clocks

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc070/tasks/abc070_c

$ N $ 台の時計があり、$ i(1≦i≦N) $ 番目の時計の針はちょうど $ T_i $ 秒で時計盤を $ 1 $ 周します。   
 最初、全ての時計の針は真っ直ぐ上に向いており、止まっています。   
 イルカは、全ての時計の針を同時に動かし始めました。   
 再び、全ての時計の針が真っ直ぐ上に向くのは何秒後でしょうか?

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ T_1 $ $ : $ $ T_N $

## 输出格式

時計の針を動かし始めてから、再び全ての時計の針が真っ直ぐ上に向くまでの秒数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
2
3
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
5
2
5
10
1000000000000000000
1000000000000000000
```

### 输出 #2

```
1000000000000000000
```

## 说明/提示

### 制約

- $ 1≦N≦100 $
- $ 1≦T_i≦10^{18} $
- 入力は全て整数である。
- 答えは $ 10^{18} $ 秒以内である。

### Sample Explanation 1

$ 2 $ つの時計があり、各時計の針が真っ直ぐ上に向くのは以下の時刻です。 - $ 1 $ 番目の時計の針: 時計の針を動かし始めてから、$ 2 $ 秒後、$ 4 $ 秒後、$ 6 $ 秒後、$ ... $ - $ 2 $ 番目の時計の針: 時計の針を動かし始めてから、$ 3 $ 秒後、$ 6 $ 秒後、$ 9 $ 秒後、$ ... $ したがって、$ 2 $ つの時計の針が真っ直ぐ上に向くのにかかる秒数は $ 6 $ 秒となります。