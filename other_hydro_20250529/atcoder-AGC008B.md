## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc008/tasks/agc008_b

$ N $ 個のマスが横一列に並んでいます。 左から $ i $ 番目のマスには整数 $ a_i $ が書かれています。

最初、すべてのマスは白色です。 すぬけ君は次の操作を好きな回数だけ繰り返します。

- 連続する $ K $ 個のマスを選び、それらすべてを白く塗るか、それらすべてを黒く塗る。 このとき、各マスの色は上書きされる。

すぬけ君が操作を終えた後、黒いマスに書かれた整数の総和がスコアになります。 考えられるスコアの最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式
考えられるスコアの最大値を出力せよ。

## 题目大意
## 题目描述
有 $ N $ 个格子排成一列，从左起第 $ i $ 个格子中写着整数 $ a_i $。

开始时，每个格子被涂成白色。snuke君将重复进行以下操作。

- 选择连续的 $ K $ 个格子，将它们全部涂成白色或全部涂成黑色。此操作将会覆盖掉格子原来的颜色。

snuke 君希望在操作完成后，黑色格子中整数的和最大。请求出此最大值。

## 数据范围
- $ 1 \leq N \leq 10^5 $
- $ 1 \leq K \leq N $
- $ a_i $ 是整数。
- $ |a_i| \leq 10^9 $

## 输入
输入按以下形式：
```
N K
a1 a2 … aN
```

## 输出
输出能得到的黑色格子中整数总和的最大值。

## 样例

样例见原题面。

## 样例解释
### 样例 1 解释
将从左数的第 $ 2,3,4 $ 格涂黑。
### 样例 2 解释
以下是其中一种最优解：
- 将从左数的第 $ 1,2 $ 格涂黑。
- 将从左数的第 $ 3,4 $ 格涂黑。
- 将从左数的第 $ 2,3 $ 格涂白。

```input1
5 3
-10 10 -10 10 -10
```

```output1
10
```

```input2
4 2
10 -10 -10 10
```

```output2
20
```

```input3
1 1
-10
```

```output3
0
```

```input4
10 5
5 -4 -5 -8 -4 7 2 -4 0 7
```

```output4
17
```

## 提示
### 制約

- $ 1\ <\ =N\ <\ =10^5 $
- $ 1\ <\ =K\ <\ =N $
- $ a_i $ は整数である。
- $ |a_i|\ <\ =10^9 $

### Sample Explanation 1

左から $ 2 $, $ 3 $, $ 4 $ 番目のマスを黒く塗ればよいです。

### Sample Explanation 2

たとえば、次のように操作を行えばよいです。 - 左から $ 1 $, $ 2 $ 番目のマスを黒く塗る。 - 左から $ 3 $, $ 4 $ 番目のマスを黒く塗る。 - 左から $ 2 $, $ 3 $ 番目のマスを白く塗る。

