## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc108/tasks/arc108_e

$ N $ 脚のイスが左から右に並んでいます。 左から $ i $ 番目のイスのIDは $ a_i $ です。ここで、$ a_i $ がすべて相異なることが保証されます。

すぬけ君は何脚かのイスに印をつけ、印をつけたイス以外を捨てることにしました。はじめ、どのイスにも印はついていません。 印のついたイスたちのIDが左から右に単調増加になっているような印のつけ方を *よい印のつけ方* と呼びます。

すぬけ君は以下の手続きに従って印をつけることにしました。

1. イス $ x $ に新たに印をつけても印のつけ方がよい印のつけ方のままであるとき、イス $ x $ を *良いイス* とする。現在の良いイスの脚数を $ k $ とする
2. $ k=0 $ なら印のついていないイスを取り除き手続きを終了する。そうでないなら、$ k $ 脚の良いイスから等確率で $ 1 $ つを選んで印をつけ手順 1 へ戻る

手続き終了時に残るイスの脚数の期待値が有理数になることが証明できます。その値を $ P/Q $ (既約分数)とします。また $ M=10^{9}+7 $ とします。このとき、$ 0 $ 以上 $ M-1 $ 以下の整数 $ R $ がただ一つ存在して $ P\ \equiv\ Q\ \times\ R\ \pmod{M} $ となることが証明でき、その値は $ P\ \times\ Q^{-1}\ \pmod{M} $ と等しくなります。ここで、$ Q^{-1} $ はモジュラ逆数です。$ R $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ \cdots $ $ a_N $

## 输出格式
$ R $ を出力せよ。

## 题目大意
从左到右排列了 $N$ 张椅子，第 $i$ 张的编号为 $a_i$ （保证 $a_i$ 互不相同）。

$\texttt{Snuke}$ 想要标记一些椅子并把剩下的丢掉，一开始所有椅子都没有被标记。我们称一种标记方案是好的，当且仅当其标号递增。即，若标记的编号为 $i_1<i_2<\cdots<i_k$，则有 $a_{i_1}<a_{i_2}<\cdots<a_{i_k}$。

$\texttt{Snuke}$ 将重复一下操作来标记椅子：

1. 称 $x$ 是不错的当且仅当把 $x$ 加入后标记方案仍是好的，记其数量为 $k$；

2. 若 $k=0$ 结束操作，否则均匀随机选择一个标记并继续操作 $1$；

求最终标记个数的期望。

```input1
3
3 1 2
```

```output1
666666673
```

```input2
30
26 16 28 30 23 11 29 18 22 15 20 13 27 9 21 7 5 25 4 19 8 3 1 24 10 14 17 12 2 6
```

```output2
297703424
```

## 提示
### 制約

- 与えられる入力は全て整数
- $ 1\ \leq\ N\ \leq\ 2000 $
- $ 1\ \leq\ a_i\ \leq\ N $
- $ a_i $ はすべて相異なる

### Sample Explanation 1

\- はじめにイス $ 1 $(IDが $ 1 $ のイスです) に印がついたとき、最終的に残るイスはイス $ 1,2 $ の $ 2 $ 脚です。 - はじめにイス $ 2 $ に印がついたとき、最終的に残るイスはイス $ 1,2 $ の $ 2 $ 脚です。 - はじめにイス $ 3 $ に印がついたとき、最終的に残るイスはイス $ 3 $ の $ 1 $ 脚です。 - イスは等確率で選ばれるので手続き終了時に残るイスの脚数の期待値は $ \frac{5}{3} $ となります。$ 5\ \equiv\ 3\ \times\ 666666673\ \pmod{M} $ より、$ R=666666673 $ です。

