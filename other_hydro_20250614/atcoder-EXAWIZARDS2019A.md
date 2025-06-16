## 题目描述
[problemUrl]: https://atcoder.jp/contests/exawizards2019/tasks/exawizards2019_a

$ 3 $ つの整数 $ A,B,C $ が与えられます。

三辺の長さがそれぞれ $ A,B,C $ であるような正三角形が存在するかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $

## 输出格式
三辺の長さが $ A,B,C $ であるような正三角形が存在するなら `Yes` を、そうでなければ `No` を出力せよ。

## 题目大意
给出三个整数 $A$，$B$ 和 $C$。

确定是否存在边长为 $A$，$B$ 和 $C$ 的等边三角形。

```input1
2 2 2
```

```output1
Yes
```

```input2
3 4 5
```

```output2
No
```

## 提示
### 制約

- 入力は全て整数である。
- $ 1\ \leq\ A,B,C\ \leq\ 100 $

### Sample Explanation 1

\- 三辺の長さが $ 2,2,2 $ であるような正三角形は存在します。

### Sample Explanation 2

\- 三辺の長さが $ 3,4,5 $ であるような正三角形は存在しません。

