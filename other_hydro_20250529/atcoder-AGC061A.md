## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc061/tasks/agc061_a

配列 $ A_1,\ \ldots,\ A_N $ があり、はじめ全ての $ i $ について $ A_i\ =\ i $ です。手順 $ \mathrm{shuffle}(L,\ R) $ を以下として定義します。

- $ R\ =\ L\ +\ 1 $ なら、$ A_L $ と $ A_R $ の値を入れ替えて終了する。
- そうでないなら、$ \mathrm{shuffle}(L,\ R\ -\ 1) $ を実行してから $ \mathrm{shuffle}(L\ +\ 1,\ R) $ を実行する。

$ \mathrm{shuffle}(1,\ N) $ を行うとします。手順終了後の $ A_K $ の値を出力してください。

各入力ファイルについて、テストケースを $ T $ 個解いてください。

## 输入格式
入力は、標準入力から以下の形式で与えられる。

> $ T $ $ case_1 $ $ case_2 $ $ \vdots $ $ case_T $

各ケースは、以下の形式である。

> $ N $ $ K $

## 输出格式
$ T $ 行出力せよ。$ i $ 行目に、$ i $ 個目のテストケースの答えを出力すること。

## 题目大意
## 题目描述

你有一个排列长度为 $n(n\le10^{18})$ 的排列 $A$，初始 $A_i=i$，现在对它进行一次 $\mathrm{shuffle}(1,n)$ 操作。$\mathrm{shuffle}(L,R)$ 的定义如下：
- $ R\ =\ L\ +\ 1 $ 时，$\mathrm{swap}(A_L,A_R)$
- 否则，依次执行 $\mathrm{shuffle}(L,R-1)$, $\mathrm{shuffle}(L+1,R)$

您需要求出 $ \mathrm{shuffle}(1,\ n) $ 执行完毕后，$A_k (1\le k\le n)$ 的值。共 $T$ 组数据。

```input1
7
2 1
2 2
5 1
5 2
5 3
5 4
5 5
```

```output1
2
1
2
4
1
5
3
```

## 提示
### 制約

- $ 1\ \leq\ T\ \leq\ 1000 $
- $ 2\ \leq\ N\ \leq\ 10^{18} $
- $ 1\ \leq\ K\ \leq\ N $

### Sample Explanation 1

$ N=2 $ のときは、以下を行って $ A=(2,1) $ を得ます。 - $ \mathrm{shuffle}(1,\ 2) $ を実行し、$ A_1 $ と $ A_2 $ を入れ替える。 $ N=5 $ のときは、以下を行って $ A=(2,4,1,5,3) $ を得ます。 - $ \mathrm{shuffle}(1,\ 5) $ を実行する。 - $ \mathrm{shuffle}(1,\ 4) $ を実行する。 - $ \mathrm{shuffle}(1,\ 3) $ を実行する。 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 4) $ を実行する。 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 5) $ を実行する。 - $ \mathrm{shuffle}(2,\ 4) $ を実行する。 - $ \vdots $ - $ \mathrm{shuffle}(3,\ 5) $ を実行する。 - $ \vdots $

