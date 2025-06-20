# AT_arc032_1 [ARC032A] ホリドッグ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc032/tasks/arc032_1

とても賢い犬であるホリドッグ(Holidog)くんは、足し算と素数判定をすることができます。 ホリドッグくんはある正整数についてそれが素数であるか尋ねられたとき、それが素数であるなら `WANWAN`、そうでなければ `BOWWOW` と吠えます。

あなたは、ホリドッグくんに $ 1 $ から $ n $ までの総和 $ 1\ +\ 2\ +\ 3\ +\ …\ +\ n $ が素数であるかどうかを尋ねました。ホリドッグくんがどう吠えたかを出力するプログラムを書いて下さい。

素数とは、$ 1 $ とその数自身以外の正整数で割り切ることが出来ない $ 2 $ 以上の正整数のことを言います。例えば $ 2 $ や $ 3 $ や $ 17 $ は素数です。$ 1 $ や $ 10 $ は素数ではありません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ n $

- $ 1 $ 行目には、$ 1 $ つの整数 $ n\ (1\ ≦\ n\ ≦\ 1000) $ が与えられる.

## 输出格式

$ 1 $ 行目には、$ 1\ +\ 2\ +\ 3\ +\ …\ +\ n $ が素数ならば `WANWAN`、 そうでなければ `BOWWOW` を出力せよ。

末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
WANWAN
```

## 输入输出样例 #2

### 输入 #2

```
5
```

### 输出 #2

```
BOWWOW
```

## 输入输出样例 #3

### 输入 #3

```
1
```

### 输出 #3

```
BOWWOW
```

## 输入输出样例 #4

### 输入 #4

```
999
```

### 输出 #4

```
BOWWOW
```

## 说明/提示

### Sample Explanation 1

$ 1\ +\ 2\ =\ 3 $ であり、$ 3 $ は素数なので `WANWAN` と出力します。

### Sample Explanation 2

$ 1\ +\ 2\ +\ 3\ +\ 4\ +\ 5\ =\ 15 $ であり、$ 15\ =\ 3\ ×\ 5 $ なので、 `BOWWOW` と出力します。

### Sample Explanation 3

$ 1 $ は素数ではありません。

### Sample Explanation 4

$ 1\ +\ 2\ +\ ...\ +\ 999 $ は素数ではありません。