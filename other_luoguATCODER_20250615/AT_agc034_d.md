# AT_agc034_d [AGC034D] Manhattan Max Matching

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc034/tasks/agc034_d

すぬけくんは、二次元平面上に赤いボールと青いボールを置いて遊んでいます。

すぬけくんはまず、赤いボールを置く操作を $ N $ 回行いました。 $ i $ 回目の操作では、座標 $ (RX_i,RY_i) $ に $ RC_i $ 個の赤いボールを置きました。 すぬけくんは次に、青いボールを置く操作を $ N $ 回行いました。 $ i $ 回目の操作では、座標 $ (BX_i,BY_i) $ に $ BC_i $ 個の青いボールを置きました。 ここで、すぬけくんが置いた赤いボールの個数の総和と青いボールの個数の総和は等しいです。 つまり、$ \sum_{i=1}^{N}\ RC_i\ =\ \sum_{i=1}^{N}\ BC_i $ です。 以後、この値を $ S $ とおきます。

すぬけくんはこれから、赤いボールと青いボールのペアを $ S $ 個作ろうとしています。 どのボールも、ちょうど $ 1 $ つのペアに属するようにします。 ここで、座標 $ (rx,ry) $ にある赤いボールと座標 $ (bx,by) $ にある青いボールのペアのスコアを、 $ |rx-bx|\ +\ |ry-by| $ と定義します。

すぬけくんは、ペアのスコアの総和を最大化したいです。 すぬけくんのために、ペアのスコアの総和の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ RX_1 $ $ RY_1 $ $ RC_1 $ $ RX_2 $ $ RY_2 $ $ RC_2 $ $ \vdots $ $ RX_N $ $ RY_N $ $ RC_N $ $ BX_1 $ $ BY_1 $ $ BC_1 $ $ BX_2 $ $ BY_2 $ $ BC_2 $ $ \vdots $ $ BX_N $ $ BY_N $ $ BC_N $

## 输出格式

ペアのスコアの総和の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
0 0 1
3 2 1
2 2 1
5 0 1
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
3
0 0 1
2 2 1
0 0 2
1 1 1
1 1 1
3 3 2
```

### 输出 #2

```
16
```

## 输入输出样例 #3

### 输入 #3

```
10
582463373 690528069 8
621230322 318051944 4
356524296 974059503 6
372751381 111542460 9
392867214 581476334 6
606955458 513028121 5
882201596 791660614 9
250465517 91918758 3
618624774 406956634 6
426294747 736401096 5
974896051 888765942 5
726682138 336960821 3
715144179 82444709 6
599055841 501257806 6
390484433 962747856 4
912334580 219343832 8
570458984 648862300 6
638017635 572157978 10
435958984 585073520 7
445612658 234265014 6
```

### 输出 #3

```
45152033546
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 0\ \leq\ RX_i,RY_i,BX_i,BY_i\ \leq\ 10^9 $
- $ 1\ \leq\ RC_i,BC_i\ \leq\ 10 $
- $ \sum_{i=1}^{N}\ RC_i\ =\ \sum_{i=1}^{N}\ BC_i $
- 入力される値はすべて整数である。

### Sample Explanation 1

座標 $ (0,0) $ に置いてある赤いボールと座標 $ (2,2) $ に置いてある青いボールをペアにすると、 そのスコアは $ |0-2|\ +\ |0-2|=4 $ です。 また、座標 $ (3,2) $ に置いてある赤いボールと座標 $ (5,0) $ に置いてある青いボールをペアにすると、 そのスコアは $ |3-5|\ +\ |2-0|=4 $ です。 この $ 2 $ つのペアを作ると、スコアの総和は $ 8 $ になり、これが最大です。

### Sample Explanation 2

同じ座標に複数回操作を行うこともあります。