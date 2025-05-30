## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc140/tasks/arc140_c

$ (1,\dots,N) $ の順列 $ P=(P_1,P_2,\ldots,P_N) $ の**嬉しさ**を以下で定義します。

- 長さ $ N-1 $ の数列 $ A=(A_1,A_2,\ldots,A_{N-1}) $ を、$ A_i\ =\ |P_i-P_{i+1}|(1\leq\ i\ \leq\ N-1) $ で定める。 $ A $ の最長狭義単調増加部分列の長さを $ P $ の嬉しさとする。

$ P_1\ =\ X $ を満たす順列 $ P $ のうち、嬉しさが最大になるものを一つ出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $

## 输出格式
$ P_1\ =\ X $ を満たす順列 $ P $ のうち、嬉しさが最大になるものを $ 1 $ つ以下の形式で出力せよ。

> $ P_1 $ $ P_2 $ $ \ldots $ $ P_N $

条件を満たす解が複数存在する場合、どれを出力しても正解とみなされる。

## 题目大意
给定 $m,n$，希望一个长度为 $m$ 并且以 $n$ 开头的排列 $a$ 满足以下条件：令其差分数组的绝对值数列是 $b$（即 $b_i=|a_{i+1}-a_i|$），希望最大化 $b$ 的最长严格上升子序列的长度。如果有多个 $a$ 符合条件，输出一个即可。

```input1
3 2
```

```output1
2 1 3
```

```input2
3 1
```

```output2
1 2 3
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ X\ \leq\ N $
- 入力は全て整数

### Sample Explanation 1

$ A=(1,2) $ となるので、$ P $ の嬉しさは $ 2 $ です。これが達成可能な嬉しさの最大であるため、出力は条件を満たします。

### Sample Explanation 2

$ A=(1,1) $ となるので、$ P $ の嬉しさは $ 1 $ です。これが達成可能な嬉しさの最大であるため、出力は条件を満たします。

