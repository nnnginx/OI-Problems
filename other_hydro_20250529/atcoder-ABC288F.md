## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc288/tasks/abc288_f

$ 10 $ 進表記で $ N $ 桁の正整数 $ X $ が与えられます。$ X $ の各桁は $ 0 $ ではありません。  
$ \lbrace\ 1,2,\ \ldots,\ N-1\ \rbrace $ の部分集合 $ S $ に対し、$ f(S) $ を以下のように定義します。

> $ X $ を $ 10 $ 進表記したものを長さ $ N $ の文字列とみなし、$ i\ \in\ S $ のとき、またそのときに限り文字列の $ i $ 文字目と $ i\ +\ 1 $ 文字目に区切りを入れることで $ |S|\ +\ 1 $ 個の文字列に分解する。  
> このようにして得られた $ |S|+1 $ 個の文字列を $ 10 $ 進表記された整数とみなし、$ f(S) $ をこれら $ |S|+1 $ 個の整数の積で定める。

$ S $ としてあり得るものは空集合を含めて $ 2^{N-1} $ 通りありますが、これら全てに対する $ f(S) $ の総和を $ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $

## 输出格式
答えを出力せよ。

## 题目大意
给定一个 $n$ 位数 $X$，把 $X$ 分成若干段，得分为每一段的乘积（可以不分割，得分为 $X$）。求所有分法得分之和，取模 $998244353$。

Translate by [xionglangqi](https://www.luogu.com.cn/user/555345)

```input1
3
234
```

```output1
418
```

```input2
4
5915
```

```output2
17800
```

```input3
9
998244353
```

```output3
258280134
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ X $ は $ 10 $ 進表記で $ N $ 桁で、各桁は $ 0 $ でない
- 入力はすべて整数

### Sample Explanation 1

$ S\ =\ \emptyset $ とすると、$ f(S)\ =\ 234 $ です。 $ S\ =\ \lbrace\ 1\ \rbrace $ とすると、$ f(S)\ =\ 2\ \times\ 34\ =\ 68 $ です。 $ S\ =\ \lbrace\ 2\ \rbrace $ とすると、$ f(S)\ =\ 23\ \times\ 4\ =\ 92 $ です。 $ S\ =\ \lbrace\ 1,\ 2\ \rbrace $ とすると、$ f(S)\ =\ 2\ \times\ 3\ \times\ 4\ =\ 24 $ です。 $ 234\ +\ 68\ +\ 92\ +\ 24\ =\ 418 $ であるため、$ 418 $ を出力します。

