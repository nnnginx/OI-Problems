# AT_arc039_a [ARC039A] A - B problem

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc039/tasks/arc039_a

高橋君は次のような問題を考えました。

- $ 3 $ 桁の整数 $ A $、$ B $ が与えられるので $ A\ -\ B $ を求める。

しかしあまりにも簡単すぎるので、ちょっと変更して次のような問題にしました。

- $ 3 $ 桁の整数 $ A $、$ B $ が与えられる。
- $ A $ と $ B $ のどちらかを $ 1 $ 桁だけ書き換えてもよい時の、$ A\ -\ B $ の答えになり得る整数の最大値を求める。

なお、一番上の桁が $ 0 $ であるような整数へと書き換えることはできません。 例えば $ 123 $ を $ 023 $ へと書き換えたりすることはできません。

高橋君は自信満々であなたへとこの問題を出題してきました。 ぜひ挑戦してみてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $

$ 1 $ 行に $ 2 $ つの整数 $ A(100\ ≦\ A\ ≦\ 999) $、$ B(100\ ≦\ B\ ≦\ 999) $ が空白区切りで与えられる。

## 输出格式

$ A $、$ B $ のどちらかを $ 1 $ 桁だけ書き換えてもよい時の、$ A\ -\ B $ の答えになり得る整数の最大値を $ 1 $ 行に出力せよ。出力は標準出力に行い、末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
567 234
```

### 输出 #1

```
733
```

## 输入输出样例 #2

### 输入 #2

```
999 100
```

### 输出 #2

```
899
```

## 输入输出样例 #3

### 输入 #3

```
100 999
```

### 输出 #3

```
-99
```

## 说明/提示

### Sample Explanation 1

$ A $ を $ 567 $ から $ 967 $ に書き換えれば $ A-B $ は $ 733 $ となり、この値が $ A-B $ の最大値となっています。

### Sample Explanation 2

どちらも書き換えない時に $ A-B $ が最大値となることもあります。

### Sample Explanation 3

答えは負になることもあります。