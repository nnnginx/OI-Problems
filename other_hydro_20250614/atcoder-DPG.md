## 题目描述
[problemUrl]: https://atcoder.jp/contests/dp/tasks/dp_g

$ N $ 頂点 $ M $ 辺の有向グラフ $ G $ があります。 頂点には $ 1,\ 2,\ \ldots,\ N $ と番号が振られています。 各 $ i $ ($ 1\ \leq\ i\ \leq\ M $) について、$ i $ 番目の有向辺は頂点 $ x_i $ から $ y_i $ へ張られています。 $ G $ は**有向閉路を含みません**。

$ G $ の有向パスのうち、最長のものの長さを求めてください。 ただし、有向パスの長さとは、有向パスに含まれる辺の本数のことです。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ $ : $ $ x_M $ $ y_M $

## 输出格式
$ G $ の有向パスのうち、最長のものの長さを出力せよ。

## 题目大意
求**有向无环图**上的最长路长度。  

长度为路径上边的数量。

```input1
4 5
1 2
1 3
3 2
2 4
3 4
```

```output1
3
```

```input2
6 3
2 3
4 5
5 6
```

```output2
2
```

```input3
5 8
5 3
2 3
2 4
5 2
5 1
1 4
4 3
1 3
```

```output3
3
```

## 提示
### 制約

- 入力はすべて整数である。
- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ x_i,\ y_i\ \leq\ N $
- ペア $ (x_i,\ y_i) $ はすべて相異なる。
- $ G $ は**有向閉路を含まない**。

### Sample Explanation 1

次図の赤い有向パスが最長です。 ![](https://img.atcoder.jp/dp/longest_0_muffet.png)

### Sample Explanation 2

次図の赤い有向パスが最長です。 ![](https://img.atcoder.jp/dp/longest_1_muffet.png)

### Sample Explanation 3

例えば、次図の赤い有向パスが最長です。 ![](https://img.atcoder.jp/dp/longest_2_muffet.png)

