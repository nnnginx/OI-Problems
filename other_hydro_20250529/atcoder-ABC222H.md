## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc222/tasks/abc222_h

正の整数 $ N $ に対して、次の条件を満たす根付き二分木を **$ N $ 次の美しい二分木** と定めます。

- 頂点には $ 0 $ か $ 1 $ が書かれている。
- 頂点が葉ならば、必ず $ 1 $ が書かれている。
- 次の操作を高々 $ N-1 $ 回行うことで、根に書かれている数を $ N $ に、それ以外の頂点に書かれている数を $ 0 $ にすることができる。
  - 頂点 $ u,\ v $ を選ぶ。ここで $ v $ は $ u $ の子、あるいは $ u $ の子の子である必要がある。 $ u,v $ に書かれている数を $ a_u,\ a_v $ としたとき、 $ a_u\ \gets\ a_u\ +\ a_v,\ a_v\ \gets\ 0 $ とする。

$ N $ が与えられるので、$ N $ 次の美しい二分木の個数を $ 998244353 $ で割ったあまりを答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを出力せよ。

## 题目大意
对于一个正整数 $n$，我们称满足以下条件的有根二叉树是一棵美丽的 $n$ 阶二叉树。

- 每个节点有一个数字 $0$ 或 $1$，节点 $i$ 的数字记为 $a_i$。
- 每个叶子节点的数字定是 $1$。
- 可以通过进行如下的操作至多 $n - 1$ 次，使得最终根节点上的数字为 $n$，其余节点的数字是 $0$。
  - 选择两个节点 $u, v$，其中 $u$ 需要是 $v$ 的父节点或父节点的父节点。作赋值 $a_u\leftarrow a_u + a_v, a_v\leftarrow 0$。

给定 $n$，请计算美丽的 $n$ 阶二叉树的数量。答案对 $998244353$ 取模。

$n \le 10^7$。

```input1
1
```

```output1
1
```

```input2
2
```

```output2
6
```

```input3
222
```

```output3
987355927
```

```input4
222222
```

```output4
675337738
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^7 $
- 入力はすべて整数である。

### Sample Explanation 1

条件を満たす二分木は、根に $ 1 $ が書かれている $ 1 $ 頂点の木のみです。

### Sample Explanation 2

条件を満たす二分木は次の $ 6 $ 通りです。 !\[image\](https://img.atcoder.jp/ghi/37c6125e227d459cd725b6ccec96e2c8.png)

