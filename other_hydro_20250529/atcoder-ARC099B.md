## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc101/tasks/arc099_b

整数 $ n $ に対して，$ n $ を十進法で表したときの各桁の和を $ S(n) $ で表すことにします． たとえば，$ S(123)\ =\ 1\ +\ 2\ +\ 3\ =\ 6 $ です．

正の整数 $ n $ であって，$ m\ >\ n $ であるような任意の正の整数 $ m $ に対して $ \frac{n}{S(n)}\ \leq\ \frac{m}{S(m)} $ が成り立つようなものを， **すぬけ数** と呼ぶことにします．

整数 $ K $ が与えられたとき，すぬけ数を小さいほうから $ K $ 個列挙してください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ K $

## 输出格式
$ K $ 行出力せよ．$ i $ 行目には，$ i $ 番目に小さいすぬけ数を出力せよ．

## 题目大意
> 定义函数 $\rm S(x)$ 表示 $x$ 各个位上数字之和。求前 $k$ 个这样的 $n$：
> $$
> \forall m>n,\frac{n}{\mathrm{S}(n)}\leq \frac{m}{\mathrm{S}(m)}
> $$
> $k\geq 1$。

```input1
10
```

```output1
1
2
3
4
5
6
7
8
9
19
```

## 提示
### 制約

- $ 1\ \leq\ K $
- $ K $ 番目のすぬけ数は $ 10^{15} $ 以下

