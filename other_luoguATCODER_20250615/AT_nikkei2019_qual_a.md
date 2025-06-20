# AT_nikkei2019_qual_a Subscribers

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-qual/tasks/nikkei2019_qual_a

私たちは、新聞の購読に関する調査を行いました。 具体的には、調査の対象者 $ N $ 人に対し、それぞれ次の $ 2 $ つの質問を行いました。

- 質問 $ 1 $: あなたは新聞 X を購読しているか？
- 質問 $ 2 $: あなたは新聞 Y を購読しているか？

その結果、質問 $ 1 $ に対して「はい」と回答した人の数は $ A $ 人、質問 $ 2 $ に対して「はい」と回答した人の数は $ B $ 人でした。

このとき、調査の対象者のうち新聞 X, Y の両方を購読している人の数は最大で何人であり、また最小で何人であると考えられるでしょうか？

この問いに答えるプログラムを書いてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $

## 输出格式

両方の新聞を購読している人の数として考えられる最大の人数と最小の人数をこの順に、空白で区切って出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 3 5
```

### 输出 #1

```
3 0
```

## 输入输出样例 #2

### 输入 #2

```
10 7 5
```

### 输出 #2

```
5 2
```

## 输入输出样例 #3

### 输入 #3

```
100 100 100
```

### 输出 #3

```
100 100
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 0\ \leq\ A\ \leq\ N $
- $ 0\ \leq\ B\ \leq\ N $
- 入力される値はすべて整数である。

### Sample Explanation 1

この例では、調査の対象者 $ 10 $ 人のうち $ 3 $ 人が新聞 X を購読していると回答し、$ 5 $ 人が新聞 Y を購読していると回答しています。 このとき、両方の新聞を購読している人の数は最大で $ 3 $ 人、最小で $ 0 $ 人です。

### Sample Explanation 2

この例では、調査の対象者 $ 10 $ 人のうち $ 7 $ 人が新聞 X を購読していると回答し、$ 5 $ 人が新聞 Y を購読していると回答しています。 このとき、両方の新聞を購読している人の数は最大で $ 5 $ 人、最小で $ 2 $ 人です。