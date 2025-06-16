## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc148/tasks/abc148_b

英小文字のみからなる長さ $ N $ の文字列 $ S $, $ T $ が与えられます。

$ S $ の $ 1 $ 文字目、$ T $ の $ 1 $ 文字目、$ S $ の $ 2 $ 文字目、$ T $ の$ 2 $ 文字目、$ S $ の $ 3 $ 文字目、...、$ S $ の$ N $ 文字目、$ T $ の$ N $ 文字目というように、 $ S $ の各文字と $ T $ の各文字を先頭から順に交互に文字を並べ、新しい文字列を作ります。この新しくできた文字列を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ T $

## 输出格式
新しくできた文字列を出力せよ。

## 题目大意
给你长度为 $n(n\le 100)$ 的 $2$ 个字符串 $S,T$ 。

请你按照 $S_1,T_1,S_2,T_2,...,S_n,T_n$ 的顺序输出。

```input1
2
ip cc
```

```output1
icpc
```

```input2
8
hmhmnknk uuuuuuuu
```

```output2
humuhumunukunuku
```

```input3
5
aaaaa aaaaa
```

```output3
aaaaaaaaaa
```

## 提示
### 制約

- $ 1\ <\ =\ N\ <\ =\ 100 $
- $ |S|\ =\ |T|\ =\ N $
- $ S $, $ T $ は英小文字のみからなる文字列

