## 题目描述
[problemUrl]: https://atcoder.jp/contests/toyota2023spring-final/tasks/toyota2023spring_final_g

プログラミング初心者のすぬけくんが，以下のようなコードを書きました．

```
N = read_integer()

parent = array(N, -1) //長さ N の配列 parent を作り，すべての要素を -1 で初期化

find(v):
    if parent[v] == -1:
        return v
    else:
        return find(parent[v])

union(a,b):
    parent[find(b)] = find(a)

for i = 0 to N-2:
    A_i = read_integer()
    B_i = read_integer()
    union(A_i,B_i)
```

これは，$ N $ 頂点の木の情報を受けとり，Union-Find で辺を結ぶだけのプログラムです．

プログラミングマスターのりんごさんは，このプログラムの欠陥に気が付きました． すなわち，Union-Find に一切の高速化が施されていないのです．

今，りんごさんは $ N $ 頂点からなる木 $ T $ を持っています． $ T $ の頂点には $ 0 $ から $ N-1 $ までの番号が，辺には $ 0 $ から $ N-2 $ までの番号がついています． 辺 $ i $ は頂点 $ A_i $ と頂点 $ B_i $ を結ぶ辺です．

りんごさんは，すぬけくんのプログラムに $ T $ を入力として与えようとしています． ただしその前に，$ T $ の辺の番号と，辺の端点の順番を自由に入れ替えることができます．

りんごさんは，すぬけくんのプログラムが非効率的であることを示すために，`find` 関数が呼ばれる回数を最大化したいです． `find` 関数が呼ばれる回数の最大値を求めてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ A_0 $ $ B_0 $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_{N-2} $ $ B_{N-2} $

## 输出格式
答えを出力せよ．

## 题目大意
这是一段没有路径压缩的并查集代码：

```
N = read_integer()

parent = array(N, -1) // 用 -1 初始化长为 N 的序列

find(v):
    if parent[v] == -1:
        return v
    else:
        return find(parent[v])

union(a,b):
    parent[find(b)] = find(a)

for i = 0 to N-2:
    A_i = read_integer()
    B_i = read_integer()
    union(A_i,B_i)
```

现在，给定 $n$ 个元素 和 $n-1$ 次合并，每次合并编号为 $A_i,B_i$ 的元素（从 0 开始标号），保证合并完后所有元素都在同一集合。

你可以任意更换合并的顺序，或者将 $A_i,B_i$ 交换。请你最小化 `find` 函数调用的次数。$2\le n\le 2000$。

```input1
2
0 1
```

```output1
2
```

```input2
3
0 1
0 2
```

```output2
5
```

```input3
5
0 1
0 2
0 3
3 4
```

```output3
13
```

```input4
20
6 16
10 6
16 8
1 5
9 4
5 3
13 16
19 10
12 2
14 10
12 18
0 2
15 16
12 7
11 14
1 10
6 4
17 8
12 1
```

```output4
148
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2000 $
- $ 0\ \leq\ A_i,B_i\ \leq\ N-1 $
- $ A_i\ \neq\ B_i $
- 入力されるグラフは木である

### Sample Explanation 1

`find` 関数は必ず $ 2 $ 回呼ばれます．

### Sample Explanation 2

辺 $ 0 $ の端点の順番を入れ替え，以下のような入力を作ると，`find` 関数が $ 5 $ 回呼ばれます． ``` 3 1 0 0 2 ```

### Sample Explanation 3

辺の順番と辺の端点の順番を適切に入れ替え，以下のような入力を作ると，`find` 関数が $ 13 $ 回呼ばれます． ``` 5 3 0 4 3 1 0 0 2 ```

