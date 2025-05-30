## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc168/tasks/abc168_e

$ N $ 匹のイワシが釣れました。$ i $ 匹目のイワシの美味しさは $ A_i $、香り高さは $ B_i $ です。

この中から $ 1 $ 匹以上のイワシを選んで同じクーラーボックスに入れますが、互いに仲が悪い $ 2 $ 匹を同時に選ぶことはできません。

$ i $ 匹目と $ j\ (\neq\ i) $ 匹目のイワシは、$ A_i\ \cdot\ A_j\ +\ B_i\ \cdot\ B_j\ =\ 0 $ を満たすとき(また、その時に限り)仲が悪いです。

イワシの選び方は何通りあるでしょう？答えは非常に大きくなる可能性があるので、$ 1000000007 $ で割ったあまりを出力してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ : $ $ A_N $ $ B_N $

## 输出格式
答えを $ 1000000007 $ で割ったあまりを出力せよ。

## 题目大意
## 题目描述

&emsp;你钓到了$ N $ 条沙丁鱼，第 $ i $ 条沙丁鱼有一个美味程度 $ A_i $ 和香味程度 $ B_i $ 。  
&emsp;因为吃不完这么多，所以需要把其中**一条以上**的沙丁鱼放进冰箱。不幸的是，由于它们之间有的关系不好，所以死了之后放在一起也会打架。
- 定义两条鱼 $(i,j)$ 之间的关系不好为：当且仅当 $ A_i\ \cdot\ A_j\ +\ B_i\ \cdot\ B_j\ =\ 0 $ 

为了不让它们打架，请输出可能的方案数，答案对 $ 1e9+7 $ 取模。

```input1
3
1 2
-1 1
2 -1
```

```output1
5
```

```input2
10
3 2
3 2
-1 1
2 -1
-3 -9
-8 12
7 7
8 1
8 2
8 4
```

```output2
479
```

## 提示
### 制約

- 入力はすべて整数
- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ -10^{18}\ \leq\ A_i,\ B_i\ \leq\ 10^{18} $

### Sample Explanation 1

条件を満たす選び方は以下の $ 5 $ 通りです。 - $ 1 $ 匹目 - $ 1,\ 2 $ 匹目 - $ 2 $ 匹目 - $ 2,\ 3 $ 匹目 - $ 3 $ 匹目

