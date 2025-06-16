## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc233/tasks/abc233_b

整数 $ L,R $ と、英小文字のみからなる文字列 $ S $ が与えられます。  
 $ S $ の $ L $ 文字目から $ R $ 文字目までの部分を反転した(すなわち、 $ L $ 文字目から $ R $ 文字目までの文字の並びを逆にした)文字列を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ L $ $ R $ $ S $

## 输出格式
問題文の指示通り出力せよ。

## 题目大意
给定一个字符串 $s$ 和一个区间 $[l,r]$，将 $s_l$ 至 $s_r$ 的字符倒转后输出。

倒装：将 $s_l$ 改变为 $s_r$，$s_{l+1}$ 改变为 $s_{r-1}$，$\cdots$，$s_r$ 改变为 $s_l$。

Translated by ShanCreeper.

```input1
3 7
abcdefgh
```

```output1
abgfedch
```

```input2
1 7
reviver
```

```output2
reviver
```

```input3
4 13
merrychristmas
```

```output3
meramtsirhcyrs
```

## 提示
### 制約

- $ S $ は英小文字のみからなる。
- $ 1\ \le\ |S|\ \le\ 10^5 $ ($ |S| $ は $ S $ の長さ)
- $ L,R $ は整数
- $ 1\ \le\ L\ \le\ R\ \le\ |S| $

### Sample Explanation 1

`abcdefgh` の $ 3 $ 文字目から $ 7 $ 文字目までの部分を反転すると、 `abgfedch` となります。

### Sample Explanation 2

操作を行った結果が元の文字列と同一であることもあります。

