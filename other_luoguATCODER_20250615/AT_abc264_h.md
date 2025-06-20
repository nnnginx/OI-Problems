# AT_abc264_h [ABC264Ex] Perfect Binary Tree

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc264/tasks/abc264_h

頂点に $ 1,2,\dots,N $ の番号が付いた、 $ N $ 頂点の根付き木があります。  
 根は頂点 $ 1 $ であり、頂点 $ i\ \ge\ 2 $ について、その親は $ P_i(\ <\ i) $ です。  
 整数 $ k=1,2,\dots,N $ に対し次の問題を解いてください。

番号が $ 1 $ 以上 $ k $ 以下の頂点を、頂点 $ 1 $ を含むようにいくつか選ぶ方法は $ 2^{k-1} $ 通りあります。  
 そのうち、選ばれた頂点集合から誘導される部分グラフの形状が頂点 $ 1 $ を根とする (頂点数がある正整数 $ d $ を用いて $ 2^d-1 $ と表せるような) 完全二分木になるような頂点の選び方はいくつですか?  
 答えは非常に大きくなる場合があるので、$ 998244353 $ で割った余りを求めてください。

 誘導される部分グラフとは?

あるグラフ $ G $ から、一部の頂点を選んだ集合を $ S $ とします。この頂点集合 $ S $ から誘導される部分グラフ $ H $ は以下のように構成されます。

- $ H $ の頂点集合は $ S $ と一致させます。
- その後、 $ H $ に以下のように辺を追加します。
- $ i,j\ \in\ S,\ i\ を満たす全ての頂点対\ (i,j) $ について、 $ G $ 中に $ i,j $ を結ぶ辺が存在すれば、 $ H $ にも $ i,j $ を結ぶ辺を追加する。
 

完全二分木とは? 完全二分木とは、以下の全ての条件を満たす根付き木です。 - 葉以外の全ての頂点が、ちょうど $ 2 $ つの子を持つ。
- 全ての葉が根から等距離にある。
 
 ただし、頂点が $ 1 $ つで辺が $ 0 $ 本のグラフも完全二分木であるものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ P_2 $ $ P_3 $ $ \dots $ $ P_N $

## 输出格式

$ N $ 行出力せよ。 そのうち $ i $ ( $ 1\ \le\ i\ \le\ N $ ) 行目には $ k=i $ についての答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10
1 1 2 1 2 5 5 5 1
```

### 输出 #1

```
1
1
2
2
4
4
4
5
7
10
```

## 输入输出样例 #2

### 输入 #2

```
1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
10
1 2 3 4 5 6 7 8 9
```

### 输出 #3

```
1
1
1
1
1
1
1
1
1
1
```

## 输入输出样例 #4

### 输入 #4

```
13
1 1 1 2 2 2 3 3 3 4 4 4
```

### 输出 #4

```
1
1
2
4
4
4
4
4
7
13
13
19
31
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ N\ \le\ 3\ \times\ 10^5 $
- $ 1\ \le\ P_i\ <\ i $

### Sample Explanation 1

\- $ k\ \ge\ 1 $ であるとき $ \{1\} $ - $ k\ \ge\ 3 $ であるとき $ \{1,2,3\} $ - $ k\ \ge\ 5 $ であるとき $ \{1,2,5\},\{1,3,5\} $ - $ k\ \ge\ 8 $ であるとき $ \{1,2,4,5,6,7,8\} $ - $ k\ \ge\ 9 $ であるとき $ \{1,2,4,5,6,7,9\},\{1,2,4,5,6,8,9\} $ - $ k\ =\ 10 $ であるとき $ \{1,2,10\},\{1,3,10\},\{1,5,10\} $ が数えるべき頂点の選び方となります。

### Sample Explanation 2

$ N=1 $ である場合、入力の $ 2 $ 行目は空行です。