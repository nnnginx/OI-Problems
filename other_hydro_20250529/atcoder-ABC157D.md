## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc157/tasks/abc157_d

とあるSNSに、人 $ 1 $ 、人 $ 2 $、 $ \cdots $、人 $ N $ が登録しています。

この $ N $ 人の間には、 $ M $ 組の「友達関係」と、 $ K $ 組の「ブロック関係」が存在します。

$ i\ =\ 1,\ 2,\ \cdots,\ M $ について、人 $ A_i $ と人 $ B_i $ は友達関係にあります。この関係は双方向的です。

$ i\ =\ 1,\ 2,\ \cdots,\ K $ について、人 $ C_i $ と人 $ D_i $ はブロック関係にあります。この関係は双方向的です。

以下の $ 4 $ つの条件が満たされるとき、人 $ a $ は人 $ b $ の「友達候補」であると定義します。

- $ a\ \neq\ b $ である。
- 人 $ a $ と人 $ b $ はブロック関係に無い。
- 人 $ a $ と人 $ b $ は友達関係に無い。
- $ 1 $ 以上 $ N $ 以下の整数から成るある数列 $ c_0,\ c_1,\ c_2,\ \cdots,\ c_L $ が存在し、$ c_0\ =\ a $ であり、 $ c_L\ =\ b $ であり、 $ i\ =\ 0,\ 1,\ \cdots,\ L\ -\ 1 $ について、人 $ c_i $ と人 $ c_{i+1} $ は友達関係にある。

人 $ i\ =\ 1,\ 2,\ ...\ N $ について、友達候補の数を答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ B_1 $ $ \vdots $ $ A_M $ $ B_M $ $ C_1 $ $ D_1 $ $ \vdots $ $ C_K $ $ D_K $

## 输出格式
答えを空白区切りで順に出力せよ。

## 题目大意
### 题目大意

某平台上有 $N$ 名用户，其中，有 $M$ 对用户是互相关注的，有 $K$ 对用户是互相拉黑的。

当用户 $i$ 和用户 $j$ 满足以下条件时，用户 $j$ 就是用户 $i$ 的“推荐用户”：

+ 用户 $i$ 可以与 用户 $j$ 通过若干对用户的互相关注关系连接起来。（比如用户 1 与用户 2，用户 2 与用户 3 都互相关注，则用户 1 和 用户 3 就可以通过他们的关系连接起来）
+ 用户 $i$ 与用户 $j$ 没有互相关注或互相拉黑。

求每位用户的“推荐用户”的数量。

数据保证不会存在一对用户既互相关注又互相拉黑。

### 输入格式

第一行输入三个正整数 $N,M,K$；

接下来 $M$ 行，每行两个正整数 $A_i,B_i$，表示一对互相关注的用户；

再接下来 $K$ 行，每行两个正整数 $C_i,D_i$，表示一对互相拉黑的用户。

### 输出格式

输出用空格隔开的 $N$ 个整数，第 $i$ 个数表示用户 $i$ 的“推荐用户”的数量。

### 说明

$2 \le N \le 10^5, 0 \le M,K \le 10^5$。

翻译 by @CarroT1212

```input1
4 4 1
2 1
1 3
3 2
3 4
4 1
```

```output1
0 1 0 1
```

```input2
5 10 0
1 2
1 3
1 4
1 5
3 2
2 4
2 5
4 3
5 3
4 5
```

```output2
0 0 0 0 0
```

```input3
10 9 3
10 1
6 7
8 2
2 5
8 4
7 3
10 9
6 4
5 8
2 6
7 5
3 1
```

```output3
1 3 5 4 3 3 3 3 1 0
```

## 提示
### 制約

- 入力は全て整数
- $ 2\ <\ =\ N\ <\ =\ 10^5 $
- $ 0\ \leq\ M\ \leq\ 10^5 $
- $ 0\ \leq\ K\ \leq\ 10^5 $
- $ 1\ \leq\ A_i,\ B_i\ \leq\ N $
- $ A_i\ \neq\ B_i $
- $ 1\ \leq\ C_i,\ D_i\ \leq\ N $
- $ C_i\ \neq\ D_i $
- $ (A_i,\ B_i)\ \neq\ (A_j,\ B_j)\ (i\ \neq\ j) $
- $ (A_i,\ B_i)\ \neq\ (B_j,\ A_j) $
- $ (C_i,\ D_i)\ \neq\ (C_j,\ D_j)\ (i\ \neq\ j) $
- $ (C_i,\ D_i)\ \neq\ (D_j,\ C_j) $
- $ (A_i,\ B_i)\ \neq\ (C_j,\ D_j) $
- $ (A_i,\ B_i)\ \neq\ (D_j,\ C_j) $

### Sample Explanation 1

人 $ 2 $ と人 $ 3 $ は友達関係にあり, 人 $ 3 $ と人 $ 4 $ は友達関係にあり, かつ人 $ 2 $ と人 $ 4 $ は友達関係にもブロック関係にもありませんから, 人 $ 4 $ は人 $ 2 $の友達候補です。 人 $ 1 $ と人 $ 3 $ は人 $ 2 $ の友達候補ではありませんから, 人 $ 2 $ の友達候補は $ 1 $ 人です。

### Sample Explanation 2

全ての人は他の全ての人と友達関係にありますが、友達候補は $ 0 $ 人です。

