# AT_pakencamp_2019_day3_c カラオケ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/pakencamp-2019-day3/tasks/pakencamp_2019_day3_c

$ 1,\ 2,\ ...,\ N $ と番号づけられている $ N $ 人の生徒から成るグループが，「全国統一カラオケコンテスト」に出場することとなりました．

このコンテストで歌える曲は，曲 $ 1 $，曲 $ 2 $，...，曲 $ M $ の $ M $ 曲あります．また，番号 $ i $ の生徒が曲 $ j $ を歌うと，必ず $ A_{i,\ j} $ 点を取ります．

さて，コンテストのルールは，以下のようになります．

- $ M $ 曲の中から $ 2 $ つの曲を選ぶ．（それぞれ $ T_1 $ と $ T_2 $ とする．）
- それぞれの生徒が，曲 $ T_1 $ と曲 $ T_2 $ の両方を歌う．
- 各生徒の得点は，その生徒が歌った $ 2 $ つの曲の点数のうち高い方となる．
- グループの得点は，生徒 $ 1,\ 2,\ ...,\ N $ の得点の合計となる．

そのとき，グループの得点として考えられる最大の値を求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられます．

> $ N $ $ M $ $ A_{1,\ 1} $ $ A_{1,\ 2} $ $ A_{1,\ 3} $ ... $ A_{1,\ M} $ $ A_{2,\ 1} $ $ A_{2,\ 2} $ $ A_{2,\ 3} $ ... $ A_{2,\ M} $ $ A_{3,\ 1} $ $ A_{3,\ 2} $ $ A_{3,\ 3} $ ... $ A_{3,\ M} $ : $ A_{N,\ 1} $ $ A_{N,\ 2} $ $ A_{N,\ 3} $ ... $ A_{N,\ M} $

## 输出格式

グループの得点として考えられる最大の値を，整数で出力してください．

## 输入输出样例 #1

### 输入 #1

```
1 2
80 84
```

### 输出 #1

```
84
```

## 输入输出样例 #2

### 输入 #2

```
3 4
37 29 70 41
85 69 76 50
53 10 95 100
```

### 输出 #2

```
250
```

## 输入输出样例 #3

### 输入 #3

```
8 2
31000000 41000000
59000000 26000000
53000000 58000000
97000000 93000000
23000000 84000000
62000000 64000000
33000000 83000000
27000000 95000000
```

### 输出 #3

```
581000000
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 2\ \leq\ M\ \leq\ 100 $
- $ 0\ \leq\ A_{i,\ j}\ \leq\ 100\ 000\ 000 $
- 入力はすべて整数

### 部分点

この問題はいくつかの小課題に分けられ，その小課題のすべてのテストケースに正解した場合に「この小課題に正解した」とみなされます．  
 提出したソースコードの得点は，正解した小課題の点数の合計となります．

1. (10 点) $ N\ =\ 1 $，$ M\ =\ 2 $．
2. (25 点) $ M\ =\ 2 $．
3. (35 点) $ N\ =\ 1 $．
4. (30 点) 追加の制約はない．

### 注意

**この問題におけるカラオケは，通常のカラオケとは違い，$ 100\ 000\ 000 $ 点までの点数が出ることがあります．**  
**また，点数は必ず整数となり，$ 314159.265 $ 点のような整数でない点数が出ることはありません．**

### Sample Explanation 1

生徒 $ 1 $ の曲 $ 1 $ の点数は $ 80 $ 点，曲 $ 2 $ の点数は $ 84 $ 点です．よって，生徒 $ 1 $ の得点は $ 84 $ 点となります． また，グループには $ 1 $ 人しか生徒がいないため，グループの得点は $ 84 $ 点となります． なお，この入力例は，小課題 $ 1 $ の制約を満たします．

### Sample Explanation 2

例えば，このグループが曲 $ 1 $ と $ 3 $ を歌った場合： - 生徒 $ 1 $ : 曲 $ 1 $ の点数は $ 37 $ 点，曲 $ 3 $ の点数は $ 70 $ 点．よって，この生徒の得点は $ 70 $ 点． - 生徒 $ 2 $ : 曲 $ 1 $ の点数は $ 85 $ 点，曲 $ 3 $ の点数は $ 76 $ 点．よって，この生徒の得点は $ 85 $ 点． - 生徒 $ 3 $ : 曲 $ 1 $ の点数は $ 53 $ 点，曲 $ 3 $ の点数は $ 95 $ 点．よって，この生徒の得点は $ 95 $ 点． よって，このグループの得点は $ 70+85+95=250 $ 点となります．グループの得点を $ 251 $ 点以上にする方法はありません．

### Sample Explanation 3

この入力例は，小課題 $ 2 $ の制約を満たします．