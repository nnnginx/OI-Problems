## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc110/tasks/abc110_c

英小文字のみからなる文字列 $ S $, $ T $ が与えられます。

文字列 $ S $ に対して、次の操作を何度でも行うことができます。

操作: 2つの異なる英小文字 $ c_1 $, $ c_2 $ を選び、$ S $ に含まれる全ての $ c_1 $ を $ c_2 $ に、$ c_2 $ を $ c_1 $ に置き換える

$ 0 $ 回以上操作を行って、$ S $ を $ T $ に一致させられるか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式
$ S $ を $ T $ に一致させられる場合は `Yes`、そうでない場合は `No` を出力せよ。

## 题目大意
您会得到由小写英文字母组成的字符串 $S$ 和 $T$。

您可以在 $S$ 上多次执行以下操作：

操作：选择两个不同的小写英文字母 $c_1$ 和 $c_2$，然后将每次出现的 $c_1$ 替换为 $c_2$，并将每次出现的 $c_2$ 替换为 $c_1$。

通过执行零次或更多次操作，确定 $S$ 和 $T$ 是否可以相等。

```input1
azzel
apple
```

```output1
Yes
```

```input2
chokudai
redcoder
```

```output2
No
```

```input3
abcdefghijklmnopqrstuvwxyz
ibyhqfrekavclxjstdwgpzmonu
```

```output3
Yes
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 2\ \times\ 10^5 $
- $ |S|\ =\ |T| $
- $ S $, $ T $ は英小文字のみからなる

### Sample Explanation 1

次のように操作を行えば、`azzel` を `apple` にできます。 - $ c_1 $ として `e` を、$ c_2 $ として `l` を選ぶと、`azzel` が `azzle` になる - $ c_1 $ として `z` を、$ c_2 $ として `p` を選ぶと、`azzle` が `apple` になる

### Sample Explanation 2

どのように操作を行っても `chokudai` を `redcoder` にできません。

