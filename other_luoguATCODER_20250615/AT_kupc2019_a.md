# AT_kupc2019_a November Festival

## 题目描述

[problemUrl]: https://atcoder.jp/contests/kupc2019/tasks/kupc2019_a

京都大学で NF (November Festival) のテーマを決める投票が行われています。

$ N $ 個のテーマ案があり、 $ i $ 番目のテーマ案には現在 $ a_i $ 票が投じられています。

これから $ X $ 票が投じられていようとしています。

テーマは、これら $ X $ 票の投票後に得票数が最大であるようなテーマ案の内からランダムに選ばれます。

テーマとして選ばれる可能性のあるテーマ案の個数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式

テーマとして選ばれる可能性のあるテーマ案の個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 5
1 3 5 7 9
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5 2
1 3 5 7 9
```

### 输出 #2

```
2
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ a_i\ \leq\ 1000 $
- $ 1\ \leq\ X\ \leq\ 1000 $
- 入力は全て整数である。

### Sample Explanation 1

この例では $ 3 $ 番目、$ 4 $ 番目、$ 5 $ 番目のテーマ案がテーマとして選ばれる可能性があります。

### Sample Explanation 2

この例では $ 4 $ 番目、$ 5 $ 番目のテーマ案がテーマとして選ばれる可能性があります。 得票数が最大であるようなテーマ案が複数ある場合、いずれのテーマ案もテーマとして選ばれる可能性があることに注意してください。