# AT_agc019_e [AGC019E] Shuffle and Swap

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc019/tasks/agc019_e

$ 0 $ と $ 1 $ からなる同じ長さの二つの文字列 $ A\ =\ A_1\ A_2\ ...\ A_n $ と $ B\ =\ B_1\ B_2\ ...\ B_n $ があります。 $ A,\ B $ に含まれる $ 1 $ の個数は等しいです。

あなたは次のアルゴリズムによって $ A $ を変化させることにしました。

- $ a_1 $, $ a_2 $, ..., $ a_k $ を、$ A $ で $ 1 $ が出現する位置の添字とする。
- $ b_1 $, $ b_2 $, ..., $ b_k $ を、$ B $ で $ 1 $ が出現する位置の添字とする。
- $ a,\ b $ の要素をそれぞれ無作為に並び替える。これらの無作為な並び替えは一様かつ独立である。
- $ 1 $ から $ k $ までの各 $ i $ に対して、順に $ A_{a_i} $ と $ A_{b_i} $ の値を入れ替える。

この手順のあと、文字列 $ A,\ B $ が一致する確率を $ P $ とします。

さらに、$ Z\ =\ P\ \times\ (k!)^2 $ とします。明らかに、$ Z $ は整数です。

$ Z $ を $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

## 输出格式

$ Z $ を $ 998244353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1010
1100
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
01001
01001
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
101010
010101
```

### 输出 #3

```
36
```

## 输入输出样例 #4

### 输入 #4

```
1101011011110
0111101011101
```

### 输出 #4

```
932171449
```

## 说明/提示

### 制約

- $ 1\ \leq\ |A|\ =\ |B|\ \leq\ 10,000 $
- $ A,\ B $ は $ 0 $ と $ 1 $ からなる。
- $ A,\ B $ に含まれる $ 1 $ の個数は等しい。
- $ A,\ B $ には $ 1 $ が少なくとも一つ含まれる。

### 部分点

- $ 1\ \leq\ |A|\ =\ |B|\ \leq\ 500 $ を満たすデータセットに正解すると、$ 1200 $ 点が与えられる。

### Sample Explanation 1

最初の二つのステップで、$ a\ =\ [1,\ 3] $, $ b\ =\ [1,\ 2] $ となります。$ a,\ b $ の要素を無作為に並び替えたあとの結果としてありうるものは次の $ 4 $ つです。 - $ a\ =\ [1,\ 3] $, $ b\ =\ [1,\ 2] $。はじめ $ A\ =\ 1010 $。$ A_1 $ と $ A_1 $ の入れ替え後 $ A\ =\ 1010 $。$ A_3 $ と $ A_2 $ の入れ替え後 $ A\ =\ 1100 $。 - $ a\ =\ [1,\ 3] $, $ b\ =\ [2,\ 1] $。はじめ $ A\ =\ 1010 $。$ A_1 $ と $ A_2 $ の入れ替え後 $ A\ =\ 0110 $。$ A_3 $ と $ A_1 $ の入れ替え後 $ A\ =\ 1100 $。 - $ a\ =\ [3,\ 1] $, $ b\ =\ [1,\ 2] $。はじめ $ A\ =\ 1010 $。$ A_3 $ と $ A_1 $ の入れ替え後 $ A\ =\ 1010 $。$ A_1 $ と $ A_2 $ の入れ替え後 $ A\ =\ 0110 $。 - $ a\ =\ [3,\ 1] $, $ b\ =\ [2,\ 1] $。はじめ $ A\ =\ 1010 $。$ A_3 $ と $ A_2 $ の入れ替え後 $ A\ =\ 1100 $。$ A_1 $ と $ A_1 $ の入れ替え後 $ A\ =\ 1100 $。 この $ 4 $ つの結果のうち、$ 3 $ つで $ A\ =\ B $ となっています。よって、$ P\ =\ 3 $ / $ 4 $ であり、$ Z\ =\ 3 $ となります。

### Sample Explanation 2

$ A $ の要素の入れ替えによって $ A $ が変化することはなく、したがって必ず $ A\ =\ B $ となります。

### Sample Explanation 3

三回の $ A $ の要素の入れ替えがどのように起こっても、$ A $ に含まれる $ 1 $ は適切な位置に移動します。