# AT_past202005_c 等比数列

## 题目描述

[problemUrl]: https://atcoder.jp/contests/past202005-open/tasks/past202005_c

初項 $ A $、公比 $ R $ の等比数列の第 $ N $ 項が $ 10^9 $ より大きければ `large` を、$ 10^9 $ 以下ならその値を整数で出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ R $ $ N $

## 输出格式

問題で指定された値または文字列を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 3 4
```

### 输出 #1

```
54
```

## 输入输出样例 #2

### 输入 #2

```
4 3 21
```

### 输出 #2

```
large
```

## 输入输出样例 #3

### 输入 #3

```
12 34 5
```

### 输出 #3

```
16036032
```

## 说明/提示

### 注意

この問題に対する言及は、2020/6/6 18:00 JST まで禁止されています。言及がなされた場合、賠償が請求される可能性があります。 試験後に総合得点や認定級を公表するのは構いませんが、どの問題が解けたかなどの情報は発信しないようにお願いします。

### 制約

- 入力はすべて整数
- $ 1\ \leq\ A,\ R,\ N\ \leq\ 10^9 $

### Sample Explanation 1

初項 $ 2 $、公比 $ 3 $ の等比数列は $ 2,\ 6,\ 18,\ 54,\ \ldots $ です。これの第 $ 4 $ 項は $ 54 $ であるため、$ 54 $ を出力します。

### Sample Explanation 2

初項 $ 4 $、公比 $ 3 $ の等比数列の第 $ 21 $ 項は $ 13947137604 $ であり、これは $ 10^9 $ より大きいため、`large` を出力します。