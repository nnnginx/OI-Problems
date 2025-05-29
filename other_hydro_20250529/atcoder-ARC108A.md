## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc108/tasks/arc108_a

整数 $ S,P $ が与えられます。 $ N+M=S,N\ \times\ M\ =P $ を満たすような正の整数の組 $ (N,M) $ はありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ P $

## 输出格式
$ N+M=S,N\ \times\ M\ =P $ を満たすような正の整数の組 $ (N,M) $ があるなら `Yes`、そうでないなら `No` を出力せよ。

## 题目大意
给定两个整数 $s, p$，求是否存在整数 $(n, m)$ 使得 $n + m = s$ 且 $n * m = p$。
如果存在，输出 $Yes$，否则输出 $No$。

```input1
3 2
```

```output1
Yes
```

```input2
1000000000000 1
```

```output2
No
```

## 提示
### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ S,P\ \leq\ 10^{12} $

### Sample Explanation 1

\- 例えば $ N=1,M=2 $ のとき、$ N+M=3,N\ \times\ M\ =2 $ となります。

### Sample Explanation 2

\- そのような $ (N,M) $ は存在しません。

