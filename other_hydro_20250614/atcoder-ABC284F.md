## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc284/tasks/abc284_f

長さ $ N $ の文字列 $ S $ および整数 $ i\ (0\leq\ i\leq\ N) $ に対して、$ f_i(S) $ を、

- $ S $ の先頭 $ i $ 文字
- $ S $ を反転した文字列
- $ S $ の末尾 $ N-i $ 文字

をこの順に連結した文字列と定義します。 例えば、$ S= $ `abc`、$ i=2 $ のとき、$ f_i(S)= $ `abcbac` です。

長さ $ 2N $ の文字列 $ T $ が与えられます。 $ f_i(S)=T $ を満たす長さ $ N $ の文字列 $ S $ と整数 $ i\ (0\leq\ i\leq\ N) $ の組を $ 1 $ つ見つけてください。 そのような $ S,i $ の組が存在しない場合は、それを報告してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ T $

## 输出格式
条件を満たす $ S,i $ の組が存在しないならば、`-1` と出力せよ。 存在するならば、$ S,i $ を改行区切りで出力せよ。 条件を満たす $ S,i $ の組が複数存在する場合は、そのどれを出力しても良い。

## 题目大意
对于一个长度为 $N$ 的字符串 $S$ 和一个整数 $i\in [0,N]$，定义 $f_i(S)$ 所得的字符串为以下三者顺次连接：

- $S$ 的前 $i$ 个字符；
- 将 $S$ 翻转得到的字符串；
- $S$ 的后 $N-i$ 个字符。

例如，对于 $S=\texttt{abc}$，$i=2$ 有 $f_i(S)=\texttt{abcbac}$。

现在有一个长度为 $2N$ 的字符串 $T$，你需要求出任意一对 $(S,i)$ 满足 $f_i(S)=T$。如果不存在，输出 $-1$。

翻译 by @Mars\_Dingdang

```input1
3
abcbac
```

```output1
abc
2
```

```input2
4
abababab
```

```output2
abab
1
```

```input3
3
agccga
```

```output3
cga
0
```

```input4
4
atcodeer
```

```output4
-1
```

## 提示
### 制約

- $ 1\leq\ N\ \leq\ 10^6 $
- $ N $ は整数
- $ T $ は英小文字からなる長さ $ 2N $ の文字列

### Sample Explanation 1

問題文中に書いた通り、$ S= $ `abc`、$ i=2 $ とすると $ f_i(S)= $ `abcbac` となって $ T $ に一致するため、`abc` と $ 2 $ を出力します。

### Sample Explanation 2

$ S= $ `abab`、$ i=3 $ としても条件を満たします。

### Sample Explanation 3

$ S= $ `agc`、$ i=3 $ としても条件を満たします。

### Sample Explanation 4

条件を満たす $ S,i $ の組が存在しない場合は `-1` を出力してください。

