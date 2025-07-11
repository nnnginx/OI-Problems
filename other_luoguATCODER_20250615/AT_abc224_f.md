# AT_abc224_f [ABC224F] Problem where +s Separate Digits

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc224/tasks/abc224_f

$ 1 $ から $ 9 $ までの数字のみで構成された文字列 $ S $ が与えられます。  
 この文字列 $ S $ から、以下の操作によって式 $ T $ を作ります。

- はじめ、 $ T=S $ であるとする。
- 各要素が $ 1 $ 以上 $ |S|-1 $ 以下の整数である、値に重複のない集合 $ A $ を選ぶ。なお、 $ A $ が空集合であってもよい。
- $ A $ の全ての要素 $ x $ について、 $ x $ の降順に以下の操作を行う。
  - $ T $ の $ x $ 文字目と $ x+1 $ 文字目の間に、 `+` を挿入する。

例えば、 $ S= $ `1234`、 $ A=\ \lbrace\ 2,3\ \rbrace $ であるとき、 $ T $= `12+3+4` となります。

この操作によって得られる $ T $ としてあり得る全ての式に対して、式を計算したときの値の総和を $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1234
```

### 输出 #1

```
1736
```

## 输入输出样例 #2

### 输入 #2

```
1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
31415926535897932384626433832795
```

### 输出 #3

```
85607943
```

## 说明/提示

### 制約

- $ 1\ \le\ |S|\ \le\ 2\ \times\ 10^5 $
- $ S $ は `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9` のみからなる。

### Sample Explanation 1

式 $ T $ としてあり得るものは `1234`, `123+4`, `12+34`, `12+3+4`, `1+234`, `1+23+4`, `1+2+34`, `1+2+3+4` の $ 8 $ つです。 これらを計算した値の総和は $ 1736 $ です。

### Sample Explanation 2

$ S $ の長さが $ 1 $ であることもあります。この場合、 $ A $ として指定可能なのは空集合のみです。

### Sample Explanation 3

答えを $ 998244353 $ で割った余りを求めてください。