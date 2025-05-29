## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc293/tasks/abc293_a

英小文字からなる長さが偶数の文字列 $ S $ が与えられます。$ S $ の長さを $ |S| $、$ S $ の $ i $ 文字目を $ S_i $ で表します。

$ i\ =\ 1,\ 2,\ \ldots,\ \frac{|S|}{2} $ の順に以下の操作を行い、すべての操作を終えた後の $ S $ を出力してください。

- $ S_{2i-1} $ と $ S_{2i} $ を入れ替える

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを出力せよ。

## 题目大意
给定长度为偶数的字符串 $S$，请将 $S$ 奇数位置上的字符与偶数位置上的字符交换（下标从 $1$ 开始）。  
即：对于 $\forall 1\le i \le \dfrac{|S|}{2}$，交换 $S_{2i},S_{2i+1}$。  
输出交换后的 $S$。

```input1
abcdef
```

```output1
badcfe
```

```input2
aaaa
```

```output2
aaaa
```

```input3
atcoderbeginnercontest
```

```output3
taocedbrgeniencrnoetts
```

## 提示
### 制約

- $ S $ は英小文字からなる長さが偶数の文字列
- $ S $ の長さは $ 100 $ 以下

### Sample Explanation 1

操作を行う前は $ S\ = $ `abcdef` です。 $ i\ =\ 1 $ について操作を行うと、$ S_1 $ と $ S_2 $ が入れ替わるので $ S\ = $ `bacdef` になります。 $ i\ =\ 2 $ について操作を行うと、$ S_3 $ と $ S_4 $ が入れ替わるので $ S\ = $ `badcef` になります。 $ i\ =\ 3 $ について操作を行うと、$ S_5 $ と $ S_6 $ が入れ替わるので $ S\ = $ `badcfe` になります。 したがって、`badcfe` を出力します。

