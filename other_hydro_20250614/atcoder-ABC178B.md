## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc178/tasks/abc178_b

整数 $ a,b,c,d $ が与えられます。 $ a\ \leq\ x\ \leq\ b,\ c\leq\ y\ \leq\ d $ を満たす整数 $ x,y $ について、$ x\ \times\ y $ の最大値はいくつですか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ c $ $ d $

## 输出格式
答えを出力せよ。

## 题目大意
整数 $a,b,c,d,x,y$ 满足： $a≤x≤b$ ， $c≤y≤d$ 。给出 $a,b,c,d$ ，求出 $x×y$ 的最大值。

```input1
1 2 1 1
```

```output1
2
```

```input2
3 5 -4 -2
```

```output2
-6
```

```input3
-1000000000 0 -1000000000 0
```

```output3
1000000000000000000
```

## 提示
### 制約

- $ -10^9\ \leq\ a\ \leq\ b\ \leq\ 10^9 $
- $ -10^9\ \leq\ c\ \leq\ d\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

$ x=1,y=1 $ のとき $ x\ \times\ y=1 $、$ x=2,y=1 $ のとき $ x\ \times\ y=2 $ であるため、答えは $ 2 $ です。

### Sample Explanation 2

答えが負になることもあります。

