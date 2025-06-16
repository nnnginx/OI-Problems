# AT_abc302_c [ABC302C] Almost Equal

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc302/tasks/abc302_c

英小文字からなる長さ $ M $ の文字列 $ N $ 個 $ S_1,S_2,\dots,S_N $ が与えられます。ここで、$ S_i $ は互いに異なります。

これらを並び替えた文字列の列 $ T_1,T_2,\dots,T_N $ であって、以下の条件を満たすものが存在するか判定してください。

- $ 1\ \le\ i\ \le\ N-1 $ を満たす全ての整数 $ i $ に対して、$ T_i $ を $ 1 $ 文字だけ別の英小文字に変えて $ T_{i+1} $ にすることが出来る。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

問題文の条件を満たす列が存在するならば `Yes` を、そうでないならば `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 4
bbed
abcd
abed
fbed
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
2 5
abcde
abced
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
8 4
fast
face
cast
race
fact
rice
nice
case
```

### 输出 #3

```
Yes
```

## 说明/提示

### 制約

- $ 2\ \le\ N\ \le\ 8 $
- $ 1\ \le\ M\ \le\ 5 $
- $ S_i $ は英小文字からなる長さ $ M $ の文字列である。$ (1\ \le\ i\ \le\ N) $
- $ S_i $ は互いに異なる。

### Sample Explanation 1

`abcd` , `abed` , `bbed` , `fbed` の順に並び替えると条件を満たします。

### Sample Explanation 2

どのように並び替えても条件を満たすことは出来ません。