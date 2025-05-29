## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc225/tasks/abc225_a

英小文字のみからなる長さ $ 3 $ の文字列 $ S $ が与えられます。

$ S $ の各文字を並び替えて得られる文字列は、何種類ありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ の各文字を並び替えて得られる文字列の種類数を出力せよ。

## 题目大意
输入一个长度为 $3$ 的，全部由英文小写字母组成的字符串 $s$ ，求将 $s$ 的所有字符重新排列后能得到多少种不同的字符串。

```input1
aba
```

```output1
3
```

```input2
ccc
```

```output2
1
```

```input3
xyz
```

```output3
6
```

## 提示
### 制約

- $ S $ は英小文字のみからなる長さ $ 3 $ の文字列

### Sample Explanation 1

$ S= $ `aba` の各文字を並び替えて得られる文字列は、`aab`, `aba`, `baa` の $ 3 $ 通りです。

### Sample Explanation 2

$ S= $ `ccc` の各文字を並び替えて得られる文字列は、`ccc` の $ 1 $ 通りのみです。

### Sample Explanation 3

$ S= $ `xyz` の各文字を並び替えて得られる文字列は、`xyz`, `xzy`, `yxz`, `yzx`, `zxy`, `zyx` の $ 6 $ 通りです。

