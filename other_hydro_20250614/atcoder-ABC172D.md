## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc172/tasks/abc172_d

正整数 $ X $ に対し、$ X $ の正の約数の個数を $ f(X) $ とします。

正整数 $ N $ が与えられるので、$ \sum_{K=1}^N\ K\times\ f(K) $ を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
値 $ \sum_{K=1}^N\ K\times\ f(K) $ を出力せよ。

## 题目大意
### 题意翻译
- $f(x)$ 表示正整数 $x$ 的因数个数
- 现在给你一个正整数 $ N $ ，让你求出 $  \sum_{K=1}^N\ K\times\ f(K) $  。
----------

### 输入格式

- 共一行，第一行输入一个正整数 $N$ ，定义见题目描述

-------------

### 输出格式

- 共一行，输出 $ \sum_{K=1}^N\ K\times\ f(K) $ 的结果
- 最后别忘了输出回车

### 说明/提示
-  $ 1\ \leq\ N\ \leq\ 10^7 $
### 样例1说明：
- $f(1)=1 $ ,  $ f(2)=2 $ ,  $ f(3)=2 $ ,  $ f(4)=3 $ , 所以答案为  $ 1\times\ 1\ +\ 2\times\ 2\ +\ 3\times\ 2\ +\ 4\times\ 3\ =23 $ 。

 _Translated by qinmingze_

```input1
4
```

```output1
23
```

```input2
100
```

```output2
26879
```

```input3
10000000
```

```output3
838627288460105
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^7 $

### Sample Explanation 1

$ f(1)=1 $, $ f(2)=2 $, $ f(3)=2 $, $ f(4)=3 $ なので、答えは $ 1\times\ 1\ +\ 2\times\ 2\ +\ 3\times\ 2\ +\ 4\times\ 3\ =23 $ となります。

### Sample Explanation 3

オーバーフローに注意してください。

