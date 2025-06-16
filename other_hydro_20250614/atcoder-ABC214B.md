## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc214/tasks/abc214_b

$ a+b+c\ \leq\ S $ かつ $ a\ \times\ b\ \times\ c\ \leq\ T $ を満たす非負整数の組 $ (a,b,c) $ はいくつありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式
条件を満たす非負整数の組 $ (a,b,c) $ の個数を出力せよ。

## 题目大意
输入两个非负整数 $s,t$ ，请编程输出满足 $a+b+c≤s$ 以及 $a×b×c≤t$ 的由非负整数构成的三元组 $(a,b,c)$ 的数量。

```input1
1 0
```

```output1
4
```

```input2
2 5
```

```output2
10
```

```input3
10 10
```

```output3
213
```

```input4
30 100
```

```output4
2471
```

## 提示
### 制約

- $ 0\ \leq\ S\ \leq\ 100 $
- $ 0\ \leq\ T\ \leq\ 10000 $
- $ S,\ T $ は整数である。

### Sample Explanation 1

条件を満たす非負整数の組 $ (a,b,c) $ は $ (0,0,0),\ (0,0,1),\ (0,1,0),\ (1,0,0) $ の $ 4 $ つです。

