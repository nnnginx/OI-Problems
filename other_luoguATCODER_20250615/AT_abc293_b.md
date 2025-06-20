# AT_abc293_b [ABC293B] Call the ID Number

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc293/tasks/abc293_b

人 $ 1 $ 、人 $ 2 $ 、$ \ldots $ 、人 $ N $ と**番号**をつけられた $ N $ 人の人がいます。

$ N $ 人は、人 $ 1 $ 、人 $ 2 $ 、$ \ldots $ 、人 $ N $ の順番に下記の行動をちょうど $ 1 $ 回ずつ行います。

- 人 $ i $ 自身がまだ一度も番号を呼ばれていないなら、人 $ A_i $ の番号を呼ぶ。
 
最後まで番号を一度も呼ばれない人全員の番号を**昇順に**列挙してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

下記の形式にしたがって、最後まで番号を一度も呼ばれない人全員の番号を昇順に列挙せよ。

> $ K $ $ X_1 $ $ X_2 $ $ \ldots $ $ X_K $

すなわち、まず $ 1 $ 行目に、最後まで番号を一度も呼ばれない人の人数 $ K $ を出力し、 $ 2 $ 行目に、最後まで番号を一度も呼ばれない人全員の番号を昇順に並べた列 $ (X_1,\ X_2,\ \ldots,\ X_K) $ を空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
3 1 4 5 4
```

### 输出 #1

```
2
2 4
```

## 输入输出样例 #2

### 输入 #2

```
20
9 7 19 7 10 4 13 9 4 8 10 15 16 3 18 19 12 13 2 12
```

### 输出 #2

```
10
1 2 5 6 8 11 14 17 18 20
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ N $
- $ A_i\ \neq\ i $
- 入力はすべて整数
 
### Sample Explanation 1

$ 5 $ 人の行動は下記の通りです。 - 人 $ 1 $ はまだ番号を一度も呼ばれていないので、人 $ 1 $ は人 $ 3 $ の番号を呼びます。 - 人 $ 2 $ はまだ番号を一度も呼ばれていないので、人 $ 2 $ は人 $ 1 $ の番号を呼びます。 - 人 $ 3 $ はすでに人 $ 1 $ によって番号を呼ばれているので、何もしません。 - 人 $ 4 $ はまだ番号を一度も呼ばれていないので、人 $ 4 $ は人 $ 5 $ の番号を呼びます。 - 人 $ 5 $ はすでに人 $ 4 $ によって番号を呼ばれているので、何もしません。 よって、最後まで番号を一度も呼ばれないのは人 $ 2 $ と人 $ 4 $ です。