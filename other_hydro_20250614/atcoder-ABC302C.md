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

## 题目大意
### 题目描述

给定 $ N $ 个长度为 $ M $ 的仅包含小写英文字母的字符串 $ S_1, S_2, \cdots, S_N $。保证 $ S_i $ 互不相同。

判断是否可以通过对这些字符串重新排序，得到一个新的字符串序列 $ T_1, T_2, \cdots, T_N $，使得：

- 对于任意 $ i $ 使得 $ 1 \le i \le N - 1 $，均满足 $ T_i $ 在改变**恰好一个**字母后可以等于 $ T_{i + 1} $。

### 数据范围

- $ 2 \le N \le 8 $
- $ 1 \le M \le 5 $
- 保证 $ S_i $ 长度为 $ M $，且仅由小写英文字母组成。$ (1 \le i \le N) $
- 保证 $ S_i $ 互不相同。

### 样例一解释

安排顺序如下：`abcd`，`abed`，`bbed`，`fbed`。满足条件。

### 样例二解释

无论如何对这两个字符串排序，均不可能满足条件。

```input1
4 4
bbed
abcd
abed
fbed
```

```output1
Yes
```

```input2
2 5
abcde
abced
```

```output2
No
```

```input3
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

```output3
Yes
```

## 提示
### 制約

- $ 2\ \le\ N\ \le\ 8 $
- $ 1\ \le\ M\ \le\ 5 $
- $ S_i $ は英小文字からなる長さ $ M $ の文字列である。$ (1\ \le\ i\ \le\ N) $
- $ S_i $ は互いに異なる。

### Sample Explanation 1

`abcd` , `abed` , `bbed` , `fbed` の順に並び替えると条件を満たします。

### Sample Explanation 2

どのように並び替えても条件を満たすことは出来ません。

