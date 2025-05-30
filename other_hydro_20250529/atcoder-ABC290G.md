## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc290/tasks/abc290_g

$ T $ 個のテストケースについて、以下の問題を解いてください。

深さ $ D $ の完全 $ K $ 分木 ( $ 1+K+K^2+\dots+K^D $ 頂点 ) があります。  
 あなたの目標はこの木の辺を何本か切って、連結成分のうちいずれかを $ X $ 頂点にすることです。  
 目標を達成するために切るべき辺の数の最小値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ T $ $ case_1 $ $ \vdots $ $ case_T $

但し、 $ case_i $ は $ i $ 個目のテストケースである。  
 各テストケースは以下の形式である。

> $ D $ $ K $ $ X $

## 输出格式
全体で $ T $ 行出力せよ。  
 そのうち $ i $ 行目には $ i $ 個目のテストケースに対する答えを整数として出力せよ。

## 题目大意
#### 题目描述

给定一颗满 $K$ 叉树，深度为 $D$，即整棵树有 $1+K+K^2+\dots+K^D$ 个节点。

现在你可以选定若干条边并将其删除（也可以选择不删）。删除后将得到一个森林。求使森林中存在一棵树的节点数为 $X$ 的最小删除边数。

#### 输入格式

第一行一个整数 $T$，表示有 $T$ 组数据。

接下来 $T$ 行，每行三个整数 $D,K,X$。中间用空格隔开。

#### 输出格式

输出共 $T$ 行，每组数据输出一行。对于每组数据，输出最少要删除的边数。

@[robinyqc](https://www.luogu.com.cn/user/338632) 翻译。

```input1
11
2 2 1
2 2 2
2 2 3
2 2 4
2 2 5
2 2 6
2 2 7
1 999999999999999999 1
1 999999999999999999 2
1 999999999999999999 999999999999999999
1 999999999999999999 1000000000000000000
```

```output1
1
2
1
1
2
1
0
1
999999999999999998
1
0
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \le\ T\ \le\ 100 $
- $ 1\ \le\ D $
- $ 2\ \le\ K $
- $ \displaystyle\ 1\ \le\ X\ \le\ \sum_{i=0}^{D}\ K^i\ \le\ 10^{18} $

