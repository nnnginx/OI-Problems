## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc036/tasks/agc036_e

`A`,`B`,`C` からなる文字列 $ S $ が与えられます。

$ S $ の連続とは限らない部分列 $ x $ であって、次の条件をすべて満たすもののうち、最長のものを $ 1 $ つ求めてください。 なお、$ S $ の部分列とは、$ S $ から $ 0 $ 個以上の文字を削除して得られる文字列を意味します。

- $ x $ に含まれる `A`,`B`,`C` それぞれの個数は全て等しい。
- $ x $ の中で同じ文字は隣り合わない。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
条件を満たす最長の部分列を $ 1 $ つ出力せよ。 解が複数ある場合は、どれを出力しても正解とみなされる。

## 题目大意
给你一个长度为 $n$ 的仅包含ABC三种字母的字符串 $s$ ，现在要你输出一个满足下列要求的最长的 $s$ 的子序列:

+ ABC三种字符的出现次数相同。
+ 子序列中相邻两个字符不能相同。

如果有多组解，输出任意一组即可。

数据范围：$|s|\leq 10^6$。

```input1
ABBCBCAB
```

```output1
ACBCAB
```

```input2
ABABABABACACACAC
```

```output2
BABCAC
```

```input3
ABCABACBCBABABACBCBCBCBCBCAB
```

```output3
ACABACABABACBCBCBCBCA
```

```input4
AAA
```

```output4

```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^6 $
- $ S $ は `A`,`B`,`C` からなる。

### Sample Explanation 1

$ S $ の部分列として、`ACBCAB` を考えると、これは条件を満たしており、またこれが最長です。 また、`ABCBCA` も条件を満たす最長の部分列です。 `ABCBCAB`, `ABBCCA` なども $ S $ の部分列ですが、これらは条件を満たしません。

### Sample Explanation 4

条件を満たす部分列が空文字列のみのこともあります。

