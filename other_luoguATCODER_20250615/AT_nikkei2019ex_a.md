# AT_nikkei2019ex_a Prefix Array

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-ex/tasks/nikkei2019ex_a

文字列 $ S $ が与えられます。$ S $ の *Prefix Array* を求めなさい。

ただし、Prefix Arrayとは、[Suffix Array](https://ja.wikipedia.org/wiki/%E6%8E%A5%E5%B0%BE%E8%BE%9E%E9%85%8D%E5%88%97) (リンク先は Wikipedia「接尾辞配列」) の定義における「接尾辞」を「接頭辞」に変更したものです。

(具体例は下記の入出力例 1 で確認できます。)

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ S $ の Prefix Array を $ |S| $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
chokudai
```

### 输出 #1

```
1
2
3
4
5
6
7
8
```

## 说明/提示

### 制約

- $ 1\ ≦\ |S|\ ≦\ 100,000 $
- $ S $ は小文字アルファベットのみからなる。

### Sample Explanation 1

`chokudai` のすべての接尾辞を辞書順にソートすると、以下のようになります。 - `c` - `ch` - `cho` - `chok` - `choku` - `chokud` - `chokuda` - `chokudai`