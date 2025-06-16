## 题目描述
[problemUrl]: https://atcoder.jp/contests/yahoo-procon2019-qual/tasks/yahoo_procon2019_qual_a

$ 1 $ 以上 $ N $ 以下の異なる整数を、差が $ 1 $ の整数をともに選ばないように $ K $ 個選ぶことができるか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
整数を $ K $ 個選ぶことができるなら `YES` を、そうでないなら `NO` を出力せよ。

## 题目大意
给定 $2$ 个数 $N$ 和 $K$ 。问能否在 $1-N$ 这 $N$ 个数（包括 $N$ ）中选择 $K$ 个不同的整数使它们的差不等于 $1$ 。

$1\leq N,K\leq 100$
且 $N$ 和 $K$ 均为整数。

```input1
3 2
```

```output1
YES
```

```input2
5 5
```

```output2
NO
```

```input3
31 10
```

```output3
YES
```

```input4
10 90
```

```output4
NO
```

## 提示
### 制約

- $ 1\leq\ N,K\leq\ 100 $
- $ N,K $ は整数である

### Sample Explanation 1

$ 1,3 $ を選べばよいです。

