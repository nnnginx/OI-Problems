## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc172/tasks/abc172_b

文字列 $ S $, $ T $ が与えられます。次の操作を繰り返して $ S $ を $ T $ に変更するとき、操作回数の最小値を求めてください。

操作：$ S $ の $ 1 $ 文字を選んで別の文字に書き換える

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式
答えを出力せよ。

## 题目大意
输入两个字符串，输出他们有几位是不同的。

```input1
cupofcoffee
cupofhottea
```

```output1
4
```

```input2
abcde
bcdea
```

```output2
5
```

```input3
apple
apple
```

```output3
0
```

## 提示
### 制約

- $ S $, $ T $ は長さ $ 1 $ 以上 $ 2\times\ 10^5 $ 以下
- $ S $, $ T $ は英小文字のみからなる
- $ S $ と $ T $ の長さは等しい

### Sample Explanation 1

例えば、次のような $ 4 $ 回の操作で達成できます。 - $ 1 $ 回目：$ 6 $ 文字目の `c` を `h` に書き換える - $ 2 $ 回目：$ 8 $ 文字目の `f` を `t` に書き換える - $ 3 $ 回目：$ 9 $ 文字目の `f` を `t` に書き換える - $ 4 $ 回目：$ 11 $ 文字目の `e` を `a` に書き換える

### Sample Explanation 3

$ 1 $ 度も操作をしなくてもよいこともあります。

