## 题目描述
[problemUrl]: https://atcoder.jp/contests/dwacon6th-prelims/tasks/dwacon6th_prelims_c

$ N $ 人の子供たちがいます。子供たちには $ 1,2,\ldots,N $ と番号が振られています。 これから $ K $ 日間、子供たちにクッキーが配られることになりました。 $ i $ 日目には $ N $ 人の中から $ a_i $ 人の子供が等確率で選ばれ、選ばれた子供たちはそれぞれクッキーを $ 1 $ 枚受け取ります。($ K $ 回の子供の選択はすべて独立に行われます。)

$ K $ 日間で子供 $ i $ が受け取るクッキーの枚数を $ c_i $ として、子供たちの *うれしさ* を $ c_1\ \times\ c_2\ \times\ \ldots\ \times\ c_N $ で定義します。 うれしさの期待値に $ \binom{N}{a_1}\ \times\ \binom{N}{a_2}\ \times\ \ldots\ \times\ \binom{N}{a_K} $ をかけた値(これは整数となることが示せます)を $ 10^9+7 $ で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ a_1 $ $ a_2 $ $ \ldots $ $ a_K $

## 输出格式
答えを出力せよ。

## 题目大意
一共有 $N$ 个人，在 $K$ 天中的第 $i$ 天随机给 $a_i$ 个人发一块饼干。$c_i$ 为第 $i$ 个人在 $k$ 天中获得的糖果总数。求 $c_1 \times c_2 \times c_3 \cdots \times c_N \times \begin{pmatrix}N\\a_1\end{pmatrix} \times \begin{pmatrix}N\\a_2\end{pmatrix} \times \cdots \times \begin{pmatrix}N\\a_K\end{pmatrix}$ 的期望值 $\text{mod} \ 10^9+7$。

```input1
3 2
3 2
```

```output1
12
```

```input2
856 16
399 263 665 432 206 61 784 548 422 313 848 478 827 26 398 63
```

```output2
337587117
```

## 提示
### 注記

$ \binom{n}{k} $ は異なる $ n $ 個の対象から $ k $ 個を選ぶ選び方の総数を表します。

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ K\ \leq\ 20 $
- $ 1\ \leq\ a_i\ \leq\ N $

### Sample Explanation 1

\- $ 1 $ 日目では、子供 $ 1,2,3 $ のいずれもクッキーを受け取ります。 - $ 2 $ 日目では、子供 $ 1,2,3 $ のいずれか $ 1 $ 人がクッキーを受け取りません。 - どの場合もうれしさは $ 4 $ のため、うれしさの期待値は $ 4 $ となります。これに $ \binom{3}{3}\ \times\ \binom{3}{2} $ をかけた値である $ 12 $ を出力してください。

### Sample Explanation 2

\- 期待値の $ \binom{N}{a_1}\ \times\ \binom{N}{a_2}\ \times\ \ldots\ \times\ \binom{N}{a_K} $ 倍を $ 10^9+7 $ で割ったあまりを求めてください。

