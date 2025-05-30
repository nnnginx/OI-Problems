## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc145/tasks/arc145_d

以下の条件を全て満たす整数集合 $ S $ を一つ構築してください。なお、この問題の制約下で条件を満たす $ S $ が少なくとも一つ存在することが証明できます。

- $ S $ の要素数は $ N $
- $ S $ の要素は $ -10^7 $ 以上 $ 10^7 $ 以下の相異なる整数
- $ \displaystyle\ \sum\ _{s\ \in\ S}\ s\ =\ M $
- $ S $ の任意の相異なる要素 $ x,y,z $ $ (x\ <\ y\ <\ z) $ について $ y-x\neq\ z-y $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
$ S $ の要素を $ s_1,s_2,\ldots,s_N $ とする。条件を満たす $ S $ を $ 1 $ つ以下の形式で出力せよ。

> $ s_1 $ $ s_2 $ $ \ldots $ $ s_N $

条件を満たす解が複数存在する場合、どれを出力しても正解とみなされる。

## 题目大意
构造一个满足以下条件的整数集合 $S$。可以证明在本题的约束下一定存在至少一个。

- $S$ 里有恰好 $N$ 个元素。
- $\forall x\in S$，$-10^7\le x\le 10^7$，且 $x$ 两两不同。
- $\sum\limits_{x\in S} x=M$。
- $\forall x,y,z\in S$，若 $x<y<z$，则 $y-x\neq z-y$。

$1\le N\le 10^4$，$|M|\le N\times 10^6$。

```input1
3 9
```

```output1
1 2 6
```

```input2
5 -15
```

```output2
-15 -5 0 2 3
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^4 $
- $ |M|\ \leq\ N\times\ 10^6 $
- 入力は全て整数

### Sample Explanation 1

$ 2-1\ \neq\ 6-2 $ であり、 $ 1+2+6=9 $ なのでこの出力は条件を満たします。他にも様々な答えが考えられます。

### Sample Explanation 2

$ M $ が負のこともあります。

