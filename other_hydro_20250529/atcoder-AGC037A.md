## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc037/tasks/agc037_a

英小文字からなる文字列 $ S $ が与えられます。以下の条件をみたす最大の正整数 $ K $ を求めてください。

- $ S $ の空でない $ K $ 個の文字列への分割 $ S=S_1S_2...S_K $ であって $ S_i\ \neq\ S_{i+1} $ ($ 1\ ≦\ i\ ≦\ K-1 $) を満たすものが存在する。

ただし、$ S_1,S_2,...,S_K $ をこの順に連結して得られる文字列のことを $ S_1S_2...S_K $ によって表しています。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
条件をみたす最大の正整数 $ K $ を出力せよ。

## 题目大意
- 给定一个字符串 $S$，请你找出一个最大的 $k$，使得将这个字符串划分成 $k$ 段后能够保证相邻的两段不相同。

- $1\le |S| \le 2\times 10^5$，且保证 $S$ 串内均为小写字母。

- translate by @[ShineEternal](https://www.luogu.com.cn/user/45475)。

```input1
aabbaa
```

```output1
4
```

```input2
aaaccacabaababc
```

```output2
12
```

## 提示
### 制約

- $ 1\ ≦\ |S|\ ≦\ 2\ \times\ 10^5 $
- $ S $ は英小文字からなる

### Sample Explanation 1

例えば `aa`,`b`,`ba`,`a` と $ S $ を $ 4 $ つの文字列に分割することができます。

