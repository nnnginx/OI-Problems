# AT_discovery_2016_qual_a DISCO presents ディスカバリーチャンネルプログラミングコンテスト 2016

## 题目描述

[problemUrl]: https://atcoder.jp/contests/discovery2016-qual/tasks/discovery_2016_qual_a

あなたはDISCO presents ディスカバリーチャンネルプログラミングコンテスト 2016に参加しようと考え、公式サイトを確認しています。 公式サイトには`DiscoPresentsDiscoveryChannelProgrammingContest2016`とだけ書いてあります。

あなたが持っているPCのディスプレイは $ 1 $ 行に $ W $ 文字までしか表示することができません。そのため、 $ W+1 $ 文字目以降は改行され、次の行に表示されます。 具体的な表示例についてはサンプルを確認してください。

さて、あなたのPCのディスプレイでは`DiscoPresentsDiscoveryChannelProgrammingContest2016`はどのように表示されているでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ W $

- $ 1 $ 行目に $ 1 $ 行に表示可能な文字数を表す整数 $ W\ (1≦W≦51) $ が与えられる。

## 输出格式

表示結果を出力せよ。末尾の改行を忘れないこと。表示例についてはサンプルを確認せよ。

## 输入输出样例 #1

### 输入 #1

```
40
```

### 输出 #1

```
DiscoPresentsDiscoveryChannelProgramming
Contest2016
```

## 输入输出样例 #2

### 输入 #2

```
17
```

### 输出 #2

```
DiscoPresentsDisc
overyChannelProgr
ammingContest2016
```

## 输入输出样例 #3

### 输入 #3

```
51
```

### 输出 #3

```
DiscoPresentsDiscoveryChannelProgrammingContest2016
```

## 说明/提示

### Sample Explanation 1

\- このケースにおいては $ 2 $ 行にわたって出力が行われます。 - このディスプレイは $ 1 $ 行に $ 40 $ 文字までしか表示することができないので $ 41 $ 文字目からは次の行に表示されています。 - $ 2 $ 行目は`Contest2016`の $ 10 $ 文字が表示されています。余分な空白文字や改行、末尾の改行忘れには注意してください。

### Sample Explanation 2

\- このケースにおいては $ 3 $ 行にわたって出力が行われます。 - このディスプレイは $ 1 $ 行に $ 17 $ 文字までしか表示することができないので $ 18 $ 文字目、 $ 35 $ 文字目からは次の行に表示されています。 - $ 3 $ 行目は`ammingContest2016`の $ 17 $ 文字が表示されています。余分な空白文字や改行、末尾の改行忘れには注意してください。

### Sample Explanation 3

\- このケースにおいては出力は $ 1 $ 行に収まります。余分な空白文字や改行、末尾の改行忘れには注意してください。