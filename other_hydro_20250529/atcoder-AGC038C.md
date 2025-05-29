## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc038/tasks/agc038_c

長さ $ N $ の整数列 $ A_0,A_1,\cdots,A_{N-1} $ があります。 次式の値を求めてください。

- $ \sum_{i=0}^{N-2}\ \sum_{j=i+1}^{N-1}\ \mathrm{lcm}(A_i,A_j) $

ここで、$ \mathrm{lcm}(x,y) $ は、$ x $ と $ y $ の最小公倍数を意味します。 なお、答えは非常に大きくなることがあるので、$ 998244353 $ で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_0\ A_1\ \cdots\ A_{N-1} $

## 输出格式
$ \sum_{i=0}^{N-2}\ \sum_{j=i+1}^{N-1}\ \mathrm{lcm}(A_i,A_j) $ の値を $ 998244353 $ で割ったあまりを出力せよ。

## 题目大意
- 给定一个长度为 $N$ 的数列 $A_1, A_2, A_3, \ldots, A_N$。
- 请你求出 $\sum_{i=1}^{N}\sum_{j=i+1}^{N}\mathrm{lcm}(A_i,A_j)$ 的值模 $998244353$ 的结果。
- $1 \leq N \leq 2 \times 10^5$，$1 \leq A_i \leq 10^6$。

```input1
3
2 4 6
```

```output1
22
```

```input2
8
1 2 3 4 6 8 12 12
```

```output2
313
```

```input3
10
356822 296174 484500 710640 518322 888250 259161 609120 592348 713644
```

```output3
353891724
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 200000 $
- $ 1\ \leq\ A_i\ \leq\ 1000000 $
- 入力される値はすべて整数である。

### Sample Explanation 1

$ \mathrm{lcm}(2,4)+\mathrm{lcm}(2,6)+\mathrm{lcm}(4,6)=4+6+12=22 $ です。

