## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc283/tasks/abc283_f

$ (1,2,\ldots,N) $ の順列 $ P=(P\ _\ 1,P\ _\ 2,\ldots,P\ _\ N) $ が与えられます。

すべての $ i\ (1\leq\ i\leq\ N) $ に対して、以下の値を求めてください。

- $ D\ _\ i=\displaystyle\min_{j\neq\ i}\left\lparen\left\lvert\ P\ _\ i-P\ _\ j\right\rvert+\left\lvert\ i-j\right\rvert\right\rparen $
 
 順列とは $ (1,2,\ldots,N) $ の順列とは、$ (1,2,\ldots,N) $ を並べ替えて得られる数列のことをいいます。 つまり、長さ $ N $ の数列 $ A $ は $ i\ (1\leq\ i\leq\ N) $ がその中にちょうど $ 1 $ 回だけ現れるとき、かつそのときに限り$ (1,2,\ldots,N) $ の順列です。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ P\ _\ 1 $ $ P\ _\ 2 $ $ \ldots $ $ P\ _\ N $

## 输出格式
$ D\ _\ i\ (1\leq\ i\leq\ N) $ を $ i $ の昇順に空白区切りで出力せよ。

## 题目大意
给定一个 $1 \sim n$ 的排列 $p = (p_1, p_2, \dots, p_n)$。

你需要对每个 $i$ 求得 
$$D_i = \min_{j \neq i} \left\{ \lvert p_i - p_j\rvert + \lvert i - j\rvert \right\} $$

一个 $1\sim n$ 的排列是一个长为 $n$ 的序列，满足 $[1, n]$ 内的所有整数恰好都在其中出现一次。

$2\le n \le 2\times 10^5$。

```input1
4
3 2 4 1
```

```output1
2 2 3 3
```

```input2
7
1 2 3 4 5 6 7
```

```output2
2 2 2 2 2 2 2
```

```input3
16
12 10 7 14 8 3 11 13 2 5 6 16 4 1 15 9
```

```output3
3 3 3 5 3 4 3 3 4 2 2 4 4 4 4 7
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times10^5 $
- $ 1\ \leq\ P\ _\ i\ \leq\ N\ (1\leq\ i\leq\ N) $
- $ i\neq\ j\implies\ P\ _\ i\neq\ P\ _\ j $
- 入力はすべて整数
 
### Sample Explanation 1

たとえば、$ i=1 $ について - $ j=2 $ のとき、$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=1,\left\lvert\ i-j\right\rvert=1 $ です。 - $ j=3 $ のとき、$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=1,\left\lvert\ i-j\right\rvert=2 $ です。 - $ j=4 $ のとき、$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=2,\left\lvert\ i-j\right\rvert=3 $ です。 よって、$ j=2 $ のとき $ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert+\left\lvert\ i-j\right\rvert=2 $ で最小となるので、$ D\ _\ 1=2 $ です。

