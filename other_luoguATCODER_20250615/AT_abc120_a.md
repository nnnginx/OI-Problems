# AT_abc120_a [ABC120A] Favorite Sound

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc120/tasks/abc120_a

高橋くんは、自動販売機でジュースを買ったときの音が好きです。

その音は $ 1 $ 回 $ A $ 円で聞くことができます。

高橋くんは $ B $ 円持っていますが、お気に入りの音を $ C $ 回聞くと満足するため、$ B $ 円で最大 $ C $ 回まで聞けるだけ聞きます。

高橋くんはお気に入りの音を何回聞くことになるでしょうか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $

## 输出格式

高橋くんはお気に入りの音を何回聞くことになるか出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 11 4
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
3 9 5
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
100 1 10
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ A,\ B,\ C\ \leq\ 100 $

### Sample Explanation 1

高橋くんは $ 8 $ 円以上持っているのでお気に入りの音を $ 4 $ 回聞いて満足します。

### Sample Explanation 2

高橋くんが満足できないこともあります。