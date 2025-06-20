# AT_abc011_3 [ABC011C] 123引き算

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc011/tasks/abc011_3

あなたは、友人から、一人用のゲームを紹介されました。

最初に、数字 $ N $ が与えられます。 $ 1 $ , $ 2 $ , $ 3 $ の中から好きな数字を選び、 与えられた数字に対し、引き算を行う、という処理を行うことできます。

この処理は $ 100 $ 回まで行うことが可能であり、最終的に数字を $ 0 $ にすることが目標のゲームです。

しかし、計算途中でなってはいけないNG数字が $ 3 $ つ与えられており、 この数字に一時的にでもなってしまった瞬間、このゲームは失敗となります。 NG数字が $ N $ と同じ場合も失敗となります。

NG数字が $ N $ と同じ場合について、正しい判定が行われていませんでした。リジャッジを行いました。

あなたは、このゲームが、目標達成可能なゲームとなっているか調べたいです。

目標達成可能な場合は`YES`、そうでない場合は`NO`と出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ NG_1 $ $ NG_2 $ $ NG_3 $

- $ 1 $ 行目には、最初に与えられる数字 $ N\ (1\ ≦\ N\ ≦\ 300) $ が与えられる。
- $ 2 $ 行目には、 $ 1 $ 番目のNG数字 $ NG_1\ (1\ ≦\ NG_1\ ≦\ 300) $ が与えられる。
- $ 3 $ 行目には、 $ 2 $ 番目のNG数字 $ NG_2\ (1\ ≦\ NG_2\ ≦\ 300) $ が与えられる。
- $ 4 $ 行目には、 $ 3 $ 番目のNG数字 $ NG_3\ (1\ ≦\ NG_3\ ≦\ 300) $ が与えられる。

## 输出格式

目標達成可能な場合は`YES`、そうでない場合は`NO`を $ 1 $ 行で出力せよ。出力の末尾にも改行をいれること。

## 输入输出样例 #1

### 输入 #1

```
2
1
7
15
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
5
1
4
2
```

### 输出 #2

```
YES
```

## 输入输出样例 #3

### 输入 #3

```
300
57
121
244
```

### 输出 #3

```
NO
```

## 说明/提示

### Sample Explanation 1

$ 2 $ を $ 1 $ 回引くことにより、 $ 0 $ を作ることが出来ます。

### Sample Explanation 2

最初に $ 2 $ を引き、次に $ 3 $ を引くことで、$ 5 $ → $ 3 $ → $ 0 $ と変化し、目標を達成することが出来ます。

### Sample Explanation 3

$ 100 $ 回連続で $ 3 $ を引かなければ、目標を達成することはできません。 しかし、 $ 3 $ だけを引き続けていると、途中でNG数字である $ 57 $ になってしまいます。