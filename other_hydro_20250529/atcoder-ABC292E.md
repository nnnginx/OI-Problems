## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc292/tasks/abc292_e

頂点に $ 1 $ から $ N $ の番号が、辺に $ 1 $ から $ M $ の番号がついた $ N $ 頂点 $ M $ 辺の単純有向グラフが与えられます。辺 $ i $ は頂点 $ u_i $ から頂点 $ v_i $ への有向辺です。

また、あなたは次の操作を $ 0 $ 回以上何度でも行えます。

- 相異なる頂点 $ x,y $ であって頂点 $ x $ から頂点 $ y $ への有向辺が存在しないようなものを選ぶ。そして、頂点 $ x $ から頂点 $ y $ への有向辺を追加する。

このグラフが次の条件を満たす状態にするために最小で何回操作を行う必要があるかを求めてください。

- 相異なる頂点 $ a,b,c $ すべてについて、頂点 $ a $ から頂点 $ b $ への有向辺と頂点 $ b $ から頂点 $ c $ への有向辺がともに存在するならば頂点 $ a $ から頂点 $ c $ への有向辺も存在する。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ \vdots $ $ u_M $ $ v_M $

## 输出格式
答えを出力せよ。

## 题目大意
给出一个简单有向图，你可以执行一下操作多次（也可以不执行）：

- 选择两个没有连边的点 $x$，$y$；
- 连一条 $x \to y$ 的有向边。

现在询问你需要对这个有向图执行至少多少次操作才能使这个有向图满足：若 $a$ 到 $b$ 有边，$b$ 到 $c$ 有边，则 $a$ 到 $c$ 有边。

```input1
4 3
2 4
3 1
4 3
```

```output1
3
```

```input2
292 0
```

```output2
0
```

```input3
5 8
1 2
2 1
1 3
3 1
1 4
4 1
1 5
5 1
```

```output3
12
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 2000 $
- $ 0\ \leq\ M\ \leq\ 2000 $
- $ 1\ \leq\ u_i\ ,v_i\ \leq\ N $
- $ u_i\ \neq\ v_i $
- $ i\ \neq\ j $ ならば $ (u_i,v_i)\ \neq\ (u_j,v_j) $
- 入力はすべて整数

### Sample Explanation 1

初め、一例として頂点 $ 2,4,3 $ について、頂点 $ 2 $ から頂点 $ 4 $ への有向辺と頂点 $ 4 $ から頂点 $ 3 $ への有向辺がともに存在するにもかかわらず、頂点 $ 2 $ から頂点 $ 3 $ への有向辺は存在せず、条件を満たさない状態です。 そこで、以下の $ 3 $ 本の有向辺を追加すると条件を満たす状態になります。 - 頂点 $ 2 $ から頂点 $ 3 $ への有向辺 - 頂点 $ 2 $ から頂点 $ 1 $ への有向辺 - 頂点 $ 4 $ から頂点 $ 1 $ への有向辺 一方、$ 3 $ 本未満の追加で条件を満たす状態には出来ないため、答えは $ 3 $ です。

