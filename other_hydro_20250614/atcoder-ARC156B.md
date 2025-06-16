## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc156/tasks/arc156_b

有限個の非負整数からなる多重集合 $ S $ にたいして、$ \mathrm{mex}(S) $ を、$ S $ に含まれない最小の非負整数と定義します。例えば、$ \mathrm{mex}(\lbrace\ 0,0,\ 1,3\rbrace\ )\ =\ 2,\ \mathrm{mex}(\lbrace\ 1\ \rbrace)\ =\ 0,\ \mathrm{mex}(\lbrace\ \rbrace)\ =\ 0 $ です。

黒板に $ N $ 個の非負整数が書かれており、$ i $ 番目の非負整数は $ A_i $ です。

あなたは、以下の操作をちょうど $ K $ 回行います。

- 黒板に書かれている非負整数を $ 0 $ 個以上選ぶ。選んだ非負整数からなる多重集合を $ S $ として、$ \mathrm{mex}(S) $ を黒板に $ 1 $ 個書き込む。
 
最終的に黒板に書かれている非負整数の多重集合としてありうるものの個数を $ 998244353 $ で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
答えを出力せよ。

## 题目大意
你有一个大小为 $N$ 的多重集 $A$。

你需要执行 $K$ 次操作，每次选取 $S \subseteq A$，然后在 $A$ 中插入 $\mathrm{mex}(S)$，表示 $S$ 内最小没有出现过的自然数。

问最终 $A$ 有多少种可能的结果。答案对 $998244353$ 取模。

```input1
3 1
0 1 3
```

```output1
3
```

```input2
2 1
0 0
```

```output2
2
```

```input3
5 10
3 1 4 1 5
```

```output3
7109
```

## 提示
### 制約

- $ 1\ \leq\ N,K\ \leq\ 2\times\ 10^5 $
- $ 0\leq\ A_i\leq\ 2\times\ 10^5 $
- 入力される数値は全て整数
 
### Sample Explanation 1

操作後に得られる多重集合は、以下の $ 3 $ 通りです。 - $ \lbrace\ 0,0,1,3\ \rbrace $ - $ \lbrace\ 0,1,1,3\rbrace $ - $ \lbrace\ 0,1,2,3\ \rbrace $ 例えば、$ \lbrace\ 0,1,1,3\rbrace $ は黒板に書かれている $ 0 $ を選び、$ S=\lbrace\ 0\rbrace $ として操作をすることで得られます。

### Sample Explanation 2

操作後に得られる多重集合は、以下の $ 2 $ 通りです。 - $ \lbrace\ 0,0,0\ \rbrace $ - $ \lbrace\ 0,0,1\rbrace $ 操作で選ぶ整数は $ 0 $ 個でも良いことに注意してください。

