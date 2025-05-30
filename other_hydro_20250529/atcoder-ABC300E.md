## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc300/tasks/abc300_e

あなたは $ 1 $ 以上 $ 6 $ 以下の整数が等確率で出るサイコロと整数 $ 1 $ を持っています。  
 あなたは持っている整数が $ N $ 未満である間、次の操作を繰り返します。

- サイコロを振り、出た目を $ x $ とする。持っている整数に $ x $ を掛ける。
 
全ての操作を終了した時に、持っている整数が $ N $ に一致する確率を $ \text{mod\ }998244353 $ で求めてください。

   確率 $ \text{mod\ }998244353 $ とは？ 求める確率は必ず有理数となることが証明できます。 またこの問題の制約下では、その値を互いに素な $ 2 $ つの整数 $ P $, $ Q $ を用いて $ \frac{P}{Q} $ と表したとき、$ R\ \times\ Q\ \equiv\ P\pmod{998244353} $ かつ $ 0\ \leq\ R\ \lt\ 998244353 $ を満たす整数 $ R $ がただ一つ存在することが証明できます。この $ R $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
全ての操作を終了した時に、持っている整数が $ N $ に一致する確率を $ \text{mod\ }998244353 $ で出力せよ。

## 题目大意
你有一个整数 $1$ 和一个等概率显示 $1$ 到 $6$ 的整数的骰子。当你的整数严格小于 $N$ 时，你重复下面的操作： 

+ 投这个骰子。如果它显示的是 $x$，就用你的整数乘以 $x$。

找出你的整数最后是 $N$ 的概率，模 $998244353$。

```input1
6
```

```output1
239578645
```

```input2
7
```

```output2
0
```

```input3
300
```

```output3
183676961
```

```input4
979552051200000000
```

```output4
812376310
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^{18} $
- $ N $ は整数
 
### Sample Explanation 1

操作が終了するまでの手順としてあり得る一例を挙げると次のようになります。 - はじめ, 持っている整数は $ 1 $ である。 - サイコロを振り, $ 2 $ が出る。持っている整数は $ 1\ \times\ 2\ =\ 2 $ になる。 - サイコロを振り, $ 4 $ が出る。持っている整数は $ 2\ \times\ 4\ =\ 8 $ になる。 - 持っている整数が $ 6 $ 以上になったので操作を終了する。 操作がこのように進んだ場合、操作後に持っている整数は $ 8 $ であり $ N\ =\ 6 $ に一致しません。 操作後に持っている整数が $ 6 $ である確率は $ \frac{7}{25} $ です。 $ 239578645\ \times\ 25\ \equiv\ 7\ \pmod{998244353} $ より、 $ 239578645 $ を出力してください。

### Sample Explanation 2

どのような目が出ても、操作後に持っている整数が $ 7 $ になることはありません。

