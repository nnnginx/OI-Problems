## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc156/tasks/abc156_b

整数 $ N $ を $ K $ 進数で表したとき、何桁になるかを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式
整数 $ N $ を $ K $ 進数で表したとき、何桁になるかを出力せよ。

## 题目大意
给定两个整数 $ N $ 和 $ K $ ,请求出整数 $ N $ 在 $ K $ 进制下的位数。

```input1
11 2
```

```output1
4
```

```input2
1010101 10
```

```output2
7
```

```input3
314159265 3
```

```output3
18
```

## 提示
### 注記

$ K $ 進表記については、[Wikipedia「位取り記数法」](https://ja.wikipedia.org/wiki/%E4%BD%8D%E5%8F%96%E3%82%8A%E8%A8%98%E6%95%B0%E6%B3%95)を参照してください。

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 10^9 $
- $ 2\ \leq\ K\ \leq\ 10 $

### Sample Explanation 1

$ 11 $ を $ 2 $ 進数で表記すると `1011` です。

