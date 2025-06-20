# AT_past202107_c 入力チェック

## 题目描述

[problemUrl]: https://atcoder.jp/contests/past202107-open/tasks/past202107_c

`0` から `9` の数字からなる文字列 $ S $ が与えられます。  
 $ S $ を整数の十進数表示として見たとき、以下の $ 2 $ つの条件をともに満たすかどうか判定してください。

- 先頭に不要な `0` がない。
- $ L $ 以上 $ R $ 以下である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ L $ $ R $

## 输出格式

$ S $ が問題文に示す $ 2 $ つの条件をともに満たすならば `Yes` と出力し、 そうでなければ `No` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
13579
10000 20000
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
12345678901234567890
0 1000000000
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
05
5 5
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
0
0 1
```

### 输出 #4

```
Yes
```

## 说明/提示

### 注意

この問題に対する言及は、2021/7/17 18:00 JST まで禁止されています。言及がなされた場合、賠償が請求される可能性があります。 試験後に総合得点や認定級を公表するのは構いませんが、どの問題が解けたかなどの情報は発信しないようにお願いします。

### 制約

- $ S $ は `0` から `9` の数字からなる文字列
- $ 1\ \leq\ |S|\ \leq\ 100 $
- $ 0\ \leq\ L\ \leq\ R\ \leq\ 10^9 $
- $ L $ と $ R $ は整数

### Sample Explanation 1

$ 13579 $ は先頭に不要な `0` を持たず、 $ 10000 $ 以上 $ 20000 $ 以下であるため、条件を満たします。 よって、`Yes` と出力します。

### Sample Explanation 2

$ S $ が表す整数は、$ 64 $ ビット整数型で表現できる最大値よりも大きいことがあります。

### Sample Explanation 3

$ 05 $ は先頭に不要な `0` を持つので、条件を満たしません。 よって、`No` と出力します。

### Sample Explanation 4

$ 0 $ の先頭の `0` は、不要な `0` ではないことに注意してください。