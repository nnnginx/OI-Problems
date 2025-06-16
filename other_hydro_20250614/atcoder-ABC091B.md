## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc091/tasks/abc091_b

高橋君は青いカードを $ N $ 枚，赤いカードを $ M $ 枚持っています。 カードにはそれぞれ文字列が書かれており， $ i $ 枚目の青いカードに書かれている文字列は $ s_i $， $ i $ 枚目の赤いカードに書かれている文字列は $ t_i $ です。

高橋君は，文字列を $ 1 $ つ言います。 そして，全てのカードを確認し， その文字列が書かれた青いカードを $ 1 $ 枚見つけるごとに $ 1 $ 円貰えます。 また，その文字列が書かれた赤いカードを $ 1 $ 枚見つけるごとに $ 1 $ 円失います。

なお，高橋君の言った文字列と，カードに書かれた文字列が完全に一致していた場合のみを考えます。 例えば，高橋君が `atcoder` と言った場合，`atcoderr`，`atcode`，`btcoder` などと書かれた青いカードがあってもお金は貰えません(逆に，このような文字列が書かれた赤いカードがあってもお金を失うことはありません)。

高橋君は，最大で差し引き何円貰うことができるでしょうか？

ただし，違うカードに同じ文字列が書かれていることもあることに注意してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ s_1 $ $ s_2 $ $ : $ $ s_N $ $ M $ $ t_1 $ $ t_2 $ $ : $ $ t_M $

## 输出格式
高橋君が最大で差し引き $ X $ 円貰える時，$ X $ を出力せよ。

## 题目大意
### 题目描述
有两组字符串，一组蓝色，一组红色，各有n、m个字符串。你可以随便说一个字符串：

如果你在蓝色的字符串组中找到了这个字符串，就加一分；如果在红色的字符串组中找到了，就扣一分。

现在让你输出得分的最大值，且只有得分非负时才输出。

### 输入格式

输入n，接下来n行输入字符串(s[i])。输入m，接下来m行输入字符串(t[i])

### 输出格式

输出得分的最大值。


```input1
3
apple
orange
apple
1
grape
```

```output1
2
```

```input2
3
apple
orange
apple
5
apple
apple
apple
apple
apple
```

```output2
1
```

```input3
1
voldemort
10
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
voldemort
```

```output3
0
```

```input4
6
red
red
blue
yellow
yellow
red
5
red
red
yellow
green
blue
```

```output4
1
```

## 提示
### 制約

- $ N,\ M $ は整数
- $ 1\ \leq\ N,\ M\ \leq\ 100 $
- $ s_1,\ s_2,\ ...,\ s_N,\ t_1,\ t_2,\ ...,\ t_M $ は全て長さ $ 1 $ 以上 $ 10 $ 以下の文字列で，英小文字のみからなる

### Sample Explanation 1

`apple` と言えば，$ 2 $ 円貰うことができます。

### Sample Explanation 2

`apple` と言うと，$ 3 $ 円失ってしまいます。`orange` と言えば，$ 1 $ 円貰うことができます。

### Sample Explanation 3

`voldemort` と言うと，$ 9 $ 円失ってしまいます。例えば `orange` と言えば，$ 1 $ 円も失わずにすみます。

