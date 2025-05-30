## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc031/tasks/agc031_a

長さ $ N $ の文字列 $ S $ が与えられます。 $ S $ の部分列であって、すべて異なる文字からなるものの数を $ 10^9+7 $ で割った余りを答えてください。文字列として同一でも、異なる位置から取り出された部分列は区別して数えることとします。

ただし、文字列の部分列とは、文字列から文字をいくつか **正の個数** 取り出し、もとの文字列から順序を変えずにつなげたものを指します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
異なる文字からなる部分列の個数を $ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
给你一个长度为 $N$ 的仅由小写字母组成的字符串 $S$，统计其中所有每种字母出现均不超过一次的子序列个数，答案对 $10^9 + 7$ 取模。

字符串的子序列是由原字符串中不改变顺序的一个或多个字符串联而成的。两个子序列当且仅当其中每个字符在原字符串中的位置都相同时，才被视为是相同的。

```input1
4
abcd
```

```output1
15
```

```input2
3
baa
```

```output2
5
```

```input3
5
abcab
```

```output3
17
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100000 $
- $ S $ は英小文字からなる
- $ |S|=N $

### Sample Explanation 1

$ S $ 自体がすべて異なる文字からなるので、すべての部分列が条件を満たします。

### Sample Explanation 2

`b`, `a` ($ 2 $ 通り), `ba` ($ 2 $ 通り) の合計 $ 5 $ 通りが答えとなります。`baa` などは`a`が $ 2 $ 回現れるため当てはまらないことに注意してください。

