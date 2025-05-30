## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_a

文字列 $ X $ が与えられます。$ X $ の長さは偶数であり、半分は `S` 、もう半分は `T` からなります。

高橋君は `ST` という文字列が苦手です。なので以下の操作を $ 10^{10000} $ 回行うことにしました。

- $ X $ の(連続な)部分文字列で `ST` となるもののうち、最も左側にあるものを取り除く。存在しないならば何もしない。

最終的に $ X $ は何文字になるかを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ X $

## 输出格式
$ 1 $ 行に問題の答えを出力する。

## 题目大意
## 题目描述
有一个字符串X，对它进行操作。 该串只含S和T，凡是S与T连在一起都要将它们一起去掉 现在进行若干次操作直到该串中没有连在一起的ST，问剩下的长度。
## 输入输出格式：
### 输入格式
仅一行X
### 输出格式
输出X的最终长度

```input1
TSTTSS
```

```output1
4
```

```input2
SSTTST
```

```output2
0
```

```input3
TSSTTTSS
```

```output3
4
```

## 提示
### 制約

- $ 2\ ≦\ |X|\ ≦\ 200,000 $
- $ X $ の長さは偶数
- $ X $ を構成する文字のうち半分は `S` であり、もう半分は `T` である

### 部分点

- $ 200 $ 点分のデータセットでは $ |X|\ ≦\ 200 $ が成り立つ

### Sample Explanation 1

$ 1 $ 回目の操作では `TSTTSS` の $ 2,3 $ 文字目が `ST` なので取り除きます。 $ X $ は `TTSS` になり、もう `ST` はないため残り $ 10^{10000}-1 $ 回は何もしません。 よって答えは $ 4 $ となります。

### Sample Explanation 2

`SSTTST` ⇒ `STST` ⇒ `ST` ⇒ `` となり、最終的に空文字列になります。

### Sample Explanation 3

`TSSTTTSS` ⇒ `TSTTSS` ⇒ `TTSS` となります。

