## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc130/tasks/arc130_a

長さ $ N $ の文字列 $ S $ が与えられます。 $ 1\leq\ i\leq\ N $ に対して、$ S $ からその $ i $ 文字目を削除してできる文字列を $ S_i $ と表します。

整数の組 $ (i,j) $ であって、次の条件をともに満たすものの個数を求めてください。

- $ 1\leq\ i\ <\ j\leq\ N $
- $ S_i\ =\ S_j $

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $ $ S $

## 输出格式
答えを出力してください。

## 题目大意
给定长度为$N$的字符串$S$。$1\leq\ i\leq\N$，$S_i表示为i$。

整数组$（i，j）$，请计算满足以下条件的个数：

- $ 1\leq\ i\ <\ j\leq\ N $
- $ S_i\ =\ S_j $

```input1
7
abbbcca
```

```output1
4
```

```input2
4
xxxx
```

```output2
6
```

```input3
2
pp
```

```output3
1
```

```input4
2
st
```

```output4
0
```

## 提示
### 制約

- $ 2\leq\ N\leq\ 3\times\ 10^5 $
- $ S $ は英小文字からなる長さ $ N $ の文字列である

### Sample Explanation 1

$ S_i $ は、順に以下の文字列となります：`bbbcca`, `abbcca`, `abbcca`, `abbcca`, `abbbca`, `abbbca`, `abbbcc` 条件を満たす $ (i,j) $ は以下の $ 4 $ 個です。 - $ (i,j)\ =\ (2,3) $ - $ (i,j)\ =\ (2,4) $ - $ (i,j)\ =\ (3,4) $ - $ (i,j)\ =\ (5,6) $

