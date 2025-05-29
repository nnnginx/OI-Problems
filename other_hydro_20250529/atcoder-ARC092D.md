## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc092/tasks/arc092_d

$ N $ 頂点 $ M $ 辺の単純な有向グラフが与えられます。 頂点には $ 1,\ 2,\ ...,\ N $ の番号が，辺には $ 1,\ 2,\ ...,\ M $ の番号が付いています。 辺 $ i $ は頂点 $ a_i $ から頂点 $ b_i $ へ伸びています。

それぞれの辺について，もしその辺を反転させたらグラフの強連結成分の個数が変わるかどうかを求めてください。

なお，辺 $ i $ を反転させるとは，グラフから辺 $ i $ を削除し， 新たに頂点 $ b_i $ から頂点 $ a_i $ へ伸びる辺を追加する操作を意味します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ $ : $ $ a_M $ $ b_M $

## 输出格式
$ M $ 行出力せよ。$ i $ 行目には，辺 $ i $ を反転させたらグラフの強連結成分の個数が変わる場合 `diff`，変わらない場合 `same` と出力せよ。

## 题目大意
- 有一个 $N$ 个点 $M$ 条边的有向图。保证图中不存在重边和自环。
- 试判断将每条边反向，其他边不变的情况下，图中强连通分量的数量是否改变。
- 若改变，输出 `diff`，否则输出 `same`。
- $1 \leq N \leq 10^3$，$1 \leq M \leq 2 \times 10^5$。

```input1
3 3
1 2
1 3
2 3
```

```output1
same
diff
same
```

```input2
2 2
1 2
2 1
```

```output2
diff
diff
```

```input3
5 9
3 2
3 1
4 1
4 2
3 5
5 3
3 4
1 2
2 5
```

```output3
same
same
same
same
same
diff
diff
diff
diff
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ M\ \leq\ 200,000 $
- $ 1\ \leq\ a_i,\ b_i\ \leq\ N $
- $ a_i\ \neq\ b_i $
- $ i\ \neq\ j $ ならば $ a_i\ \neq\ a_j $ または $ b_i\ \neq\ b_j $

### Sample Explanation 1

辺を反転させない場合強連結成分の個数は $ 3 $ 個ですが，辺 $ 2 $ を反転させると強連結成分の個数は $ 1 $ 個になります。

### Sample Explanation 2

辺を反転させた結果，グラフに多重辺が生じる場合もあります。

