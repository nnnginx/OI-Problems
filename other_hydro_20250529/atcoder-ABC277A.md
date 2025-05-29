## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc277/tasks/abc277_a

$ (1,2,…,N) $ を並び替えた数列 $ P $ と整数 $ X $ が与えられます。 数列 $ P $ の $ i $ 番目の項の値は $ P_i $ です。 $ P_k\ =\ X $ を満たす $ k $ を出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ P_1 $ $ P_2 $ $ \ldots $ $ P_N $

## 输出格式
答えを出力せよ。

## 题目大意
【题面翻译】

给定一个长度为 $n$ 的排列 $P$，以及一个数字 $X$（$1 \le X \le n$）。求排列中，第几位的元素为 $X$。

translated by [liangbowen](https://www.luogu.com.cn/user/367488).

```input1
4 3
2 3 1 4
```

```output1
2
```

```input2
5 2
3 5 1 4 2
```

```output2
5
```

```input3
6 6
1 2 3 4 5 6
```

```output3
6
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ X\ \leq\ N $
- $ P $ は $ (1,2,…,N) $ を並び替えてできる数列
- 入力はすべて整数
 
### Sample Explanation 1

$ P\ =\ (2,3,1,4) $ なので、$ P_2\ =\ 3 $ です。したがって、$ 2 $ を出力します。

