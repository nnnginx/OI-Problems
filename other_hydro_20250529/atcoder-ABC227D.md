## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc227/tasks/abc227_d

キーエンスには $ N $ 個の部署があり、$ i\,(1\ \leq\ i\ \leq\ N) $ 番目の部署には $ A_i $ 人の社員が所属しています。異なる部署に同じ社員が所属していることはありません。

キーエンスは、部署をまたいだ全社横断プロジェクトを計画しています。$ 1 $ つのプロジェクトは $ K $ 個の相異なる部署から $ 1 $ 人ずつ選出して作り、ちょうど $ K $ 人から構成されるようにします。

プロジェクトは最大でいくつ作れますか？ただし、$ 1 $ 人が複数のプロジェクトに参加することはできません。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
プロジェクトの個数の最大値を出力せよ。

## 题目大意
一个公司有 $N$ 个部门，第 $i$ 个部门有 $A_i$ 名员工。不会有员工同时属于多个不同部门。
公司计划建立若干个横跨不同部门的项目，一个项目必须由来自不同部门的恰好 $K$ 名员工组成。
问最多可以同时建立多少个项目？

```input1
3 3
2 3 4
```

```output1
2
```

```input2
4 2
1 1 3 4
```

```output2
4
```

```input3
4 3
1 1 3 4
```

```output3
2
```

## 提示
### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^{12} $
- 入力は全て整数

### Sample Explanation 1

$ 3 $ 個の部署それぞれから $ 1 $ 人ずつ選出したプロジェクトを $ 2 $ つ作ることができます。

