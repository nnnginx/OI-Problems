## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc241/tasks/abc241_a

$ 1 $ 桁の数字が表示される画面と、ボタンからなる機械があります。

画面に数字 $ k $ が表示されているとき、ボタンを $ 1 $ 回押すと画面の数字が $ a_k $ に変わります。

$ 0 $ が表示されている状態からボタンを $ 3 $ 回押すと、画面には何が表示されますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a_0 $ $ a_1 $ $ \dots $ $ a_9 $

## 输出格式
答えを出力せよ。

## 题目大意
小A拥有一个数字和一个按钮。

当前显示数字 $k$ 时，按下 $1$ 次按钮，数字会变为 $a_k$ 。



数字开始为 $0$ ，按 $3$ 次按钮，数字会变成什么？

```input1
9 0 1 2 3 4 5 6 7 8
```

```output1
7
```

```input2
4 8 8 8 0 8 8 8 8 8
```

```output2
4
```

```input3
0 0 0 0 0 0 0 0 0 0
```

```output3
0
```

## 提示
### 制約

- $ 0\leq\ a_i\ \leq\ 9 $
- 入力は全て整数である

### Sample Explanation 1

画面に表示される数字は、$ 0\ \rightarrow\ 9\ \rightarrow\ 8\ \rightarrow\ 7 $ と変化します。

### Sample Explanation 2

画面に表示される数字は、$ 0\ \rightarrow\ 4\ \rightarrow\ 0\ \rightarrow\ 4 $ と変化します。

