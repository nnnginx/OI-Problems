## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc113/tasks/arc113_a

正の整数 $ K $ が与えられます。正の整数の $ 3 $ つ組 $ (A,B,C) $ であって、$ ABC\leq\ K $ なるものの個数を求めてください。 ただし、$ A,B,C $ の順番が異なるだけの組も異なる組として数えます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式
正の整数の $ 3 $ つ組 $ (A,B,C) $ であって、$ ABC\leq\ K $ なるものの個数を出力せよ。

## 题目大意
给出一个正整数 $K$，问有多少三元组 $(a,b,c)$ 满足 $a\times b\times c\le K$？

```input1
2
```

```output1
4
```

```input2
10
```

```output2
53
```

```input3
31415
```

```output3
1937281
```

## 提示
### 制約

- $ 1\leq\ K\leq\ 2\times\ 10^5 $
- $ K $ は整数である

### Sample Explanation 1

$ (1,1,1),(1,1,2),(1,2,1),(2,1,1) $ が条件を満たします。

