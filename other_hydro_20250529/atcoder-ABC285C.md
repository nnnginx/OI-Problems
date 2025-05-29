## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc285/tasks/abc285_c

別世界の AtCoder で開催されている AtCoder Big Contest では、 $ 10^{16} $ 問の問題が一度に出題されます。  
問題の ID は $ 1 $ 問目から順に `A`, `B`, ..., `Z`, `AA`, `AB`, ..., `ZZ`, `AAA`, ... と付けられています。

つまり、 ID は以下の順番で付けられています。

- 長さ $ 1 $ の英大文字からなる文字列を辞書順に並べたもの
- 長さ $ 2 $ の英大文字からなる文字列を辞書順に並べたもの
- 長さ $ 3 $ の英大文字からなる文字列を辞書順に並べたもの
- $ ... $

このコンテストに含まれる問題の ID である文字列 $ S $ が与えられるので、それが何問目か答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを整数として出力せよ。

## 题目大意
给你一个由大小写字母组成的字符串，A 对应 $1$，B 对应 2，C 对应 $3$，以此类推。最后将字符串看作一个二十六进制的整数，如 ABC 看作 $(123)_ {26}$，求这个数在十进制中对应的数。

translate by @[VT_SODC3DC3BSLF](https://www.luogu.com.cn/user/672333)

```input1
AB
```

```output1
28
```

```input2
C
```

```output2
3
```

```input3
BRUTMHYHIIZP
```

```output3
10000000000000000
```

## 提示
### 制約

- $ S $ は AtCoder Big Contest に含まれる問題の ID として正しい

### Sample Explanation 1

ID が `AB` である問題は、 AtCoder Big Contest の $ 28 $ 問目です。

### Sample Explanation 2

ID が `C` である問題は、 AtCoder Big Contest の $ 3 $ 問目です。

### Sample Explanation 3

ID が `BRUTMHYHIIZP` である問題は、 AtCoder Big Contest の $ 10^{16} $ 問目、すなわち最終問題です。

