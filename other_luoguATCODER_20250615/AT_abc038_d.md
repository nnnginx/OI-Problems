# AT_abc038_d [ABC038D] プレゼント

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc038/tasks/abc038_d

高橋くんはプレゼントを用意することになりました。プレゼントの中身はすでに決まり、あとはプレゼントを入れる箱を用意するだけです。 高橋くんが使える箱は$ N $個あり、$ i $番目の箱は縦$ h_i $cm×横$ w_i $cmのサイズです。

プレゼントがより多くの箱に入っていたほうが面白いと考えた高橋くんは、なるべく多くの箱を入れ子にし、最も内側の箱にプレゼントを入れることにしました。 ある箱は、縦・横ともにより大きいサイズの箱にのみ入れることができます。また、ある箱は$ 1 $つまでしか他の箱を入れることはできません。

プレゼントを入れる箱を最大で何重の入れ子にできるか答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ w_1 $ $ h_1 $ $ w_2 $ $ h_2 $ : $ w_N $ $ h_N $

## 输出格式

プレゼントを包む箱の数の最大値を $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
3 3
1 1
2 2
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
2
4 5
4 3
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4
2 5
3 3
4 5
6 6
```

### 输出 #3

```
3
```

## 输入输出样例 #4

### 输入 #4

```
5
8 8
5 3
2 2
4 2
2 1
```

### 输出 #4

```
4
```

## 说明/提示

### 制約

- $ 1≦N≦10^5 $
- $ 1≦h_i≦10^5 $
- $ 1≦w_i≦10^5 $

### 部分点

- $ N\ ≦\ 1,000 $ を満たすテストケース全てに正解した場合、部分点として$ 30 $点が与えられる。

### Sample Explanation 1

外側の箱から順に、$ 1,\ 3,\ 2 $番目の箱でプレゼントを包むことができます。

### Sample Explanation 2

箱を$ 90 $度回転することはできないことに注意してください。また、ある箱を縦または横の長さが等しい箱に入れることはできません。