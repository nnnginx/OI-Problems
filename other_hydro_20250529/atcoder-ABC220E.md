## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc220/tasks/abc220_e

$ 2^N-1 $ 頂点からなる木があります。  
 頂点には $ 1 $ から $ 2^N-1 $ の番号がつけられており、各 $ 1\leq\ i\ <\ 2^{N-1} $ について、

- 頂点 $ i $ と頂点 $ 2i $ を結ぶ無向辺
- 頂点 $ i $ と頂点 $ 2i+1 $ を結ぶ無向辺

が存在します。これら以外の辺はありません。

$ 2 $ 頂点間の距離を、その $ 2 $ 頂点を結ぶ単純パスに含まれる辺の個数とします。

頂点の組 $ (i,j) $ であって、距離が $ D $ であるようなものの個数を $ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ D $

## 输出格式
答えを出力せよ。

## 题目大意
给定一个完全二叉树，一共有 $2 ^ N - 1$ 个节点，按 $1$ 到 $2 ^ N - 1$ 编号。其中，对于 $1 \le i < 2 ^ {N  - 1}$，有：

+ 节点 $i$ 与节点 $2i$ 有一条无向边。
+ 节点 $i$ 与节点 $2i + 1$ 有一条无向边。

$2$ 节点之间的距离是连接该 $2$ 节点的简单路径中包含的边数。

求有多少组节点 $(i,j)$，满足节点 $i$ 与节点 $j$ 的距离为 $D$。

答案模 $998244353$。

```input1
3 2
```

```output1
14
```

```input2
14142 17320
```

```output2
11284501
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ 1\ \leq\ D\ \leq\ 2\times\ 10^6 $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

与えられる木は以下の図のようなものです。 !\[図\](https://img.atcoder.jp/ghi/86d098048a50638decb39ed6659d32cf.png) 距離が $ 2 $ であるような頂点の組は $ (1,4),(1,5),(1,6),(1,7),(2,3),(3,2),(4,1),(4,5),(5,1),(5,4),(6,1),(6,7),(7,1),(7,6) $ の $ 14 $ 組存在します。

