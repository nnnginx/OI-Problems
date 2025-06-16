## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc168/tasks/abc168_b

英小文字からなる文字列 $ S $ があります。

$ S $ の長さが $ K $ 以下であれば、$ S $ をそのまま出力してください。

$ S $ の長さが $ K $ を上回っているならば、先頭 $ K $ 文字だけを切り出し、末尾に `...` を付加して出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ K $ $ S $

## 输出格式
問題文の通りに出力せよ。

## 题目大意
给一段由小写字母构成的字符串 $S$ 及限制 $K$ 。如果 $S$ 的长度超过 $K$ ，就将 $S$ 的前  $K$ 个字符输出，再输出 ... 。否则，就直接输出整个字符串。

```input1
7
nikoandsolstice
```

```output1
nikoand...
```

```input2
40
ferelibenterhominesidquodvoluntcredunt
```

```output2
ferelibenterhominesidquodvoluntcredunt
```

## 提示
### 制約

- $ K $ は $ 1 $ 以上 $ 100 $ 以下の整数
- $ S $ は英小文字からなる文字列
- $ S $ の長さは $ 1 $ 以上 $ 100 $ 以下

### Sample Explanation 1

`nikoandsolstice` の長さは $ 15 $ であり、$ K=7 $ を上回っています。 この先頭 $ 7 $ 文字を切り出して末尾に `...` を付加した文字列 `nikoand...` を出力します。

### Sample Explanation 2

ガイウス・ユリウス・カエサルの名言です。

