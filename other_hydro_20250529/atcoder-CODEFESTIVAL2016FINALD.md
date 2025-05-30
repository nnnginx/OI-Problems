## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf16-final/tasks/codefestival_2016_final_d

高橋君は $ N $ 枚のカードで遊んでいます。

$ i $ 枚目のカードには整数 $ X_i $ が書かれています。

高橋君は以下のいずれかの条件を満たすカードの$ 2 $ 枚組をなるべくたくさん作ろうとしています。

- $ 2 $ 枚のカードに書かれた整数が同じである。
- $ 2 $ 枚のカードに書かれた整数の和が $ M $ の倍数である。

高橋君が作ることの出来る組の個数の最大値を求めなさい。

ただし、$ 1 $ 枚のカードを複数の組で使うことはできないものとします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ X_1 $ $ X_2 $ $ ... $ $ X_N $

## 输出格式
高橋君が作ることの出来る組の個数の最大値を出力せよ。

## 题目大意
## 题意：

已知高桥君有 $n$ 张卡片，每一张卡牌上有一个整数 $x_i$。高桥君想要以以下两种条件合并两张卡牌：

$1$：两张卡牌上的整数相等。

$2$：两张卡牌上的整数之和是 $m$ 的倍数。

求出高桥君可以组成多少组的组数最大值。

注：一张卡牌不能在多组中使用。


------------

## 输入格式：

第一行两个整数 $n$ 和 $m$。

接下来一行，有 $n$ 个整数：$x_1$，$x_2...x_n$。


------------
## 输出格式：

输出组数的最大值。



------------
## 数据范围与约定：

$2\le n \le 10^5$，$1\le m \le 10^5$，$1 \le x_i \le 10^5$。

```input1
7 5
3 1 4 1 5 9 2
```

```output1
3
```

```input2
15 10
1 5 6 10 11 11 11 20 21 25 25 26 99 99 99
```

```output2
6
```

## 提示
### 制約

- $ 2≦N≦10^5 $
- $ 1≦M≦10^5 $
- $ 1≦X_i≦10^5 $

### Sample Explanation 1

$ (3,2),\ (1,4),\ (1,9) $ の $ 3 $ 組を作ることが出来ます。 $ (3,2),\ (1,1) $ のように組を作ることもできますが、これでは組の個数が最大とならないことに注意してください。

