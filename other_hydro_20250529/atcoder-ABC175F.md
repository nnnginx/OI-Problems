## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc175/tasks/abc175_f

英小文字から成る $ N $ 個の文字列 $ S_1,\ S_2,\ \cdots,\ S_N $ があります。

高橋君はまずこれらの文字列から重複を許して合計 $ 1 $ 個以上選んだ後、選んだ文字列を好きな順番で連結することで、回文であるような文字列を作ろうとしています。

文字列 $ S_i $ を $ 1 $ 個使うにはコストが $ C_i $ かかり、同じ文字列であっても使った個数の分だけコストがかかります。

上述の方法で回文を作ることのできるように文字列を選ぶ方法のうち、コストの和としてありうる値の最小値を求めてください。

また、どのように選んでも回文を作ることが不可能である場合は $ -1 $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ C_1 $ $ S_2 $ $ C_2 $ $ : $ $ S_N $ $ C_N $

## 输出格式
回文を作ることのできるように文字列を選ぶ方法のうち、コストの和としてありうる値の最小値を出力せよ。不可能である場合は $ -1 $ を出力せよ。

## 题目大意
### 题目大意

有 $N$ 个仅含小写字母的字符串 $S_1,S_2,\cdots,S_N$。你需要把从这些字符串中选择一些以任意顺序拼接起来，同一个字符串可以被选择多次。每选择一次 $S_i$，你都需要花费 $C_i$ 的代价，也就是说你选择 $S_i$ 所花费的代价为 $C_i$ 与 $S_i$ 被选择的次数之积。求使拼接得到的字符串为回文串所需的最小花费。若不管如何都无法拼接成回文串，输出 `-1`。

数据范围：$1 \le N \le 50$，$1 \le |S_i| \le 20$，$1 \le C_i \le 10^9$。

### 输入格式

第一行一个整数 $N$，接下来 $N$ 行每行一个字符串 $S_i$ 和一个整数 $C_i$。

### 输出格式

一个整数，为最小代价或 `-1`。

### 样例解释

样例 1：我们可以分别选择一次 `abc` 与 `ba`，拼接得到回文串 `abcba`，花费为 $(3+4=7)$，为最小值。

样例 2：选择一次 `abcab`，两次 `cba`，拼接得到回文串 `abcabcbacba`，花费为 $(5+3\times2=11)$，为最小值。

样例 3：选择 `ab` 与 `cba` 花费的代价比仅选择 `a` 更少。

样例 4：无法拼成回文串。

（翻译 by @CarroT1212）

```input1
3
ba 3
abc 4
cbaa 5
```

```output1
7
```

```input2
2
abcab 5
cba 3
```

```output2
11
```

```input3
4
ab 5
cba 3
a 12
ab 10
```

```output3
8
```

```input4
2
abc 1
ab 2
```

```output4
-1
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ 1\ \leq\ |S_i|\ \leq\ 20 $
- $ S_i $ は英小文字から成る
- $ 1\ \leq\ C_i\ \leq\ 10^9 $

### Sample Explanation 1

`ba`, `abc`, `cbaa` があります。 例えば、`ba`, `abc` を $ 1 $ 個ずつ使うとコストは $ 7 $ で、`abc`, `ba` の順で連結すると回文になります。 また、`abc`, `cbaa` を $ 1 $ 個ずつ使うとコストは $ 9 $ で、`cbaa`, `abc` の順で連結すると回文になります。 コスト $ 7 $ 未満で回文を作ることはできないので、$ 7 $ を出力してください。

### Sample Explanation 2

`abcab` を $ 1 $ 個、`cba` を $ 2 $ 個選んで、`abcab`, `cba`, `cba` の順で連結すると回文になり、コストは $ 11 $ です。

### Sample Explanation 3

`a` を $ 1 $ 個だけ選んで回文とすることもできますが、`ab` と `cba` を選んで連結する方がコストが小さいです。

### Sample Explanation 4

回文を作ることが不可能であるので、$ -1 $ を出力してください。

