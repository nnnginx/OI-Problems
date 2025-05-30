## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc274/tasks/abc274_c

あなたはアメーバの観察記録をつけました。

最初 $ 1 $ 匹のアメーバがおり、番号は $ 1 $ です。

観察記録は時系列順に $ N $ 個あり、$ i $ 番目の観察記録は「番号 $ A_i $ のアメーバが分裂して消滅し、新たに $ 2 $ 匹のアメーバが生まれ、それらにそれぞれ $ 2i,2i+1 $ と番号をつけた」というものです。  
 このとき、アメーバ $ A_i $ を アメーバ $ 2i,2i+1 $ の親と呼びます。

各 $ k=1,\ldots,2N+1 $ について、アメーバ $ k $ から何代親を遡るとアメーバ $ 1 $ になるか求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式
$ 2N+1 $ 行出力せよ。$ k $ 行目にはアメーバ $ k $ から何代親を遡るとアメーバ $ 1 $ になるかを出力せよ。

## 题目大意
你有一棵树，起始时仅有一个根节点 $1$。

接下来有 $n$ 次操作。对于第 $i$ 次操作，编号为 $A_i$ 的节点将会增加两个儿子，编号分别为 $2i$ 和 $2i + 1$。

对于 $i=1,2,...,2N+1$，求节点 $i$ 到根节点的距离。

```input1
2
1 2
```

```output1
0
1
1
2
2
```

```input2
4
1 3 5 2
```

```output2
0
1
1
2
2
3
3
2
2
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- 観察記録は矛盾していない。すなわち
  - $ 1\leq\ A_i\ \leq\ 2i-1 $
  - $ A_i $ は相異なる整数

### Sample Explanation 1

アメーバ $ 1 $ からアメーバ $ 2,3 $ が生まれ、アメーバ $ 2 $ からアメーバ $ 4,5 $ が生まれました。 - アメーバ $ 1 $ は $ 0 $ 代遡るとアメーバ $ 1 $ になります。 - アメーバ $ 2 $ は $ 1 $ 代遡るとアメーバ $ 1 $ になります。 - アメーバ $ 3 $ は $ 1 $ 代遡るとアメーバ $ 1 $ になります。 - アメーバ $ 4 $ は $ 1 $ 代遡るとアメーバ $ 2 $ になり、$ 2 $ 代遡るとアメーバ $ 1 $ になります。 - アメーバ $ 5 $ は $ 1 $ 代遡るとアメーバ $ 2 $ になり、$ 2 $ 代遡るとアメーバ $ 1 $ になります。

