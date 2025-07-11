# AT_abc371_f [ABC371F] Takahashi in Narrow Road

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc371/tasks/abc371_f

東西に続く道があり、道の上には $ N $ 人の高橋くんがいます。 道は原点と呼ばれる点から東西に十分長く続いています。

$ i $ 番目 $ (1\leq\ i\leq\ N) $ の高橋くんは、はじめ原点から東に $ X\ _\ i $ メートル進んだところにいます。

高橋くんたちは道の上を東西に動くことができます。 具体的には、次の移動を好きなだけ行うことができます。

- 高橋くんを一人選ぶ。**移動する先に他の高橋くんがいない場合**、選んだ高橋くんを $ 1 $ メートル東に、もしくは西に移動させる。

高橋くんたちには合計 $ Q $ 個の用事があり、$ i $ 個目 $ (1\leq\ i\leq\ Q) $ の用事は次の形式で表されます。

- $ T\ _\ i $ 番目の高橋くんが座標 $ G\ _\ i $ に到着する。

$ Q $ 個の用事を先頭から順にすべて完了するために必要な移動回数の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ X\ _\ 1 $ $ X\ _\ 2 $ $ \ldots $ $ X\ _\ N $ $ Q $ $ T\ _\ 1 $ $ G\ _\ 1 $ $ T\ _\ 2 $ $ G\ _\ 2 $ $ \vdots $ $ T\ _\ Q $ $ G\ _\ Q $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
10 20 30 40 50
4
3 45
4 20
1 35
2 60
```

### 输出 #1

```
239
```

## 输入输出样例 #2

### 输入 #2

```
8
0 1 2 3 4 5 6 100000000
6
1 100000000
8 0
1 100000000
8 4
1 100000000
5 21006578
```

### 输出 #2

```
4294967297
```

## 输入输出样例 #3

### 输入 #3

```
12
1558 3536 3755 3881 4042 4657 5062 7558 7721 8330 8542 9845
8
9 1694
7 3296
12 5299
5 5195
5 5871
1 2491
8 1149
8 2996
```

### 输出 #3

```
89644
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq2\times10\ ^\ 5 $
- $ 0\leq\ X\ _\ 1\lt\ X\ _\ 2\lt\dotsb\lt\ X\ _\ N\leq10\ ^\ 8 $
- $ 1\leq\ Q\leq2\times10\ ^\ 5 $
- $ 1\leq\ T\ _\ i\leq\ N\ (1\leq\ i\leq\ Q) $
- $ 0\leq\ G\ _\ i\leq10\ ^\ 8\ (1\leq\ i\leq\ Q) $
- 入力はすべて整数

### Sample Explanation 1

高橋くんたちの最適な行動は以下のようになります（それぞれの高橋くんの座標は正確に描かれているとは限りません）。 !\[\](https://img.atcoder.jp/abc371/2ebef79b440e6dae3115bb518fccfb5f.png) それぞれの用事では、高橋くんたちは次のように移動しています。 - $ 4 $ 番目の高橋くんが $ 6 $ 回東に進み、$ 3 $ 番目の高橋くんが $ 15 $ 回東に進む。 - $ 2 $ 番目の高橋くんが $ 2 $ 回西に進み、$ 3 $ 番目の高橋くんが $ 26 $ 回西に進み、$ 4 $ 番目の高橋くんが $ 26 $ 回西に進む。 - $ 4 $ 番目の高橋くんが $ 18 $ 回東に進み、$ 3 $ 番目の高橋くんが $ 18 $ 回東に進み、$ 2 $ 番目の高橋くんが $ 18 $ 回東に進み、$ 1 $ 番目の高橋くんが $ 25 $ 回東に進む。 - $ 5 $ 番目の高橋くんが $ 13 $ 回東に進み、$ 4 $ 番目の高橋くんが $ 24 $ 回東に進み、$ 3 $ 番目の高橋くんが $ 24 $ 回東に進み、$ 2 $ 番目の高橋くんが $ 24 $ 回東に進む。 高橋くんたちの移動回数の合計は $ 21+54+79+85=239 $ 回となります。 移動回数の合計を $ 238 $ 回以下としてすべての用事を完了することはできないため、`239` を出力してください。

### Sample Explanation 2

途中で一部の高橋くんが原点より西側や、原点より $ 10\ ^\ 8+1 $ メートル以上東に進んだところに移動する必要がある場合があることに注意してください。 また、答えが $ 2\ ^\ {32} $ を超える場合があることに注意してください。