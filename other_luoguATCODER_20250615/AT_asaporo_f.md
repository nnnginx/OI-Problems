# AT_asaporo_f 数字列をカンマで分ける問題

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf16-tournament-round1-open/tasks/asaporo_f

`1` から `9` までの数字のみで構成された文字列 $ S $ が与えられます。 この文字列に、$ K $ 個以下のカンマ(`,`)を 挿入し、複数の数に分けたいと思います。

この操作をした際に現れる数の最大値を最小化したとき、その値を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $ $ S $

## 输出格式

求める整数を $ 1 $ 行で出力しなさい。

## 输入输出样例 #1

### 输入 #1

```
2
15267315
```

### 输出 #1

```
315
```

## 输入输出样例 #2

### 输入 #2

```
0
12456174517653111
```

### 输出 #2

```
12456174517653111
```

## 输入输出样例 #3

### 输入 #3

```
8
127356176351764127645176543176531763517635176531278461856198765816581726586715987216581
```

### 输出 #3

```
5317635176
```

## 说明/提示

### 制約

- $ 0\ ≦\ K\ <\ |S|\ ≦\ 100,000 $
- $ S $ は `1` から `9` までの数字のみからなる。

### 部分点

- $ 100 $ 点分のデータセットでは、$ |S|\ ≦\ 2 $ が成り立つ。
- 別の $ 100 $ 点分のデータセットでは、$ |S|\ ≦\ 16 $ が成り立つ。
- 別の $ 200 $ 点分のデータセットでは、$ |S|\ ≦\ 100 $ が成り立つ。
- 別の $ 200 $ 点分のデータセットでは、$ |S|\ ≦\ 2,000 $ が成り立つ。

### Sample Explanation 1

$ 152 $, $ 67 $, $ 315 $ と区切ると、最大値が $ 315 $ となり、これが答えとなります。

### Sample Explanation 2

$ 12456174517653111 $ がそのまま答えとなります。