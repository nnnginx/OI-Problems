## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc057/tasks/agc057_e

$ H\times\ W $ 行列 $ A\ =\ (A_{i,j}) $ ($ 1\leq\ i\leq\ H,\ 1\leq\ j\leq\ W $) に対して、次の操作を考えます。

- **行ソート**：すべての行を昇順にソートする。つまり、すべての $ i $ に対して $ A_{i,1},\ldots,A_{i,W} $ を昇順にソートする。
- **列ソート**：すべての列を昇順にソートする。つまり、すべての $ j $ に対して $ A_{1,j},\ldots,A_{H,j} $ を昇順にソートする。

$ H\times\ W $ 行列 $ B\ =\ (B_{i,j}) $ が与えられます。次の $ 2 $ 条件をともに満たす $ H\times\ W $ 行列 $ A $ の総数を $ 998244353 $ で割った余りを求めてください。

- $ A $ に対して行ソート、列ソートをこの順に行った結果は $ B $ に一致する。
- $ A $ に対して列ソート、行ソートをこの順に行った結果は $ B $ に一致する。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ H $ $ W $ $ B_{1,1} $ $ B_{1,2} $ $ \ldots $ $ B_{1,W} $ $ \vdots $ $ B_{H,1} $ $ B_{H,2} $ $ \ldots $ $ B_{H,W} $

## 输出格式
条件を満たす行列 $ A $ の総数を $ 998244353 $ で割った余りを出力してください。

## 题目大意
给定一个 $n\times m$，值域 $[0,9]$ 的矩阵 $B$，请你计数有多少个大小相同的矩阵 $A$ 满足下列条件：

- 分别对 $A$ 的 **每一列** 中元素从小到大排序，再分别对 $A$ 的 **每一行** 中元素从小到大排序能够得到 $B$。
- 分别对 $A$ 的 **每一行** 中元素从小到大排序，再分别对 $A$ 的 **每一列** 中元素从小到大排序能够得到 $B$。

$1\le n,m\le 1500$，答案对 998244353 取模。

```input1
2 2
0 0
1 2
```

```output1
4
```

```input2
3 3
0 1 3
2 4 7
5 6 8
```

```output2
576
```

```input3
3 5
0 0 0 1 1
0 0 1 1 2
0 1 1 2 2
```

```output3
10440
```

```input4
1 7
2 3 3 6 8 8 9
```

```output4
1260
```

## 提示
### 制約

- $ 1\leq\ H,\ W\leq\ 1500 $
- $ 0\leq\ B_{i,j}\leq\ 9 $
- 任意の $ 1\leq\ i\leq\ H $ および $ 1\leq\ j\leq\ W\ -\ 1 $ に対して $ B_{i,j}\leq\ B_{i,j+1} $
- 任意の $ 1\leq\ j\leq\ W $ および $ 1\leq\ i\leq\ H\ -\ 1 $ に対して $ B_{i,j}\leq\ B_{i+1,j} $
- 入力される値はすべて整数

### Sample Explanation 1

条件を満たす行列は次の $ 4 $ つです：$ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $, $ \begin{pmatrix}0&amp;0\\2&amp;1\end{pmatrix} $, $ \begin{pmatrix}1&amp;2\\0&amp;0\end{pmatrix} $, $ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix} $. 例えば、$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix} $ が条件を満たすことは次のように確かめられます。 - 行ソート、列ソートをこの順に行う場合：$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix}\to\ \begin{pmatrix}1&amp;2\\0&amp;0\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $. - 列ソート、行ソートをこの順に行う場合：$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix}\to\ \begin{pmatrix}0&amp;0\\2&amp;1\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $.

### Sample Explanation 2

例えば $ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix} $ が条件を満たします。このことは次のように確かめられます。 - 行ソート、列ソートをこの順に行う場合：$ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix}\to\ \begin{pmatrix}5&amp;6&amp;7\\0&amp;1&amp;3\\2&amp;4&amp;8\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;1&amp;3\\2&amp;4&amp;7\\5&amp;6&amp;8\end{pmatrix} $. - 列ソート、行ソートをこの順に行う場合：$ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix}\to\ \begin{pmatrix}3&amp;0&amp;1\\4&amp;7&amp;2\\5&amp;8&amp;6\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;1&amp;3\\2&amp;4&amp;7\\5&amp;6&amp;8\end{pmatrix} $.

