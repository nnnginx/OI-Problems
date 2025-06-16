# AT_jsc2019_final_e Nearest String

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jsc2019-final/tasks/jsc2019_final_e

高橋くんは、文字列 $ a $ に対して、以下の $ 2 $ 種類の操作が行なえます。

- $ a $ の先頭、または末尾の $ 1 $ 文字を削除する。これには $ X $ のコストがかかる。
- $ a $ の末尾に、好きな $ 1 $ 文字を追加する。これには $ Y $ のコストがかかる。

高橋くんは今、$ N $ 個の文字列 $ S_0,S_1,\cdots,S_{N-1} $ を持っています。 高橋くんの友達の青木くんは、高橋くんに次の $ Q $ 個の質問を行います。

- 質問 $ i $ ($ 0\ \leq\ i\ \leq\ Q-1 $): 青木くんが文字列 $ T_i $ を見せる。 $ T_i $ に上記の操作を繰り返し行い、高橋くんの持っている $ N $ 個の文字列のいずれかに一致させるために必要なコストの最小値を求めよ。

多忙な高橋くんの代わりに、これらの質問に答えるプログラムを作成してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ Q $ $ X $ $ Y $ $ S_0 $ $ S_1 $ $ \vdots $ $ S_{N-1} $ $ T_0 $ $ T_1 $ $ \vdots $ $ T_{Q-1} $

## 输出格式

$ Q $ 行出力せよ。 $ i+1 $ ($ 0\ \leq\ i\ \leq\ Q-1 $) 行目には、質問 $ i $ の答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3 4 2
b
bcd
cd
a
ab
abc
```

### 输出 #1

```
6
4
6
```

## 输入输出样例 #2

### 输入 #2

```
4 3 1 100
a
aaaa
aaaaaaa
aaaaaaaaaa
aaa
aaaaaa
aaaaaaaaa
```

### 输出 #2

```
2
2
2
```

## 输入输出样例 #3

### 输入 #3

```
10 10 86 69
bbabbaaaaa
babaababab
bbababbbba
aaaaaaaaab
bbbbbbaabb
aabbabbbba
babbbbbbaa
baaabbaaaa
aaaaababbb
ababaaaaaa
bbaabbbbaa
abbbbabbbb
abbaaabaaa
ababaaaaab
bbaabbaaaa
abbbbbbabb
aabbbabbba
aaabbbaaaa
abbbababab
babaaabbbb
```

### 输出 #3

```
930
620
775
155
775
465
775
930
620
620
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ Q\ \leq\ 10^5 $
- $ 1\ \leq\ X,Y\ \leq\ 10^9 $
- $ 1\ \leq\ |S_i| $
- $ \sum_{i=0}^{N-1}\ |S_i|\ \leq\ 5\ \times\ 10^5 $
- $ S_i\ \neq\ S_j $ ($ i\ \neq\ j $)
- $ 1\ \leq\ |T_i| $
- $ \sum_{i=0}^{Q-1}\ |T_i|\ \leq\ 5\ \times\ 10^5 $
- $ T_i\ \neq\ T_j $ ($ i\ \neq\ j $)
- 入力される数はすべて整数である。
- 入力される文字列はすべて英小文字からなる文字列である。

### Sample Explanation 1

例えば、質問 $ 2 $ について考えると、以下のように操作するのが最適です。 - `abc` の先頭の文字を削除して、`bc` を得る。コストが $ 4 $ かかる。 - `bc` の末尾に `d` を追加して、`bcd` を得る。コストが $ 2 $ かかる。