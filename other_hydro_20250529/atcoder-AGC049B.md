## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc049/tasks/agc049_b

`0` と `1` からなる長さ $ N $ の文字列 $ S $ 及び $ T $ が与えられます． あなたは，$ S $ に以下の操作を好きな回数行うことができます．

- $ S_i= $`1` となる $ i $ ($ 2\ \leq\ i\ \leq\ N $) を選ぶ． そして，$ S_i $ を `0` で置き換える． さらに，$ S_{i-1} $ を今と異なる文字へ変更する．つまり，操作の直前で $ S_{i-1} $ が `0` であれば `1` に，`1` であれば `0` に変更する．

$ S $ を $ T $ に一致させることは可能でしょうか？ また可能な場合は，そのために必要な最小の操作回数はいくらでしょうか？

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $ $ T $

## 输出格式
$ S $ を $ T $ に一致させることが可能な場合，必要な最小の操作回数を出力せよ． 不可能な場合，$ -1 $ を出力せよ．

## 题目大意
一个 $N$ 长度的 `01` 串 $S$，你可以进行若干次如下操作：

选一个不在首位的 $1$ 位，反转这一位和前一位。

如果可能将 $S$ 变 $T$，输出 `-1` 或最小次数。

```input1
3
001
100
```

```output1
2
```

```input2
3
001
110
```

```output2
-1
```

```input3
5
10111
01010
```

```output3
5
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 5\ \times\ 10^5 $
- $ S $ は `0`,`1` からなる長さ $ N $ の文字列．
- $ T $ は `0`,`1` からなる長さ $ N $ の文字列．

### Sample Explanation 1

`001` → ($ i=3 $ で操作) → `010` → ($ i=2 $ で操作) → `100` とすればよいです．

