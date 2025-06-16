# AT_abc307_b [ABC307B] racecar

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc307/tasks/abc307_b

英小文字のみからなる $ N $ 個の文字列 $ S_1,S_2,\ldots,S_N $ が与えられます。  
 $ 1 $ 以上 $ N $ 以下の **相異なる** 整数 $ i,j $ であって、$ S_i $ と $ S_j $ をこの順に連結した文字列が回文となるようなものが存在するか判定してください。

ただし、長さ $ M $ の文字列 $ T $ が回文であるとは、任意の $ 1\leq\ i\leq\ M $ について、$ T $ の $ i $ 文字目と $ (M+1-i) $ 文字目が一致していることをいいます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

問題文の条件をみたす $ i,j $ が存在するならば `Yes` を、そうでないならば `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
ab
ccef
da
a
fe
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
3
a
b
aba
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
2
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

### 输出 #3

```
Yes
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 100 $
- $ 1\leq\ \lvert\ S_i\rvert\ \leq\ 50 $
- $ N $ は整数
- $ S_i $ は英小文字のみからなる文字列
- $ S_i $ はすべて異なる。
 
### Sample Explanation 1

$ (i,j)=(1,4) $ とすると、$ S_1= $`ab` と $ S_4= $`a` をこの順に連結した文字列は `aba` となり、 これは回文であるため条件をみたしています。 よって、`Yes` を出力します。 また、$ (i,j)=(5,2) $ としても、$ S_5= $`fe` と $ S_2= $`ccef` をこの順に連結した文字列は `feccef` となり、やはり条件をみたしています。

### Sample Explanation 2

$ S_1 $, $ S_2 $, $ S_3 $ のうち、どの相異なる $ 2 $ つの文字列を繋げても回文となりません。 よって、`No` を出力します。 問題文における $ i,j $ は相異なる必要があることに注意してください。