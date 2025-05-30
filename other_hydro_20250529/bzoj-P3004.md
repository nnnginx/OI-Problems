## 题目描述

Alice家里有一盏很大的吊灯。所谓吊灯，就是由很多个灯泡组成。只有一个灯泡是挂在天花板上的，剩下的灯泡都是挂在其他的灯泡上的。也就是说，整个吊灯实际上类似于一棵树。其中编号为 $ 1 $ 的灯泡是挂在天花板上的，剩下的灯泡都是挂在编号小于自己的灯泡上的。

现在，Alice想要办一场派对，她想改造一下这盏吊灯，将灯泡换成不同的颜色。她希望相同颜色的灯泡都
是相连的，并且每一种颜色的灯泡个数都是相同的。

Alice希望你能告诉她，总共有哪些方案呢？

Alice是一个贪心的孩子，如果她发现方案不够多，或者太多了，就会很不高兴，于是她会尝试调整。对于编号为 $ x(x \neq 1) $ 的灯泡，如果原来是挂在编号为 $ f[x] $ 的灯泡上，那么Alice会把第 $ x $ 个灯泡挂到第  $ ( f[x] + 19940105 )
\mod (x-1) + 1 $  个灯泡上。

由于九在古汉语中表示极大的数，于是，Alice决定只调整 $ 9 $ 次。对于原始状态和每一次调整过的状态，Alice希望你依次告诉她每种状态下有哪些方案。

## 输入格式

第一行一个整数 $ n $，表示灯泡的数量。

接下来一行，有 $ n-1 $ 个整数 $ U_i $，第 $ i $ 个数字表示第 $ i+1 $ 个灯泡挂在了 $ U_i $ 个的下面。保证编号为 $ 1 $ 的灯泡是挂在天
花板上的。数字之间用逗号```,```隔开且最后一个数字后面没有逗号。

## 输出格式

对于 $ 10 $ 种状态下的方案，需要按照顺序依次输出。

对于每一种状态，需要先输出单独的一行，表示状态编号，如样例所示。

之后若干行，每行 $ 1 $ 个整数，表示划分方案中每种颜色的灯泡个数，按升序输出。

## 样例输入

```
6
1,2,3,4,5
```

## 样例输出

```
Case #1:
1
2
3
6
Case #2:
1
2
6
Case #3:
1
3
6
Case #4:
1
3
6
Case #5:
1
3
6
Case #6:
1
2
6
Case #7:
1
2
3
6
Case #8:
1
6
Case #9:
1
2
6
Case #10:
1
3
6
```

## 数据规模与约定

对于 $100\%$ 的数据， $ n \leq 1.2 \times 10^6 $。
