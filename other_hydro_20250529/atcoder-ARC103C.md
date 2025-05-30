## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc103/tasks/arc103_c

長さ $ n $ の文字列 $ s $ が与えられます。 以下の条件を満たす $ n $ 頂点の木は存在するでしょうか？

- 各頂点には $ 1,2,...,\ n $ の番号が付けられている
- 各辺には $ 1,2,...,\ n-1 $ の番号が付けられていて、$ i $ 番目の辺は 頂点 $ u_i $ と $ v_i $ をつないでいる
- $ s $ の $ i $ 番目の文字が `1` であるとき、 木からある辺を $ 1 $ つ取り除くことで、サイズ $ i $ の連結成分が作れる
- $ s $ の $ i $ 番目の文字が `0` であるとき、 木からどのように辺を $ 1 $ つ取り除いてもサイズ $ i $ の連結成分が作れない

条件を満たす木が存在する場合、$ 1 $ つ構築してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
条件を満たす $ n $ 頂点の木が存在しない場合、`-1` と出力してください。

条件を満たす $ n $ 頂点の木が存在する場合、 $ n-1 $ 行出力してください。 $ i $ 行目には $ u_i,v_i $ を空白区切りで出力してください。 複数の木が条件を満たす場合、どれを出力しても構いません。

## 题目大意
给定一个长度为 $n$ 的 $01$ 序列 $\{s_n\}$。

尝试构造一棵具有如下性质的 $n$ 个结点的树：

>$\forall i\in[1,n]\cap\mathbb{Z_+}$，$s_i$ 若为 $1$ ，则一定存在大小为 $i$ 的连通块；$s_i$ 若为 $0$ ，则一定不存在大小为 $i$ 的连通块。  
> 定义连通块为删去一条边后的一个极大连通分量。

$1 \le n \le {10}^5$。

```input1
1111
```

```output1
-1
```

```input2
1110
```

```output2
1 2
2 3
3 4
```

```input3
1010
```

```output3
1 2
1 3
1 4
```

## 提示
### 制約

- $ 2\leq\ n\ \leq\ 10^5 $
- $ s $ は `0` と `1` からなる長さ $ n $ の文字列

### Sample Explanation 1

$ n $ 頂点の木から辺を $ 1 $ つ取り除いてサイズ $ n $ の連結成分を作ることはできません。

### Sample Explanation 2

$ 1 $ 番目の辺または $ 3 $ 番目の辺を取り除くと、サイズ $ 1 $ の連結成分とサイズ $ 3 $ の連結成分ができます。 $ 2 $ 番目の辺を取り除くと、サイズ $ 2 $ の連結成分が $ 2 $ つできます。

### Sample Explanation 3

どの辺を取り除いても、サイズ $ 1 $ の連結成分とサイズ $ 3 $ の連結成分ができます。

