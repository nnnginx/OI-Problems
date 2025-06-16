## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc254/tasks/abc254_c

長さ $ N $ の数列 $ A=(a_1,\ldots,a_N) $ があります。また、整数 $ K $ が与えられます。

あなたは次の操作を $ 0 $ 回以上何度でも行えます。

- $ 1\ \leq\ i\ \leq\ N-K $ を満たす整数 $ i $ を選び、$ a_i $ と $ a_{i+K} $ の値を入れ替える。

$ A $ を昇順に並べ替えることが出来るかどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ a_1 $ $ \ldots $ $ a_N $

## 输出格式
$ A $ を昇順に並び替えることが出来るならば `Yes` と、出来ないならば `No` と出力せよ。

## 题目大意
## 题目翻译

给出一个长为 $n$ 的数列 $a_1, a_2, \cdots, a_n$。再给一个整数 $k$。

每次可以选一个下标 $i$（$1 \le i \le n - k$），将 $a_i$ 和 $a_{i + k}$ 交换。

问能否通过交换让数列 $a$ 成为升序（任意 $a_i \le a_{i  +1}$）？

translate by @[liangbowen](https://www.luogu.com.cn/user/367488)。

## 输入格式

输入包括两行，第一行有 $2$ 个正整数 $n, k$。

第二行有 $n$ 个正整数 $a_1, a_2, \cdots, a_n$。

## 输出格式

如果可以通过交换变成升序，输出 $\texttt{Yes}$。不能变成升序，输出 $\texttt{No}$。

## 数据范围

$2 \le n \le 2 \times 10^5$；$1 \le k \le n - 1$；$1 \le a_i \le 10^9$。

```input1
5 2
3 4 1 3 4
```

```output1
Yes
```

```input2
5 3
3 4 1 3 4
```

```output2
No
```

```input3
7 5
1 2 3 4 5 5 10
```

```output3
Yes
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ K\ \leq\ N-1 $
- $ 1\ \leq\ a_i\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

次のように操作をすることで $ A $ を昇順に並び替えることが出来ます。 - $ i=1 $ とし、$ a_1 $ と $ a_3 $ の値を入れ替える。数列は $ (1,4,3,3,4) $ となる。 - $ i=2 $ とし、$ a_2 $ と $ a_4 $ の値を入れ替える。数列は $ (1,3,3,4,4) $ となる。

### Sample Explanation 3

操作を行う必要が無い場合もあります。

