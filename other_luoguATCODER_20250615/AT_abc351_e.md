# AT_abc351_e [ABC351E] Jump Distance Sum

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc351/tasks/abc351_e

座標平面上に $ N $ 個の点 $ P_1,P_2,\ldots,P_N $ があり、点 $ P_i $ の座標は $ (X_i,Y_i) $ です。  
$ 2 $ つの点 $ A,B $ の距離 $ \text{dist}(A,B) $ を次のように定義します。

> 最初、ウサギが点 $ A $ にいる。  
> $ (x,y) $ にいるウサギは $ (x+1,y+1) $, $ (x+1,y-1) $, $ (x-1,y+1) $, $ (x-1,y-1) $ のいずれかに $ 1 $ 回のジャンプで移動することができる。  
> 点 $ A $ から点 $ B $ まで移動するために必要なジャンプの回数の最小値を $ \text{dist}(A,B) $ として定義する。  
> ただし、何度ジャンプを繰り返しても点 $ A $ から点 $ B $ まで移動できないとき、$ \text{dist}(A,B)=0 $ とする。

$ \displaystyle\sum_{i=1}^{N-1}\displaystyle\sum_{j=i+1}^N\ \text{dist}(P_i,P_j) $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ X_1 $ $ Y_1 $ $ X_2 $ $ Y_2 $ $ \vdots $ $ X_N $ $ Y_N $

## 输出格式

$ \displaystyle\sum_{i=1}^{N-1}\displaystyle\sum_{j=i+1}^N\ \text{dist}(P_i,P_j) $ の値を整数で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
0 0
1 3
5 6
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5
0 5
1 7
2 9
3 8
4 6
```

### 输出 #2

```
11
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 2\times\ 10^5 $
- $ 0\leq\ X_i,Y_i\leq\ 10^8 $
- $ i\neq\ j $ ならば $ (X_i,Y_i)\neq\ (X_j,Y_j) $
- 入力はすべて整数

### Sample Explanation 1

$ P_1,P_2,P_3 $ の座標はそれぞれ $ (0,0) $, $ (1,3) $, $ (5,6) $ です。 $ P_1 $ から $ P_2 $ へはウサギは $ (0,0)\to\ (1,1)\to\ (0,2)\to\ (1,3) $ と $ 3 $ 回で移動でき、$ 2 $ 回以下では $ P_1 $ から $ P_2 $ まで移動できないため、 $ \text{dist}(P_1,P_2)=3 $ です。 $ P_1 $ から $ P_3 $ および $ P_2 $ から $ P_3 $ へはウサギは移動できないため、$ \text{dist}(P_1,P_3)=\text{dist}(P_2,P_3)＝0 $ となります。 よって、答えは $ \displaystyle\sum_{i=1}^{2}\displaystyle\sum_{j=i+1}^3\text{dist}(P_i,P_j)=\text{dist}(P_1,P_2)+\text{dist}(P_1,P_3)+\text{dist}(P_2,P_3)=3+0+0=3 $ となります。