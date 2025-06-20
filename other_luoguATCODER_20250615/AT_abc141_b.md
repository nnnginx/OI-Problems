# AT_abc141_b [ABC141B] Tap Dance

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc141/tasks/abc141_b

高橋君はタップダンスをすることにしました。タップダンスの動きは文字列 $ S $ で表され、$ S $ の各文字は `L`, `R`, `U`, `D` のいずれかです。各文字は足を置く位置を表しており、$ 1 $ 文字目から順番に踏んでいきます。

$ S $ が以下の $ 2 $ 条件を満たすとき、またその時に限り、$ S $ を「踏みやすい」文字列といいます。

- 奇数文字目がすべて `R`, `U`, `D` のいずれか。
- 偶数文字目がすべて `L`, `U`, `D` のいずれか。

$ S $ が「踏みやすい」文字列なら `Yes` を、そうでなければ `No` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ S $

## 输出格式

$ S $ が「踏みやすい」文字列なら `Yes` を、そうでなければ `No` を出力してください。

## 输入输出样例 #1

### 输入 #1

```
RUDLUDR
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
DULL
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
UUUUUUUUUUUUUUU
```

### 输出 #3

```
Yes
```

## 输入输出样例 #4

### 输入 #4

```
ULURU
```

### 输出 #4

```
No
```

## 输入输出样例 #5

### 输入 #5

```
RDULULDURURLRDULRLR
```

### 输出 #5

```
Yes
```

## 说明/提示

### 制約

- $ S $ は長さ $ 1 $ 以上 $ 100 $ 以下の文字列
- $ S $ の各文字は `L`, `R`, `U`, `D` のいずれか

### Sample Explanation 1

$ 1,\ 3,\ 5,\ 7 $ 文字目は `R`, `U`, `D` のいずれかです。 $ 2,\ 4,\ 6 $ 文字目は `L`, `U`, `D` のいずれかです。 したがって、この $ S $ は「踏みやすい」文字列です。

### Sample Explanation 2

$ 3 $ 文字目が `R`, `U`, `D` のいずれでもないので、この $ S $ は「踏みやすい」文字列ではありません。