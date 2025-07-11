# AT_abc358_b [ABC358B] Ticket Counter

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc358/tasks/abc358_b

AtCoder Land の入り口には $ 1 $ つのチケット売り場があり、来園客はこのチケット売り場の前に一列に並んで順にチケットを購入します。 チケットの購入手続きには一人当たり $ A $ 秒かかり、列の先頭の人がチケットを購入し終わると、（存在すれば）次の人がすぐさま購入手続きを開始します。

現在チケット売り場に並んでいる人はおらず、今から $ N $ 人の人が順にチケットを買いに来ます。 具体的には、$ i $ 番目の人は今から $ T_i $ 秒後にチケット売り場を訪れ、既に列が存在すればその最後尾に並び、存在しなければすぐさま購入手続きを開始します。 ここで、$ T_1\ <\ T_2\ <\ \dots\ <\ T_N $ です。

各 $ i\ (1\leq\ i\leq\ N) $ について、$ i $ 番目の人がチケットを購入し終わるのは今から何秒後か求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ T_1 $ $ T_2 $ $ \dots $ $ T_N $

## 输出格式

$ N $ 行出力せよ。 $ i\ (1\leq\ i\ \leq\ N) $ 行目には、$ i $ 番目の人がチケットを購入し終わるのは今から何秒後かを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 4
0 2 10
```

### 输出 #1

```
4
8
14
```

## 输入输出样例 #2

### 输入 #2

```
3 3
1 4 7
```

### 输出 #2

```
4
7
10
```

## 输入输出样例 #3

### 输入 #3

```
10 50000
120190 165111 196897 456895 540000 552614 561627 743796 757613 991216
```

### 输出 #3

```
170190
220190
270190
506895
590000
640000
690000
793796
843796
1041216
```

## 说明/提示

### 制約

- $ 1\leq\ N\ \leq\ 100 $
- $ 0\leq\ T_1\ <\ T_2\ <\ \dots\ <\ T_N\leq\ 10^6 $
- $ 1\leq\ A\leq\ 10^6 $
- 入力は全て整数
 
### Sample Explanation 1

時系列順に以下のように物事が進行します。 - $ 0 $ 秒後：$ 1 $ 番目の人がチケット売り場を訪れ、チケットの購入手続きを開始する。 - $ 2 $ 秒後：$ 2 $ 番目の人がチケット売り場を訪れ、$ 1 $ 番目の人の後ろに並ぶ。 - $ 4 $ 秒後：$ 1 $ 番目の人がチケットを購入し終え、$ 2 $ 番目の人が購入手続きを開始する。 - $ 8 $ 秒後：$ 2 $ 番目の人がチケットを購入し終える。 - $ 10 $ 秒後：$ 3 $ 番目の人がチケット売り場を訪れ、チケットの購入手続きを開始する。 - $ 14 $ 秒後：$ 3 $ 番目の人がチケットを購入し終える。

### Sample Explanation 2

時系列順に以下のように物事が進行します。 - $ 1 $ 秒後：$ 1 $ 番目の人がチケット売り場を訪れ、チケットの購入手続きを開始する。 - $ 4 $ 秒後：$ 1 $ 番目の人がチケットを購入し終えると同時に、$ 2 $ 番目の人がチケット売り場を訪れ、チケットの購入手続きを開始する。 - $ 7 $ 秒後：$ 2 $ 番目の人がチケットを購入し終えると同時に、$ 3 $ 番目の人がチケット売り場を訪れ、チケットの購入手続きを開始する。 - $ 10 $ 秒後：$ 3 $ 番目の人がチケットを購入し終える。