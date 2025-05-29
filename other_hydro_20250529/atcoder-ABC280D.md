## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc280/tasks/abc280_d

$ 2 $ 以上の整数 $ K $ が与えられます。  
正の整数 $ N $ であって、$ N! $ が $ K $ の倍数となるようなもののうち最小のものを求めてください。

ただし、$ N! $ は $ N $ の階乗を表し、問題の制約下で、そのような $ N $ が必ず存在することが証明できます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式
$ N! $ が $ K $ の倍数となるような最小の正整数 $ N $ を出力せよ。

## 题目大意
- 给出一个数 $k$，求一个数 $n$，要求 $n!$ 是 $k$ 的倍数，输出 $n$ 的最小值。
- $k\le10^{12}$

translated by @[PineappleSummer](https://www.luogu.com.cn/user/880187)。

```input1
30
```

```output1
5
```

```input2
123456789011
```

```output2
123456789011
```

```input3
280
```

```output3
7
```

## 提示
### 制約

- $ 2\leq\ K\leq\ 10^{12} $
- $ K $ は整数

### Sample Explanation 1

\- $ 1!=1 $ - $ 2!=2\times\ 1=2 $ - $ 3!=3\times\ 2\times\ 1=6 $ - $ 4!=4\times\ 3\times\ 2\times\ 1=24 $ - $ 5!=5\times\ 4\times\ 3\times\ 2\times\ 1=120 $ より、$ N! $ が $ 30 $ の倍数となる最小の正整数 $ N $ は $ 5 $ です。よって、$ 5 $ を出力します。

