# AT_arc105_c [ARC105C] Camels and Bridge

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc105/tasks/arc105_c

$ 1 $ から $ N $ の番号がついた $ N $ 頭のラクダがいます。

ラクダ $ i $ の体重は $ w_i $ です。

あなたはラクダたちに隊列を組ませ、$ M $ 個のパーツからなる橋を渡らせようとしています。

あなたは橋を渡る前にラクダたちの隊列を決め(番号の昇順となる必要はありません)、ラクダどうしを任意の非負の実数の間隔で並ばせることができます。 ラクダたちはこの決められた間隔を保って橋を渡ります。

橋の $ i $ 番目のパーツは長さ $ l_i $ で耐荷重は $ v_i $ です。 パーツ内部(両端を除く)にいるラクダたちの体重の総和が $ v_i $ より大きくなると、橋は崩落してしまいます。

橋が崩落しないようにラクダたちを渡らせることが可能かどうかを判定し、可能ならばそのときの先頭のラクダと末尾のラクダの距離としてありうる値の最小値を求めてください。 これは整数になることが証明できるので、整数で出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ w_1 $ $ w_2 $ $ \cdots $ $ w_N $ $ l_1 $ $ v_1 $ $ \vdots $ $ l_M $ $ v_M $

## 输出格式

どのようにしても橋が崩落してしまう場合、`-1` を出力せよ。 そうでない場合、橋が崩落しないようにラクダたちを渡らせるときの先頭のラクダと末尾のラクダの距離としてありうる値の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2
1 4 2
10 4
2 6
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
2 1
12 345
1 1
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
8 1
1 1 1 1 1 1 1 1
100000000 1
```

### 输出 #3

```
700000000
```

## 输入输出样例 #4

### 输入 #4

```
8 20
57 806 244 349 608 849 513 857
778 993
939 864
152 984
308 975
46 860
123 956
21 950
850 876
441 899
249 949
387 918
34 965
536 900
875 889
264 886
583 919
88 954
845 869
208 963
511 975
```

### 输出 #4

```
3802
```

## 说明/提示

### 制約

- 与えられる入力は全て整数
- $ 2\ \leq\ N\ \leq\ 8 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ w_i,l_i,v_i\ \leq\ 10^8 $

### Sample Explanation 1

\- 例えば、先頭から順に $ 1,3,2 $ の順番に並べ、ラクダどうしの間隔をそれぞれ $ 0,10 $ にすることで橋が崩落しないようにラクダたちを渡らせることが可能です。 - パーツ $ 1 $ ではラクダ $ 1,3 $ あるいはラクダ $ 2 $ のみがパーツの内部にいる状態が起こります。どちらもパーツの内部にいるラクダたちの体重の総和がパーツ $ 1 $ の耐荷重である $ 4 $ 以下のため、橋が崩落することはありません。 - パーツ $ 2 $ ではラクダ $ 1,3 $ あるいはラクダ $ 2 $ のみがパーツの内部にいる状態が起こります。どちらもパーツの内部にいるラクダたちの体重の総和がパーツ $ 1 $ の耐荷重である $ 6 $ 以下のため、橋が崩落することはありません。 - ラクダどうしの間隔が $ 0 $ でもよいこと、パーツの内部はパーツの両端を含まないことに注意してください。

### Sample Explanation 2

\- どのようにしても橋が崩落してしまう場合は `-1` を出力してください。