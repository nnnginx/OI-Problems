# AT_abc268_h [ABC268Ex] Taboo

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc268/tasks/abc268_h

文字列 $ S $ が与えられます。また、高橋君は次の操作を $ 0 $ 回以上行うことが出来ます。

- $ 1\ \leq\ i\ \leq\ |S| $ なる整数 $ i $ を選び、$ S $ の $ i $ 文字目を `*` に変える。

高橋君の目的は、$ S $ の**部分文字列として** $ N $ 個の文字列 $ T_1,T_2,\ldots,T_N $ がいずれも現れないようにすることです。  
 これを達成するために必要な操作の回数の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ N $ $ T_1 $ $ T_2 $ $ \vdots $ $ T_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
abcdefghijklmn
3
abcd
ijk
ghi
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
atcoderbeginnercontest
1
abc
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
aaaaaaaaa
2
aa
xyz
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 5\ \times\ 10^5 $
- $ 1\ \leq\ N $
- $ N $ は整数
- $ 1\ \leq\ |T_i| $
- $ \sum{|T_i|}\ \leq\ 5\ \times\ 10^5 $
- $ i\ \neq\ j $ ならば $ T_i\ \neq\ T_j $
- $ S,\ T_i $ は英小文字のみからなる文字列

### Sample Explanation 1

$ i $ として $ 1 $ と $ 9 $ を選んで操作をすると $ S $ は `\*bcdefgh\*jklmn` となり、`abcd`、`ijk`、`ghi` がいずれも部分文字列として現れなくなります。

### Sample Explanation 2

操作をする必要がありません。