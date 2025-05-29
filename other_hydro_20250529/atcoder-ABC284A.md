## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc284/tasks/abc284_a

$ N $ 個の文字列 $ S_1,S_2,\ldots,S_N $ がこの順番で与えられます。

$ S_N,S_{N-1},\ldots,S_1 $ の順番で出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式
$ N $ 行出力せよ。 $ i\ (1\leq\ i\ \leq\ N) $ 行目には、$ S_{N+1-i} $ を出力せよ。

## 题目大意
给定 $N$ 个字符串，$S_1,S_2 ... S_n$。

将这 $N$ 个字符串反序输出（即 $S_n,S_{n-1} ... S_1$），中间以一个换行隔开。

数据保证 $ 1 \leq N \leq 10$。

translate by [ChrisWangZi](https://www.luogu.com.cn/user/637180)

```input1
3
Takahashi
Aoki
Snuke
```

```output1
Snuke
Aoki
Takahashi
```

```input2
4
2023
Year
New
Happy
```

```output2
Happy
New
Year
2023
```

## 提示
### 制約

- $ 1\leq\ N\ \leq\ 10 $
- $ N $ は整数
- $ S_i $ は英小文字、英大文字、数字からなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列
 
### Sample Explanation 1

$ N=3 $、$ S_1= $ `Takahashi`、$ S_2= $ `Aoki`、$ S_3= $ `Snuke` です。 よって、`Snuke`、`Aoki`、`Takahashi` の順で出力します。

### Sample Explanation 2

与えられる文字列が数字を含むこともあります。

