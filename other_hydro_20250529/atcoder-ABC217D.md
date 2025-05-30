## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc217/tasks/abc217_d

長さ $ L $ メートルの直線状の木材があります。  
 $ x\ =\ 1,\ 2,\ \dots,\ L\ -\ 1 $ に対して、木材の左端から $ x $ メートルの地点には目印として線 $ x $ が引かれています。

$ Q $ 個のクエリが与えられます。 $ i $ 番目のクエリは数の組 $ (c_i,\ x_i) $ によって表されます。  
 以下の説明に従ってクエリを $ i $ の昇順に処理してください。

- $ c_i\ =\ 1 $ のとき : 線 $ x_i $ がある地点で木材を $ 2 $ つに切る。
- $ c_i\ =\ 2 $ のとき : 線 $ x_i $ を含む木材を選び、その長さを出力する。

ただし $ c_i\ =\ 1,\ 2 $ の両方に対して、線 $ x_i $ はクエリを処理する時点で切られていないことが保証されます。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ L $ $ Q $ $ c_1 $ $ x_1 $ $ c_2 $ $ x_2 $ $ \vdots $ $ c_Q $ $ x_Q $

## 输出格式
$ c_i\ =\ 2 $ を満たすクエリの回数と等しい行数だけ出力せよ。 $ j $ 行目では $ j $ 番目のそのようなクエリに対する答えを出力せよ。

## 题目大意
给定一个长度为 $L$ 的序列 $[1,L]$ 和 $q$ 个询问。对于第 $i$ 次询问有一个 $c_i$ 和 $x_i$，如果 $c_i=1$，将 $x$ 点所在的区间 $[l,r]$ 分为 $[l,x]$ 和 $[x+1,r]$；如果 $c_i=2$，输出 $x$ 点所在区间的长度。

```input1
5 3
2 2
1 3
2 2
```

```output1
5
3
```

```input2
5 3
1 2
1 4
2 3
```

```output2
2
```

```input3
100 10
1 31
2 41
1 59
2 26
1 53
2 58
1 97
2 93
1 23
2 84
```

```output3
69
31
6
38
38
```

## 提示
### 制約

- $ 1\ \leq\ L\ \leq\ 10^9 $
- $ 1\ \leq\ Q\ \leq\ 2\ \times\ 10^5 $
- $ c_i\ =\ 1,\ 2 $ $ (1\ \leq\ i\ \leq\ Q) $
- $ 1\ \leq\ x_i\ \leq\ L\ -\ 1 $ $ (1\ \leq\ i\ \leq\ Q) $
- 全ての $ i $ $ (1\ \leq\ i\ \leq\ Q) $ に対して次が成り立つ: $ 1\ \leq\ j\ \lt\ i $ かつ $ (c_j,x_j)\ =\ (1,\ x_i) $ を満たす $ j $ は存在しない。
- 入力は全て整数である。

### Sample Explanation 1

$ 1 $ 番目のクエリ時点では木材は一度も切られていないので、線 $ 2 $ を含む木材の長さは $ 5 $ メートルです。よって $ 5 $ を出力します。 $ 2 $ 番目のクエリによって、木材は $ 3 $ メートルの木材と $ 2 $ メートルの木材に分割されます。 $ 3 $ 番目のクエリ時点では 線 $ 2 $ を含む木材の長さは $ 3 $ メートルなので、$ 3 $ を出力します。

