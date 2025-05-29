## 题目描述
[problemUrl]: https://atcoder.jp/contests/code-festival-2017-qualb/tasks/code_festival_2017_qualb_f

文字列 $ S $ に対し、 $ f(S) $ を $ S $ の巡回シフトのうち辞書順最小のものとします。 たとえば、 $ S\ = $`babca` のとき、 $ S $ の巡回シフト (`babca`, `abcab`, `bcaba`, `cabab`, `ababc`) のうち最小の `ababc` が $ f(S) $ となります。

あなたは、三個の整数 $ X,\ Y $, $ Z $ が与えられます。 あなたは、 `a` をちょうど $ X $ 個、`b` をちょうど $ Y $ 個、`c` をちょうど $ Z $ 個含む文字列 $ T $ を構成したいです。 そのような文字列が複数存在する場合は、 $ f(T) $ を辞書順で最大化したいです。

$ f(T) $ の辞書順での最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ X $ $ Y $ $ Z $

## 输出格式
答えを出力せよ。

## 题目大意
定义 $f(S)$ 为：对于一个字符串 $S$，每次将它最左边的字符放置到字符串末尾生成的字符串集合中，字典序最小的字符串。例如：对于 $S$ 为 `babca` 的情况，$f(S)$ 即为 `babca`、`abcab`、`bcaba`、`cabab`、`ababc` 中最小的那个，即 `ababc`。

你需要构造一个字符串 $T$，共包含 $X$ 个字符 `a`、$Y$ 个字符 `b` 和 $Z$ 个字符 `c`，使得 $f(T)$ 尽可能大，输出这个 $f(T)$。

```input1
2 2 0
```

```output1
abab
```

```input2
1 1 1
```

```output2
acb
```

## 提示
### 制約

- $ 1\ \leq\ X\ +\ Y\ +\ Z\ \leq\ 50 $
- $ X,\ Y,\ Z $ は非負整数である。

### Sample Explanation 1

$ T $ は `a` 二個と `b` 二個からならなければなりません。 - $ T\ = $`aabb` のとき $ f(T)\ = $`aabb`. - $ T\ = $`abab` のとき $ f(T)\ = $`abab`. - $ T\ = $`abba` のとき $ f(T)\ = $`aabb`. - $ T\ = $`baab` のとき $ f(T)\ = $`aabb`. - $ T\ = $`baba` のとき $ f(T)\ = $`abab`. - $ T\ = $`bbaa` のとき $ f(T)\ = $`aabb`. となるので、 $ f(T) $ の最大値は `abab` です。

