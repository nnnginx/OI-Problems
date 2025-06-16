# AT_pakencamp_2021_day2_f Fraction

## 题目描述

[problemUrl]: https://atcoder.jp/contests/pakencamp-2021-day2/tasks/pakencamp_2021_day2_f

正整数 $ N $ が与えられます。

$ \dfrac{a}{b}\ <\ \dfrac{c}{d}\ <\ \dfrac{e}{f} $ を満たす整数の組 $ (a,b,c,d,e,f)\ (1\ \le\ a,b,c,d,e,f\ \le\ N) $ のうち、$ \dfrac{e}{f}-\dfrac{a}{b} $ が最小になるものを一つ構築してください。

この問題の制約下で、$ \dfrac{a}{b}\ <\ \dfrac{c}{d}\ <\ \dfrac{e}{f} $ を満たす整数の組 $ (a,b,c,d,e,f) $ は必ず存在します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

答えとなる $ (a,b,c,d,e,f) $ をこの順に空白区切りで出力せよ。解が複数存在する場合、そのいずれを出力しても正解となる。

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
1 2 1 1 2 1
```

## 输入输出样例 #2

### 输入 #2

```
3
```

### 输出 #2

```
1 3 1 2 2 3
```

## 说明/提示

### 制約

- $ 2\ \le\ N\ \le\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

$ \dfrac{1}{2}\ <\ \dfrac{1}{1}\ <\ \dfrac{2}{1} $ です。 `1 2 2 2 2 1` と答えても正解となります。

### Sample Explanation 2

原案: \[turtle0123\\\_\\\_\](https://atcoder.jp/users/turtle0123\_\_)