## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc152/tasks/arc152_c

$ N $ 項からなる数列 $ a_1,a_2,\ldots,a_N $ があります。 あなたはこれから、この数列に以下の操作を好きな回数行うことができます。（$ 1 $ 回も行わなくてもよいです。）

- その時点の数列から項を $ 1 $ つ選び、その値を $ s $ とする。 次に、全ての $ 1\leq\ i\leq\ N $ に対して、$ a_i $ を $ 2s-a_i $ で置き換える。 ただし、この操作によって、数列に負の値を持つ項が生じてはならない。
 
あなたは、数列の項の最大値をできるだけ小さくしたいと考えています。 適切に操作を行った場合の、数列の項の最大値はいくつになるでしょうか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ \ldots $ $ a_N $

## 输出格式
答えを整数で出力せよ。

## 题目大意
给你一个 $n$ 项的数列，你可以对其做任意次如下的操作（也可以不做）：

选择序列里面的一项，令其值为 $s$，对于每一个数列里面的每一项 $a_i$，将 $a_i$ 替换为 $2s -a_i$。操作完的序列必须是非负整数

希望让这个序列的最大值最小化，求最优的操作后的序列中最大值。

Translation by Ziqqurat.

```input1
3
1 3 6
```

```output1
5
```

```input2
5
400 500 600 700 800
```

```output2
400
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ a_1\ <\ a_2\ <\ \ldots\ <\ a_N\ \leq\ 10^9 $
- 入力される値はすべて整数である
 
### Sample Explanation 1

$ s=3 $ として操作を行うと、数列は $ (5,3,0) $ になります。このとき最大値は $ 5 $ です。 数列に負の項が生じてはいけないという条件の下で、これ以上数列の項の最大値を小さくすることはできませんので、$ 5 $ と答えてください。

### Sample Explanation 2

$ s=400 $ として操作を一度行うほか、$ s=500 $ として操作を行った後、$ s=300 $ としてもう一度操作を行うなどの方法が考えられます。

