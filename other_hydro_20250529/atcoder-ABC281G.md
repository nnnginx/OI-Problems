## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc281/tasks/abc281_g

正整数 $ N,\ M $ が与えられます。  
 頂点に $ 1,\ \dots,\ N $ の番号が付けられた $ N $ 頂点の単純連結無向グラフであって、以下の条件を満たすものの総数を $ M $ で割った余りを求めてください。

- 全ての $ u\ =\ 2,\ \dots,\ N-1 $ について、頂点 $ 1 $ から頂点 $ u $ までの最短距離は、頂点 $ 1 $ から頂点 $ N $ までの最短距離より真に小さい。
 
ただし、頂点 $ u $ から頂点 $ v $ までの最短距離とは、頂点 $ u,\ v $ を結ぶ単純パスに含まれる辺の本数の最小値を指します。  
 また、$ 2 $ つのグラフが異なるとは、ある $ 2 $ 頂点 $ u,\ v $ が存在して、これらの頂点を結ぶ辺が一方のグラフにのみ存在することを指します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式
答えを出力せよ。

## 题目大意
构造一张 $N$ 个点的无向连通图，边权都是 $1$。记图中 $1$ 到 $u$ 的最短路径长度为 $d_u$，你需要保证 $\max\{d_1,d_2,...,d_{N-1}\}$ **严格小于** $d_N$。求构造方案数模 $M$ 的值，方案区分节点编号。

```input1
4 1000000000
```

```output1
8
```

```input2
3 100000000
```

```output2
1
```

```input3
500 987654321
```

```output3
610860515
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 500 $
- $ 10^8\ \leq\ M\ \leq\ 10^9 $
- $ N,\ M $ は整数
 
### Sample Explanation 1

以下の $ 8 $ 通りが条件を満たします。 !\[example\_00\](https://img.atcoder.jp/abc281/5c77dfe15dfa3c03666e654bf8cfdc01.png)

### Sample Explanation 3

$ M $ で割った余りを求めることに注意してください。

