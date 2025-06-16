# AT_abc359_a [ABC359A] Count Takahashi

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc359/tasks/abc359_a

文字列が $ N $ 個与えられます。

$ i $ 番目 $ (1\leq\ i\leq\ N) $ に与えられる文字列 $ S\ _\ i $ は `Takahashi` か `Aoki` のどちらかと等しいです。

$ S\ _\ i $ が `Takahashi` と等しい $ i $ がいくつあるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S\ _\ 1 $ $ S\ _\ 2 $ $ \vdots $ $ S\ _\ N $

## 输出格式

$ S\ _\ i $ が `Takahashi` と等しい $ i $ の個数を整数として一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
Aoki
Takahashi
Takahashi
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2
Aoki
Aoki
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
20
Aoki
Takahashi
Takahashi
Aoki
Aoki
Aoki
Aoki
Takahashi
Aoki
Aoki
Aoki
Takahashi
Takahashi
Aoki
Takahashi
Aoki
Aoki
Aoki
Aoki
Takahashi
```

### 输出 #3

```
7
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 100 $
- $ N $ は整数
- $ S\ _\ i $ は `Takahashi` か `Aoki` のいずれか $ (1\leq\ i\leq\ N) $
 
### Sample Explanation 1

$ S\ _\ 2,S\ _\ 3 $ の $ 2 $ つが `Takahashi` と等しく、$ S\ _\ 1 $ はそうではありません。 よって、`2` を出力してください。

### Sample Explanation 2

`Takahashi` と等しい $ S\ _\ i $ が存在しないこともあります。