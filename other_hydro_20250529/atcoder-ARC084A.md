## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc077/tasks/arc084_a

今年もすぬけ祭の季節がやってきました。りんごさんは、まず手始めにすぬけ君召喚の儀式を執り行おうと思っています。 儀式には祭壇が必要で、祭壇は上部、中部、下部の $ 3 $ つのカテゴリーのパーツ $ 1 $ つずつからなります。

祭壇の $ 3 $ カテゴリーのパーツがそれぞれ $ N $ 個ずつあります。 $ i $ 個目の上部のパーツのサイズは $ A_i $ 、$ i $ 個目の中部のパーツのサイズは $ B_i $ 、$ i $ 個目の下部のパーツのサイズは $ C_i $ です。

祭壇を作るにあたっては、中部のパーツのサイズは上部のパーツのサイズより真に大きく、下部のパーツのサイズは中部のパーツのサイズより 真に大きくなければなりません。逆に、この条件を満たす任意の $ 3 $ つのピースを組み合わせて祭壇を作ることができます。

りんごさんが作ることのできる祭壇は何種類あるでしょうか。ただし、$ 2 $ つの祭壇が異なるとは、上部、中部、下部に使われるピースのうち 少なくとも $ 1 $ つが異なることを言います。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ ... $ $ A_N $ $ B_1 $ $ ... $ $ B_N $ $ C_1 $ $ ... $ $ C_N $

## 输出格式
りんごさんが作ることのできる祭壇の種類数を出力せよ。

## 题目大意
## 题面：
今年也到了滑雪节的季节。仪式上必须有祭坛，祭坛由上部、中部、下部3个类别的部件各1个构成。


祭坛的3分类的零件各有N个。i上部零件的大小Ai，第i个中部零件的大小Bi，第i个下部的零件的大小是Ci。


在制作祭坛的时候，中部的零件的尺寸要比上部的零件的尺寸大，下部的零件的尺寸必须比中部的零件的尺寸大。反过来说，满足此条件的任意三块组合就可建造祭坛。


问：能做的祭坛有几种？（当上部、中部、下部使用的块中至少有一个是不同的时候，两个祭坛视为不同。）


## 样例1说明：
可以建造以下三种祭坛：


上部使用第1个，中部第1个，下部第1个零件的祭坛


上部使用第1个，中部第1个，下部第2个零件的祭坛


上部使用第1个，中部第2个，下部第2个零件的祭坛

```input1
2
1 5
2 4
3 6
```

```output1
3
```

```input2
3
1 1 1
2 2 2
3 3 3
```

```output2
27
```

```input3
6
3 14 159 2 6 53
58 9 79 323 84 6
2643 383 2 79 50 288
```

```output3
87
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^9(1\leq\ i\leq\ N) $
- $ 1\ \leq\ B_i\ \leq\ 10^9(1\leq\ i\leq\ N) $
- $ 1\ \leq\ C_i\ \leq\ 10^9(1\leq\ i\leq\ N) $
- 入力は全て整数である

### Sample Explanation 1

次の $ 3 $ 種類の祭壇があります。 - 上部に $ 1 $ 個目、中部に $ 1 $ 個目、下部に $ 1 $ 個目のパーツを使った祭壇 - 上部に $ 1 $ 個目、中部に $ 1 $ 個目、下部に $ 2 $ 個目のパーツを使った祭壇 - 上部に $ 1 $ 個目、中部に $ 2 $ 個目、下部に $ 2 $ 個目のパーツを使った祭壇

