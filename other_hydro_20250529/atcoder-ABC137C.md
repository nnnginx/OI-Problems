## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc137/tasks/abc137_c

文字列 $ a $ に含まれる文字を何らかの順序で並べることで得られる文字列を $ a $ の *アナグラム* と呼びます。

例えば、`greenbin` は `beginner` のアナグラムです。このように、同じ文字が複数回現れるときはその文字をちょうどその回数だけ使わなければなりません。

$ N $ 個の文字列 $ s_1,\ s_2,\ \ldots,\ s_N $ が与えられます。それぞれの文字列は長さが $ 10 $ で英小文字からなり、またこれらの文字列はすべて異なります。二つの整数 $ i,\ j $ $ (1\ \leq\ i\ <\ j\ \leq\ N) $ の組であって、$ s_i $ が $ s_j $ のアナグラムであるようなものの個数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ s_2 $ $ : $ $ s_N $

## 输出格式
二つの整数 $ i,\ j $ $ (1\ \leq\ i\ <\ j\ \leq\ N) $ の組であって、$ s_i $ が $ s_j $ のアナグラムであるようなものの個数を出力せよ。

## 题目大意
我们将调用通过以某种顺序排列字符串 $a$ 中包含的字符而获得的字符串，即 _anagram_。

例如，`greenbin` 是 `beginer` 的 _anagram_。 如此处所示，当同一字符多次出现时，该字符必须使用该次数。

给定 $N$ 个字符串 $s_1,s_2,\ldots,s_N$。每个字符串的长度为 $10$，由小写英文字符组成。 此外，所有这些字符串都是不同的。 找出整数对的数量 $(1 \leq i < j \leq N)$，使 $s_i$ 是 $s_j$ 的 _anagram_。

```input1
3
acornistnt
peanutbomb
constraint
```

```output1
1
```

```input2
2
oneplustwo
ninemodsix
```

```output2
0
```

```input3
5
abaaaaaaaa
oneplustwo
aaaaaaaaba
twoplusone
aaaabaaaaa
```

```output3
4
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ s_i $ は長さ $ 10 $ の文字列である。
- $ s_i $ の各文字は英小文字である。
- $ s_1,\ s_2,\ \ldots,\ s_N $ はすべて異なる。

### Sample Explanation 1

$ s_1\ = $ `acornistnt` は $ s_3\ = $ `constraint` のアナグラムです。他に $ s_i $ が $ s_j $ のアナグラムであるような $ i,\ j $ の組はないため、答えは $ 1 $ です。

### Sample Explanation 2

$ s_i $ が $ s_j $ のアナグラムであるような $ i,\ j $ の組がないときは $ 0 $ と出力してください。

### Sample Explanation 3

ここにそのようなケースを置くことはできませんが、答えは $ 32 $ bit 整数型に収まらない可能性があるので注意してください。

