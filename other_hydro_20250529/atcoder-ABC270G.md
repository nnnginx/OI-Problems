## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc270/tasks/abc270_g

次の漸化式で定められる数列 $ X=(X_0,X_1,\ldots) $ があります。

$ X_i\ =\ \left\{
\begin{array}{ll}
S\  \ (i\ =\ 0)\\
(A\ X_{i-1}+B)\ \bmod\ P\  \ (i\ \geq\ 1)
\end{array}
\right. $

$ X_i=G $ となる $ i $ が存在するか判定し、存在するならばそのような最小の $ i $ を求めてください。  
ここで、$ x\ \bmod\ y $ は、$ x $ を $ y $ で割ったあまり(最小非負剰余)を表すものとします。

$ 1 $ ファイルにつき $ T $ 個のテストケースが与えられます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ T $ $ \mathrm{case}_1 $ $ \mathrm{case}_2 $ $ \vdots $ $ \mathrm{case}_T $

各テストケースは以下の形式で与えられる。

> $ P $ $ A $ $ B $ $ S $ $ G $

## 输出格式
$ T $ 行出力せよ。  
$ t $ 行目には、$ \mathrm{case}_t $ について、$ X_i=G $ となる最小の $ i $ を出力せよ。そのような $ i $ が存在しないならかわりに `-1` を出力せよ。

## 题目大意
对于某个无穷序列 $\{X\}$，构造如下：

$$
X_i =
\begin{cases}
S      & i=0 \\
(A\times X_{i-1}+B)\bmod P & i \geq 1
\end{cases}
$$

求最小的 $i$ 满足 $X_i=G$，没有输出 `-1`。

多组数据，记 $T$ 为数据组数，则有 $1\le T\le100$。

保证 $P$ 是质数，$2\le P\le10^9$。

保证 $0\le A,B,S,G< P$。

```input1
3
5 2 1 1 0
5 2 2 3 0
11 1 1 0 10
```

```output1
3
-1
10
```

## 提示
### 制約

- $ 1\ \leq\ T\ \leq\ 100 $
- $ 2\ \leq\ P\ \leq\ 10^9 $
- $ P $ は素数
- $ 0\leq\ A,B,S,G\ <\ P $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

$ 1 $ 番目のケースについて、$ X=(1,3,2,0,\ldots) $ であることから、$ X_i=0 $ となる最小の $ i $ は $ 3 $ です。 $ 2 $ 番目のケースについて、$ X=(3,3,3,3,\ldots) $ であることから、$ X_i=0 $ となる $ i $ は存在しません。

