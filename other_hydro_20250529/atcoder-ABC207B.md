## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc207/tasks/abc207_b

水色のボールが $ A $ 個容器に入っています。高橋くんはこの容器に対し、以下の操作を $ 0 $ 回以上好きなだけ繰り返します。

- 水色のボール $ B $ 個と赤色のボール $ C $ 個を容器に追加する。

高橋くんの目標は、容器に入っている水色のボールの個数が赤色のボールの個数の $ D $ 倍以下になるようにすることです。

目標が達成可能かを判定し、可能なら必要な操作回数の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $

## 输出格式
高橋くんの目標が達成可能なら、操作回数の最小値を出力せよ。そうでなければ、`-1` を出力せよ。

## 题目大意
有两个数 $m$ 和 $n$ 。 $m$ 的初始值由输入的第一个数给出， $n$ 的初始值为 $0$ 。每次将 $m$ 加上 $a$ ，将 $n$ 加上 $b$ ，求 $m$ 在经过多少次操作后能使 $m≤cn$ 。如果目标无法实现，请输出 $-1$ 。输入：一行四个整数 $m,a,b,c$ ；输出：目标可以实现输出题目答案，否则输出 $-1$ 。

```input1
5 2 3 2
```

```output1
2
```

```input2
6 9 2 3
```

```output2
-1
```

## 提示
### 制約

- $ 1\ \leq\ A,B,C,D\ \leq\ 10^5 $
- 入力は全て整数である。

### Sample Explanation 1

$ 0 $ 回目の操作を行った直後の $ (= $ $ 1 $ 度も操作をしていない状態での$ ) $ 容器には、水色のボールが $ 5 $ 個と赤色のボールが $ 0 $ 個入っています。水色のボールの個数は赤色のボールの個数の $ D=2 $ 倍よりも大きいので、この時点ではまだ高橋くんの目標は達成されていません。 $ 1 $ 回目の操作を行った直後の容器には、水色のボールが $ 7 $ 個と赤色のボールが $ 3 $ 個入っています。水色のボールの個数は赤色のボールの個数の $ 2 $ 倍よりも大きいので、この時点でもまだ高橋くんの目標は達成されていません。 $ 2 $ 回目の操作を行った直後の容器には、水色のボールが $ 9 $ 個と赤色のボールが $ 6 $ 個入っています。水色のボールの個数は赤色のボールの個数の $ 2 $ 倍以下であるため、高橋くんの目標は達成されています。 よって答えは $ 2 $ となります。

### Sample Explanation 2

高橋くんが何回操作を繰り返しても、彼の目標が達成されることはありません。

