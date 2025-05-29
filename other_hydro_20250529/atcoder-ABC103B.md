## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc103/tasks/abc103_b

英小文字からなる文字列 $ S $, $ T $ が与えられます。

$ S $ を回転させて $ T $ に一致させられるか判定してください。

すなわち、以下の操作を任意の回数繰り返して $ S $ を $ T $ に一致させられるか判定してください。

操作: $ S\ =\ S_1\ S_2\ ...\ S_{|S|} $ のとき、$ S $ を $ S_{|S|}\ S_1\ S_2\ ...\ S_{|S|-1} $ に変更する

ここで、$ |X| $ は文字列 $ X $ の長さを表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式
$ S $ を回転させて $ T $ に一致させられる場合は `Yes`、一致させられない場合は `No` を出力せよ。

## 题目大意
你可以对一个字符串进行操作，把它的第一个字母插入到末尾

如你可以把`jingkong`变为`ingkongj`

给定两个字符串,请问是否可以通过不限次的操作将它们变为两个一样的字符串

- 保证字符串的长度大于等于2且小于等于100

- 保证两个字符串的长度相同

- 保证两个字符串只由小写字母组成

```input1
kyoto
tokyo
```

```output1
Yes
```

```input2
abc
arc
```

```output2
No
```

```input3
aaaaaaaaaaaaaaab
aaaaaaaaaaaaaaab
```

```output3
Yes
```

## 提示
### 制約

- $ 2\ \leq\ |S|\ \leq\ 100 $
- $ |S|\ =\ |T| $
- $ S $, $ T $ は英小文字からなる

### Sample Explanation 1

\- $ 1 $ 回目の操作で `kyoto` が `okyot` になります - $ 2 $ 回目の操作で `okyot` が `tokyo` になります

### Sample Explanation 2

何度操作を行っても `abc` と `arc` を一致させられません。

