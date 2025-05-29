## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc051/tasks/agc051_d

以下の無向グラフにおいて、$ S $ から $ S $ へのウォークであって辺 $ ST $, $ TU $, $ UV $, $ VS $ をそれぞれ $ a $, $ b $, $ c $, $ d $ 回通るもの (向きは不問) の数を $ 998,244,353 $ で割った余りを求めてください。

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_agc051_d/648da6e8de7f6ac243febb92657c094616c7b1d5.png)

## 输入格式
入力は標準入力から以下の形式で与えられる。

> $ a $ $ b $ $ c $ $ d $

## 输出格式
答えを出力せよ。

## 题目大意
有一张 $4$ 个点 $4$ 条边的简单无向连通图，点的编号分别为 $1,2,3,4$ ，边分别连接着 $e1:(1,2),e2:(2,3),e3:(3,4),e4:(4,1) $。

给定 $4$ 个数 $v_1,v_2,v_3,v_4$ 求满足以下条件的路径数量：

从 $1$ 号点出发并到 $1$ 号点结束，且经过第 $i$ 条边 $e_i$ 恰好 $v_i$ 次。

你需要输出路径数对 $998244353$ 取模的结果。

$v_1,v_2,v_3,v_4 \le 5 \times 10^5$

```input1
2 2 2 2
```

```output1
10
```

```input2
1 2 3 4
```

```output2
0
```

```input3
470000 480000 490000 500000
```

```output3
712808431
```

## 提示
### 注記

$ S $ から $ S $ へのウォークとは、頂点の列 $ v_0\ =\ S,\ v_1,\ \ldots,\ v_k\ =\ S $ であって、各 $ i\ (0\ \leq\ i\ <\ k) $ について $ v_i $ と $ v_{i+1} $ を結ぶ辺があるものをいいます。 $ 2 $ つのウォークは、列として異なるときに異なるとみなされます。

### 制約

- $ 1\ \leq\ a,\ b,\ c,\ d\ \leq\ 500,000 $
- 入力中の全ての値は整数である。

### Sample Explanation 1

条件を満たすウォークは $ 10 $ 個あり、その一例は $ S $ $ \rightarrow $ $ T $ $ \rightarrow $ $ U $ $ \rightarrow $ $ V $ $ \rightarrow $ $ U $ $ \rightarrow $ $ T $ $ \rightarrow $ $ S $ $ \rightarrow $ $ V $ $ \rightarrow $ $ S $ です。

