# AT_arc110_e [ARC110E] Shorten ABC

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc110/tasks/arc110_e

`A`, `B`, `C` からなる長さ $ N $ の文字列 $ S $ があります。

あなたは $ S $ に対して、以下の操作を $ 0 $ 回以上行うことができます。

- $ S_i\ \neq\ S_{i\ +\ 1} $ である $ i\ ~\ (1\ \leq\ i\ \leq\ |S|\ -\ 1) $ を選ぶ。$ S_i $ を $ S_i,\ S_{i\ +\ 1} $ のいずれとも（`A`, `B`, `C` の中で）異なる文字で置き換え、$ S_{i\ +\ 1} $ を $ S $ から削除する

操作を $ 0 $ 回以上行ったあとの $ S $ として、ありえるものの種類数を $ 10^9+7 $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

操作を $ 0 $ 回以上行ったあとの $ S $ として、ありえるものの種類数を $ 10^9+7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
ABAAC
```

### 输出 #1

```
11
```

## 输入输出样例 #2

### 输入 #2

```
50
AACCCCBBBACCCCABABCCCCABACCACACACCACABABBBABABACCB
```

### 输出 #2

```
256972022
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^6 $
- $ S $ は `A`, `B`, `C` からなる長さ $ N $ の文字列

### Sample Explanation 1

たとえば以下のように操作すると、文字列 $ S $ として `ACB` が得られます。 - まず $ i $ として $ 2 $ を選ぶ。$ S_2 $ を `C` で置き換え、$ S_3 $ を削除するので $ S $ は `ACAC` になる - 次に $ i $ として $ 3 $ を選ぶ。$ S_3 $ を `B` で置き換え、$ S_4 $ を削除するので $ S $ は `ACB` になる