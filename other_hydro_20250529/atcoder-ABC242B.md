## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc242/tasks/abc242_b

文字列 $ S $ が与えられます。$ S $ の各文字を並び替えて得られる文字列 $ S' $ のうち、辞書順で最小のものを出力してください。

なお、相異なる $ 2 $ つの文字列 $ s\ =\ s_1\ s_2\ \ldots\ s_n $ と $ t\ =\ t_1\ t_2\ \ldots\ t_m $ について、それらが以下の条件のいずれかを満たすとき、辞書順で $ s\ \lt\ t $ であるとします。

- ある整数 $ i\ (1\ \leq\ i\ \leq\ \min(n,m)) $ が存在し、$ s_i\ \lt\ t_i $ かつすべての整数 $ j\ (1\ \leq\ j\ \lt\ i) $ について $ s_j=t_j $
- すべての整数 $ i\ (1\ \leq\ i\ \leq\ \min(n,m)) $ について $ s_i\ =\ t_i $ かつ、$ n\ \lt\ m $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ の各文字を並び替えて得られる文字列 $ S' $ のうち、辞書順で最小のものを出力せよ。

## 题目大意
最开始你拥有一个字符串 $S$。

对 $S$ 的所有字符进行排列得到一个字符串 $S'$。请输出所有 $S'$ 中字典序最小的。

关于字典序：

两个字符串 $S=s_1,s_2,s_3……s_n$ 和 $T=t_1,t_2,t_3……t_m$，$S$ 的字典序小于 $T$ 当且仅当：

$s_1=t_1,s_2=t_2,s_3=t_3……s_{k-1}=t_{k-1},s_k<t_k$

或

$s_1=t_1,s_2=t_2,s_3=t_3……s_{n-1}=t_{n-1},s_n=t_n$且$n<m$

```input1
aba
```

```output1
aab
```

```input2
zzzz
```

```output2
zzzz
```

## 提示
### 制約

- $ S $ は英小文字のみからなる長さ $ 1 $ 以上 $ 2\ \times\ 10^5 $ 以下の文字列

### Sample Explanation 1

$ S= $ `aba` を並び替えて得られる文字列は以下の $ 3 $ つが考えられます。 - `aba` - `aab` - `baa` この中で辞書順で最小のものは、`aab` です。

