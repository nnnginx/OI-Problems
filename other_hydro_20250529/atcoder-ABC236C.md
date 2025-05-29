## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc236/tasks/abc236_c

AtCoder 鉄道のとある路線には $ N $ 個の駅が存在し、始点から終点に向かって $ i\ \,\ (1\ \leq\ i\ \leq\ N) $ 番目の駅の名前は $ S_i $ です。

普通列車は全ての駅に止まりますが、急行列車は全ての駅に止まるとは限りません。具体的には、急行列車は $ M\ \,\ (M\ \leq\ N) $ 個の駅にのみ止まり、$ j\ \,\ (1\ \leq\ j\ \leq\ M) $ 番目に止まる駅の名前は $ T_j $ です。  
 ただし、$ T_1\ =\ S_1 $ かつ $ T_M\ =\ S_N $、すなわち急行列車は始点と終点の両方に止まることが保証されます。

$ N $ 個の駅それぞれについて、その駅に急行列車が止まるかどうか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ S_1 $ $ \ldots $ $ S_N $ $ T_1 $ $ \ldots $ $ T_M $

## 输出格式
$ N $ 行出力せよ。$ i\ \,\ (1\ \leq\ i\ \leq\ N) $ 行目には、始点から終点に向かって $ i $ 番目の駅に急行列車が止まるなら `Yes`、そうでないなら `No` と出力せよ。

## 题目大意
# 题目简述
有 $N$ 个站点按顺序排在一条直线上，第 $i(1\le i\le N)$ 个站点是 $S_i$。

有一辆火车会在其中的 $M(M\le N)$ 个站点停下,第 $j(1\le j\le M)$ 个停下来的站点的名字是 $T_j$。

保证 $T_1=S_1,T_M=S_N$。

对于 $N$ 个站点中的每一个，请判断火车是否在该站点停下。

# 数据范围
>$2≤M≤N≤10^5$
>
>$N,M$ 为整数
>
>$S_i（1 \le i \le N）$是一个长度在 $[1, 10]$ 之间的小写英文字符串。
>
>$S_i\ne S_j（i \ne j）$
>
>$T_1=S_1,T_M=S_N$
>
>$(T_1,\dots, T_M)$ 是通过移除 $(S_1,\dots, S_N)$ 中的若干个站点且不改变原有顺序得到的。
# 输入格式
第一行包含整数 $N,M$。

第二行包含 $N$ 个字符串 $S_1,S_2,\dots,S_N$。

第三行包含 $M$ 个字符串 $T_1,T_2,\dots,T_M$。

# 输出格式
输出 $N$ 行。如果第 $i(1 \le i \le N)$ 个站点在火车的经停站点列表中，输出 `Yes`，否则输出 `No`。

Translated by @[tianbiandeshenghuo11](/user/752485)

```input1
5 3
tokyo kanda akiba okachi ueno
tokyo akiba ueno
```

```output1
Yes
No
Yes
No
Yes
```

```input2
7 7
a t c o d e r
a t c o d e r
```

```output2
Yes
Yes
Yes
Yes
Yes
Yes
Yes
```

## 提示
### 制約

- $ 2\ \leq\ M\ \leq\ N\ \leq\ 10^5 $
- $ N,\ M $ は整数
- $ S_i\ \,\ (1\ \leq\ i\ \leq\ N) $ は英小文字のみからなる $ 1 $ 文字以上 $ 10 $ 文字以下の文字列
- $ S_i\ \neq\ S_j\ \,\ (i\ \neq\ j) $
- $ T_1\ =\ S_1 $ かつ $ T_M\ =\ S_N $
- $ (T_1,\ \dots,\ T_M) $ は $ (S_1,\ \dots,\ S_N) $ から $ 0 $ 個以上の文字列を選んで取り除き、残った文字列を元の順序で並べることで得られる

### Sample Explanation 2

急行列車が全ての駅に止まることもあります。

