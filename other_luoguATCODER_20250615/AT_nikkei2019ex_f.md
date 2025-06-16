# AT_nikkei2019ex_f スーパーFizzBuzz

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-ex/tasks/nikkei2019ex_f

整数 $ N $ が与えられます。[FizzBuzz問題](https://ja.wikipedia.org/wiki/Fizz_Buzz) (リンク先は Wikipedia「Fizz Buzz」) を解いてください。 ただし、通常のFizzBuzz問題においては

- $ 3 $ の倍数に対し `Fizz`
- $ 5 $ の倍数に対し `Buzz`

と出力しますが、今回は、

- $ 2 $ の倍数に対し `a`
- $ 3 $ の倍数に対し `b`
- $ 4 $ の倍数に対し `c`
- $ 5 $ の倍数に対し `d`
- $ 6 $ の倍数に対し `e`

と出力してください。 (より詳しくは、出力例 1 をご覧ください。)

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

解答を $ N $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
20
```

### 输出 #1

```
1
a
b
ac
d
abe
7
ac
b
ad
11
abce
13
a
bd
ac
17
abe
19
acd
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 1,000 $

### Sample Explanation 1

$ 7 $ 行目と $ 10 $ 行目の出力について述べます。 - $ 7 $ 行目: $ 7 $ は $ 2,3,4,5,6 $ のいずれの倍数でもないため、`7` と出力します。 - $ 10 $ 行目: $ 10 $ は $ 2 $ と $ 5 $ の倍数であるため、`ad` と出力します。