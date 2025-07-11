# AT_abc166_c [ABC166C] Peaks

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc166/tasks/abc166_c

AtCoder丘陵には $ N $ 個の展望台があり、展望台 $ i $ の標高は $ H_i $ です。 また、異なる展望台どうしを結ぶ $ M $ 本の道があり、道 $ j $ は展望台 $ A_j $ と展望台 $ B_j $ を結んでいます。

展望台 $ i $ が良い展望台であるとは、展望台 $ i $ から一本の道を使って辿り着けるどの展望台よりも展望台 $ i $ の方が標高が高いことをいいます。 展望台 $ i $ から一本の道を使って辿り着ける展望台が存在しない場合も、展望台 $ i $ は良い展望台であるといいます。

良い展望台がいくつあるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ H_1 $ $ H_2 $ $ ... $ $ H_N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ : $ $ A_M $ $ B_M $

## 输出格式

良い展望台の数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
1 2 3 4
1 3
2 3
2 4
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6 5
8 6 9 1 2 1
1 3
4 2
4 3
4 6
4 6
```

### 输出 #2

```
3
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 1\ \leq\ H_i\ \leq\ 10^9 $
- $ 1\ \leq\ A_i,B_i\ \leq\ N $
- $ A_i\ \neq\ B_i $
- 同じ展望台の組を結ぶ道が複数あることもある。
- 入力中の値はすべて整数である。

### Sample Explanation 1

\- 展望台 $ 1 $ から一本の道を使って辿り着ける展望台は展望台 $ 3 $ ですが、展望台 $ 1 $ の標高は展望台 $ 3 $ の標高より高くないため、展望台 $ 1 $ は良い展望台ではありません。 - 展望台 $ 2 $ から一本の道を使って辿り着ける展望台は展望台 $ 3 $ と展望台 $ 4 $ ですが、展望台 $ 2 $ の標高は展望台 $ 3 $ の標高より高くないため、展望台 $ 2 $ は良い展望台ではありません。 - 展望台 $ 3 $ から一本の道を使って辿り着ける展望台は展望台 $ 1 $ と展望台 $ 2 $ ですが、展望台 $ 3 $ の標高は展望台 $ 1 $ の標高より高く、かつ展望台 $ 2 $ の標高より高いため、展望台 $ 3 $ は良い展望台です。 - 展望台 $ 4 $ から一本の道を使って辿り着ける展望台は展望台 $ 2 $ ですが、展望台 $ 4 $ の標高は展望台 $ 2 $ の標高より高いため、展望台 $ 4 $ は良い展望台です。 展望台 $ 3 $ と展望台 $ 4 $ が良い展望台なので、良い展望台の数は $ 2 $ です。