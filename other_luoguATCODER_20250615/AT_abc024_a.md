# AT_abc024_a [ABC024A] 動物園

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc024/tasks/abc024_a

ABC動物園は、高橋王国で一番の人気を誇る動物園です。

ABC動物園の入場料の設定は以下のようになっています。

- 子供 $ 1 $ 人あたり $ A $ 円
- 大人 $ 1 $ 人あたり $ B $ 円
- 合計人数が $ K $ 人以上の団体は $ 1 $ 人あたり $ C $ 円引き

今、子供 $ S $ 人、大人 $ T $ 人からなる団体が入場しようとしています。 この団体が合計で支払わなければならない入場料を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ K $ $ S $ $ T $

- $ 1 $ 行目には入場料の値段設定を表す $ 4 $ つの整数 $ A,\ B,\ C,\ K $ が空白区切りで与えられる。各変数の意味は問題文と同様である。各変数は以下の制約を満たす。 
  - $ 0\ ≦\ C\ ≦\ A\ ≦\ B\ ≦\ 1,000 $
  - $ 0\ ≦\ K\ ≦\ 100 $
- $ 2 $ 行目には団体が含む子供と大人の人数を表す $ 2 $ つの整数 $ S(0\ ≦\ S\ ≦\ 100),\ T(0\ ≦\ T\ ≦\ 100) $ が空白区切りで与えられる。

## 输出格式

団体が合計で支払わなければならない入場料を $ 1 $ 行に出力せよ。 出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
100 200 50 20
40 10
```

### 输出 #1

```
3500
```

## 输入输出样例 #2

### 输入 #2

```
400 1000 400 21
10 10
```

### 输出 #2

```
14000
```

## 输入输出样例 #3

### 输入 #3

```
400 1000 400 20
10 10
```

### 输出 #3

```
6000
```

## 说明/提示

### Sample Explanation 1

子供 $ 40 $ 人、大人 $ 10 $ 人の団体です。合計人数が $ 20 $ 人以上なので一人あたり $ 50 $ 円割引、つまり全体で $ 2500 $ 円割引されます。

### Sample Explanation 2

団体の合計人数が $ 21 $ 人以上ではないので割引は適応されません。