# AT_abc203_c [ABC203C] Friends and Travel costs

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc203/tasks/abc203_c

$ 10^{100}+1 $ 個の村があり、それぞれ村 $ 0 $, 村 $ 1 $, $ \ldots $, 村 $ 10^{100} $ と番号がついています。  
 $ 0 $ 以上 $ 10^{100}-1 $ 以下の全ての整数 $ i $ について、村 $ i $ で $ 1 $ 円を払う事で村 $ (i+1) $ に移動することができます。 それ以外の移動方法はありません。

太郎君は初め $ K $ 円を持った状態で村 $ 0 $ におり、その後、可能な限り大きな番号の村まで進もうとします。  
 太郎君には $ N $ 人の友達がいます。$ i $ 人目の友達は村 $ A_i $ にいて、太郎君が村 $ A_i $ に着いたときに $ B_i $ 円を太郎君に渡します。  
 太郎君が最終的にたどり着く村の番号を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ B_1 $ $ : $ $ A_N $ $ B_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3
2 1
5 10
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5 1000000000
1 1000000000
2 1000000000
3 1000000000
4 1000000000
5 1000000000
```

### 输出 #2

```
6000000000
```

## 输入输出样例 #3

### 输入 #3

```
3 2
5 5
2 1
2 2
```

### 输出 #3

```
10
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ K\ \leq\ 10^9 $
- $ 1\ \leq\ A_i\ \leq\ 10^{18} $
- $ 1\ \leq\ B_i\ \leq\ 10^9 $
- 入力は全て整数である。

### Sample Explanation 1

太郎君は以下のように動きます: - 村 $ 0 $ から村 $ 1 $ へ $ 1 $ 円払って移動する。所持金は $ 2 $ 円となる。 - 村 $ 1 $ から村 $ 2 $ へ $ 1 $ 円払って移動する。所持金は $ 1 $ 円となる。 - 村 $ 2 $ で $ 1 $ 人目の友達から $ 1 $ 円受け取り、所持金は $ 2 $ 円となる。 - 村 $ 2 $ から村 $ 3 $ へ $ 1 $ 円払って移動する。所持金は $ 1 $ 円となる。 - 村 $ 3 $ から村 $ 4 $ へ $ 1 $ 円払って移動する。所持金は $ 0 $ 円となり、この村には友達もいないため村 $ 4 $ で止まる。 よって、 $ 4 $ を出力します。

### Sample Explanation 2

答えが $ 32 $ bit 整数に収まらないことがある事に注意してください。

### Sample Explanation 3

同じ村に複数の友達がいる可能性もあります。