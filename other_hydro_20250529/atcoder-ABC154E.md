## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc154/tasks/abc154_e

$ 1 $ 以上 $ N $ 以下の整数であって、 $ 10 $ 進法で表したときに、$ 0 $ でない数字がちょうど $ K $ 個あるようなものの個数を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
条件を満たす数の個数を出力せよ。

## 题目大意
给定两个正整数 $N,K$，求出 $1$ 到 $N$ 中有多少个正整数，满足它的非零数位个数和恰好等于 $K$。  

$1 \le N < 10^{100}$，$1 \le K \le3$。

```input1
100
1
```

```output1
19
```

```input2
25
2
```

```output2
14
```

```input3
314159
2
```

```output3
937
```

```input4
9999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
3
```

```output4
117879300
```

## 提示
### 制約

- $ 1\ \leq\ N\ <\ 10^{100} $
- $ 1\ \leq\ K\ \leq\ 3 $

### Sample Explanation 1

条件を満たす数は次の $ 19 $ 個です。 - $ 1,2,3,4,5,6,7,8,9,10,20,30,40,50,60,70,80,90,100 $

### Sample Explanation 2

条件を満たす数は次の $ 14 $ 個です。 - $ 11,12,13,14,15,16,17,18,19,21,22,23,24,25 $

