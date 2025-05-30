## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf16-exhibition/tasks/codefestival_2016_ex_b

高橋王国の通貨の単位は「ミョン」です。 高橋王国では、$ 10 $ 冪 ($ 1,\ 10,\ 100,\ 1000,\ ... $) ミョンの硬貨が用いられています。

エキシビ商店では $ N $ 個の品物が売られています。 商品 $ i\ (1≦i≦N) $ の値段は $ A_i $ ミョンです。

高橋くんはエキシビ商店に行き、$ N $ 個の商品のうち $ 1 $ 個以上 $ N $ 個以下の商品を選んで買おうとしています。 高橋くんはお釣りが嫌いなので、どのように買い物をしてもお釣りが出ないように、財布の中に入れる硬貨を選びたいと思っています。 また、財布が重くなるのも困るので、硬貨の枚数をできるだけ少なくしたいと思っています。

このとき、高橋くんが財布に入れる必要のある硬貨の枚数の最小値を求めて下さい。ただし、財布に入れるための硬貨が足りなくなることは無いものとします。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式
どのように買い物をしてもお釣りが出ないように財布の中に入れる必要のある硬貨の枚数の最小値を出力せよ。

```input1
3
43 24 37
```

```output1
16
```

```input2
5
49735011221 970534221705 411566391637 760836201000 563515091165
```

```output2
105
```

## 提示
### 制約

- $ 1≦N≦20,000 $
- $ 1≦A_i≦10^{12} $

### Sample Explanation 1

支払う金額として考えられるものは、$ 24,\ 37,\ 43,\ 61,\ 67,\ 80,\ 104 $ の $ 7 $ 通りです。 $ 1 $ ミョン硬貨が $ 7 $ 枚、$ 10 $ ミョン硬貨が $ 8 $ 枚、$ 100 $ ミョン硬貨が $ 1 $ 枚あれば、これらをお釣りなく支払うことが出来ます。

