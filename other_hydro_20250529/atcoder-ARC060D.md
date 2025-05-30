## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc060/tasks/arc060_d

$ x $ を長さ $ 1 $ 以上の文字列とします。 いかなる文字列 $ y $ および $ 2 $ 以上の整数 $ k $ に対しても、 $ y $ を $ k $ 回繰り返した文字列が $ x $ と異なるならば、 $ x $ を*良い文字列*であると呼ぶことにします。 例えば、`a`, `bbc`, `cdcdc` などは良い文字列ですが、 `aa`, `bbbb`, `cdcdcd` などは良い文字列ではありません。

$ w $ を長さ $ 1 $ 以上の文字列とします。 $ m $ 項からなる列 $ F=(\,f_1,\,f_2,\,...,\,f_m) $ について、 次の条件がともに満たされるならば、$ F $ を $ w $ の*良い表現*と呼ぶことにします。

- すべての $ i\ \,\ (1\ \leq\ i\ \leq\ m) $ について、$ f_i $ は良い文字列である。
- $ f_1,\,f_2,\,...,\,f_m $ をこの順に連結すると $ w $ になる。

例えば、$ w= $`aabb` の場合、$ w $ の良い表現は次の $ 5 $ つとなります。

- $ ( $`aabb`$ ) $
- $ ( $`a`$ , $`abb`$ ) $
- $ ( $`aab`$ , $`b`$ ) $
- $ ( $`a`$ , $`ab`$ , $`b`$ ) $
- $ ( $`a`$ , $`a`$ , $`b`$ , $`b`$ ) $

文字列 $ w $ の良い表現のうち、項数 $ m $ が最小であるものを、 $ w $ の*最良表現*と呼ぶことにします。 例えば、$ w= $`aabb` の最良表現は $ ( $`aabb`$ ) $ の $ 1 $ つのみとなります。

文字列 $ w $ が与えられます。次の $ 2 $ つを求めてください。

- $ w $ の最良表現の項数
- $ w $ の最良表現の総数を $ 1000000007\ \,\ (=10^9+7) $ で割った余り

なお、$ w $ に対し、良い表現が存在することは保証されます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ w $

## 输出格式
出力は $ 2 $ 行からなる。

- $ 1 $ 行目に、$ w $ の最良表現の項数を出力せよ。
- $ 2 $ 行目に、$ w $ の最良表現の総数を $ 1000000007 $ で割った余りを出力せよ。

## 题目大意
设$x$是一个长度至少为1的字符串，我们称$x$是好的，当且仅当对于任意字符串$y$和任意整数$k(k≥2)$，由$y$复制$k$次并连接得到的字符串均与$x$不同。 举个例子，`a`，`bbc`和`cdcdc`是好串，然而`aa`，`bbbb`和`cdcdcd`不是。

设$w$是一个长度至少为1的字符串，对于一个由$m$个元素组成的序列 $F=(f_1,f_2,...,f_m)$，我们称$F$为$w$的一个“亮眼表现”当且仅当下面的条件同时被满足：
* 对于任意$i(1≤i≤m)$，元素$f_i$是一个好串。
* 把$f_1,f_2,...,f_m$按顺序连接起来得到的字符串就是$w$。

举个例子，当$w$='`aabb`'时，$w$有五个亮眼表现：

* (`aabb`)
* (`a`,`abb`)
* (`aab`,`b`)
* (`a`,`ab`,`b`)
* (`a`,`a`,`b`,`b`)

在$w$的所有亮眼表现中，元素数量最少的那个（些）亮眼表现被称为$w$的“全场最佳”。举个例子，当$w$='`aabb`'时，$w$的全场最佳只有一个：(`aabb`)。

给你一个字符串$w$，请计算：

* $w$的一个全场最佳所含的元素数量
* $w$有多少个全场最佳（对1e9+7取模）

(数据保证$w$一定存在亮眼表现)

```input1
aab
```

```output1
1
1
```

```input2
bcbc
```

```output2
2
3
```

```input3
ddd
```

```output3
3
1
```

## 提示
### 制約

- $ 1\ \leq\ |w|\ \leq\ 500000\ \,\ (=5\ \times\ 10^5) $
- $ w $ は英小文字 (`a`-`z`) のみからなる文字列である

### 部分点

- $ 1\ \leq\ |w|\ \leq\ 4000 $ を満たすデータセットに正解した場合は、$ 400 $ 点が与えられる。

### Sample Explanation 2

\- この入力に対しては、項数が $ 2 $ の最良表現が以下の $ 3 $ 通り存在します。 - $ ( $`b`$ , $`cbc`$ ) $ - $ ( $`bc`$ , $`bc`$ ) $ - $ ( $`bcb`$ , $`c`$ ) $

