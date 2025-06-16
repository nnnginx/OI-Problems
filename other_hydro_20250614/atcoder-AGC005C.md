## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_c

青木君は数列と木が大好きです。

青木君はある日高橋くんから長さ $ N $ の数列 $ a_1,\ a_2,\ ...,\ a_N $ を貰いました。そしてこの数列を見て、木を作りたくなりました。

青木君が作りたいのは、頂点数が $ N $ で、全ての $ i\ =\ 1,2,...,N $ について頂点 $ i $ と最も遠い頂点の距離が $ a_i $ となる木です。なお、辺の長さは全て $ 1 $ とします。

これを満たす木が存在するか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式
条件を満たす木が存在するならば `Possible`、しないならば `Impossible` と出力する。

## 题目大意
## Description
   青木君特别喜欢数列和树，他觉得它们是世界上最美妙的事物。

   有一天，神仙给了青木君一个长度为 $N$ 的整数数列 $a$。这让青木君特别想构造一棵美妙树。

   美妙树的每条边长度都为 $1$。而且美妙树有一个最重要的性质：对于每一个点 $i(1\le i\le N)$，在树中离它距离最远的点与它的距离应恰好等于 $a _ i$。

   青木君想了想就秒掉了这题，他决定考考你：对于一个给定的序列，是否存在一棵美妙树？

    

## Input
   第一行一个正整数 $N(2 \le N \le 100)$。

   接下来一行，有 $N$ 个正整数，描述序列 $a _ 1, a _ 2, \cdots , a _ N$，其中 $1 \le a _ i \le N-1$。

## Output
   如果对于输入的序列存在美妙树，则输出 `Possible`，否则输出 `Impossible`。

```input1
5
3 2 2 3 3
```

```output1
Possible
```

```input2
3
1 1 2
```

```output2
Impossible
```

```input3
10
1 2 2 2 2 2 2 2 2 2
```

```output3
Possible
```

```input4
10
1 1 2 2 2 2 2 2 2 2
```

```output4
Impossible
```

```input5
6
1 1 1 1 1 5
```

```output5
Impossible
```

```input6
5
4 3 2 3 4
```

```output6
Possible
```

## 提示
### 制約

- $ 2\ ≦\ N\ ≦\ 100 $
- $ 1\ ≦\ a_i\ ≦\ N-1 $

### Sample Explanation 1

!\[\](https://atcoder.jp/img/agc005/cda0380bb5cd1b9502cfceaf2526d91e.png) 上図は条件を見たす木の一例です。赤い矢印は最も遠い頂点への経路を表します。

