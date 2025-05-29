## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc152/tasks/abc152_f

$ 1 $ から $ N $ までの番号がつけられた $ N $ 個の頂点を持つ木があります。 この木の $ i $ 番目の辺は頂点 $ a_i $ と頂点 $ b_i $ を結んでいます。  
 この木の各辺に、それぞれ白か黒の色を塗ることを考えます。このような塗り方は $ 2^{N-1} $ 通り考えられますが、そのうち以下の $ M $ 個の制約をすべて満たすものの個数を求めてください。

- $ i(1\ \leq\ i\ \leq\ M) $ 番目の制約は、 $ 2 $ つの整数 $ u_i $ と $ v_i $ によって表される。これは、頂点 $ u_i $ と頂点 $ v_i $ を結ぶパスに含まれる辺のうち、黒く塗られているものが $ 1 $ つ以上存在しなければならないことを意味する。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ b_1 $ $ : $ $ a_{N-1} $ $ b_{N-1} $ $ M $ $ u_1 $ $ v_1 $ $ : $ $ u_M $ $ v_M $

## 输出格式
$ M $ 個の制約をすべて満たす塗り方の個数を出力せよ。

## 题目大意
给你一颗有n个节点的树，你要给这棵树黑白染色，并且符合m条限制，每条限制给定u和v，需要满足u到v的路径上至少有一个黑色边，问有多少种染色方案。

```input1
3
1 2
2 3
1
1 3
```

```output1
3
```

```input2
2
1 2
1
1 2
```

```output2
1
```

```input3
5
1 2
3 2
3 4
5 3
3
1 3
2 4
2 5
```

```output3
9
```

```input4
8
1 2
2 3
4 3
2 5
6 3
6 7
8 6
5
2 7
3 5
1 6
2 8
7 8
```

```output4
62
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 50 $
- $ 1\ \leq\ a_i,b_i\ \leq\ N $
- 入力で与えられるグラフは木である。
- $ 1\ \leq\ M\ \leq\ \min(20,\frac{N(N-1)}{2}) $
- $ 1\ \leq\ u_i\ <\ v_i\ \leq\ N $
- $ i\ \not=\ j $ なら $ u_i\ \not=u_j $ または $ v_i\not=v_j $
- 入力はすべて整数である。

### Sample Explanation 1

この入力中の木は以下のようなものです。 !\[図\](https://img.atcoder.jp/ghi/5b0208ab1e3bb39a5d4fb7bafbfc448e.png) 辺 $ 1 $ と辺 $ 2 $ をそれぞれ (白,黒), (黒,白), (黒,黒) で塗った場合に、$ M $ 個の制約をすべて満たすことができます。 したがって答えは $ 3 $ です。

### Sample Explanation 2

この入力中の木は以下のようなものです。 !\[図\](https://img.atcoder.jp/ghi/d08b3f53dfa4857fe9ffe13fa5d7ae69.png) 辺 $ 1 $ を黒く塗った場合のみ、 $ M $ 個の制約をすべて満たすことができます。 したがって答えは $ 1 $ です。

### Sample Explanation 3

この入力中の木は以下のようなものです。 !\[図\](https://img.atcoder.jp/ghi/386502bb3c85e0bb5aee64e4e7c087a1.png)

### Sample Explanation 4

この入力中の木は以下のようなものです。 !\[図\](https://img.atcoder.jp/ghi/955fa8fd8af658abb24ff2f68b9997be.png)

