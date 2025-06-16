## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc255/tasks/abc255_a

整数 $ R,C $ と $ 2 $ 行 $ 2 $ 列からなる行列 $ A $ が与えられるので、 $ A_{R,C} $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ R $ $ C $ $ A_{1,1} $ $ A_{1,2} $ $ A_{2,1} $ $ A_{2,2} $

## 输出格式
答えを整数として出力せよ。

## 题目大意
给定整数 $R,C$ 和一个两行两列的矩阵 $A$ ，输出 $A_{R,C}$ 。

```input1
1 2
1 0
0 1
```

```output1
0
```

```input2
2 2
1 2
3 4
```

```output2
4
```

```input3
2 1
90 80
70 60
```

```output3
70
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \le\ R,C\ \le\ 2 $
- $ 0\ \le\ A_{i,j}\ \le\ 100 $

### Sample Explanation 1

$ A_{1,2}=0 $ です。

### Sample Explanation 2

$ A_{2,2}=4 $ です。

### Sample Explanation 3

$ A_{2,1}=70 $ です。

