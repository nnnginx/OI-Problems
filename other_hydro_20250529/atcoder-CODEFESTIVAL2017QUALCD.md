## 题目描述
[problemUrl]: https://atcoder.jp/contests/code-festival-2017-qualc/tasks/code_festival_2017_qualc_d

英小文字のみからなる文字列 $ s $ があります。 すぬけ君は、$ s $ をいくつかの空でない部分文字列へ分割しようとしています。 分割後の部分文字列を、左から順に $ s_1 $, $ s_2 $, $ ... $, $ s_N $ とします (このとき、$ s\ =\ s_1\ +\ s_2\ +\ ...\ +\ s_N $ です)。 すぬけ君は、次の条件が成り立つように $ s $ を分割しようとしています。

- 各 $ i $ ($ 1\ \leq\ i\ \leq\ N $) について、$ s_i $ の文字を並べ替えて回文が得られる。

条件が成り立つように $ s $ を分割するとき、$ N $ の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
条件が成り立つように $ s $ を分割するとき、$ N $ の最小値を求めよ。

## 题目大意
### 题目描述
给定一个字符串$\texttt{s}$，把$\texttt{s}$分成$N$个子串，要求每个子串中的字母经过一定的移动，会变成一个回文串（如`aab`经过一定的移动，变成了`aba`，`aba`是一个回文串），**且$N$最少**。
### 输入格式
一个字符串$\texttt{s}$（$1 \le \texttt{|s|} \le 2 \times 10^5$）
### 输出格式
一个正整数$N$，表示最少的子串个数。

```input1
aabxyyzz
```

```output1
2
```

```input2
byebye
```

```output2
1
```

```input3
abcdefghijklmnopqrstuvwxyz
```

```output3
26
```

```input4
abcabcxabcx
```

```output4
3
```

## 提示
### 制約

- $ 1\ \leq\ |s|\ \leq\ 2\ \times\ 10^5 $
- $ s $ は英小文字のみからなる。

### Sample Explanation 1

`aabxyyzz` = `aab` + `xyyzz` と分割すればよいです。 このとき、`aab` の文字を並べ替えて回文 `aba` が得られ、`xyyzz` の文字を並べ替えて回文 `zyxyz` が得られます。

### Sample Explanation 2

`byebye` の文字を並べ替えて回文 `byeeyb` が得られます。

### Sample Explanation 4

`abcabcxabcx` = `a` + `b` + `cabcxabcx` と分割すればよいです。

