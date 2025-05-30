## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc167/tasks/abc167_e

$ N $ 個のブロックが横一列に並んでいます。このブロック列に色を塗ります。

$ 2 $ つのブロック列の塗り方が異なるとは、あるブロックが存在して、そのブロックが異なる色で塗られていることと定義します。

次の条件を満たすブロック列の塗り方が何通りあるか求めてください。

- 各ブロックを色 $ 1 $ から色 $ M $ までのいずれか一色で塗る。使わない色があってもよい。
- 隣り合うブロックの組であって同じ色で塗られている組は、 $ K $ 組以下である。

ただし、答えは非常に大きくなる場合があるので、 $ 998244353 $ で割った余りを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $

## 输出格式
答えを出力せよ。

## 题目大意
有 $n$ 个方格排成一排，你需要给这些方格染色。

你有 $m$ 种颜色给方格染色，每一个方格只可以染一种颜色，且这 $n$ 个方格都需要染色。注意，一种染色方式不一定需要使用所有的颜色。

请问有多少种染色方式，使得**最多**可能有 $k$ 对相邻颜色相同的方格。由于答案可能很大，所以请你输出答案模 $998244353$ 的值。

样例一解释：共有六种方法，分别是：```112```、```121```、```122```、```211```、```212```、```221``` 。

Translate by Chancylaser.

```input1
3 2 1
```

```output1
6
```

```input2
100 100 0
```

```output2
73074801
```

```input3
60522 114575 7559
```

```output3
479519525
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ N,\ M\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ K\ \leq\ N\ -\ 1 $

### Sample Explanation 1

ブロック列の塗り方を色を書き並べた文字列で表すと、条件を満たすブロック列の色の塗り方は、`112` , `121`, `122`, `211`, `212`, `221` です。

