# AT_abc307_a [ABC307A] Weekly Records

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc307/tasks/abc307_a

高橋君は $ N $ 週間の間、自分が歩いた歩数を記録しました。$ i $ 日目に歩いた歩数は $ A_i $ でした。

各週に高橋君が歩いた歩数の合計を求めてください。  
 より正確には、$ 1 $ 週目( $ 1 $ 日目から $ 7 $ 日目まで)の $ 7 $ 日間の歩数の合計、$ 2 $ 週目( $ 8 $ 日目から $ 14 $ 日目まで)の $ 7 $ 日間の歩数の合計、……をそれぞれ求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_{7N} $

## 输出格式

$ i $ 週目に歩いた歩数を $ B_i $ とする。$ B_1,B_2,\ldots,B_N $ をこの順に空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
1000 2000 3000 4000 5000 6000 7000 2000 3000 4000 5000 6000 7000 8000
```

### 输出 #1

```
28000 35000
```

## 输入输出样例 #2

### 输入 #2

```
3
14159 26535 89793 23846 26433 83279 50288 41971 69399 37510 58209 74944 59230 78164 6286 20899 86280 34825 34211 70679 82148
```

### 输出 #2

```
314333 419427 335328
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10 $
- $ 0\ \leq\ A_i\ \leq\ 10^5 $
- 入力は整数
 
### Sample Explanation 1

高橋君は $ 1 $ 週目に $ 1000+2000+3000+4000+5000+6000+7000=28000 $ 歩あるき、$ 2 $ 週目に $ 2000+3000+4000+5000+6000+7000+8000=35000 $ 歩あるきました。