# AT_abc185_e [ABC185E] Sequence Matching

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc185/tasks/abc185_e

長さ $ N $ の整数列 $ A $ と、長さ $ M $ の整数列 $ B $ があります。  
 高橋君は $ A $ から、いくつかの要素を取り除き、残った要素をそのままの順番で繋げることで新たな数列 $ A' $ を作ります。(一つも取り除かなくても、全部取り除いても構いません。)  
 $ B $ についても同様に、いくつかの要素を取り除き、残った要素をそのままの順番で繋げることで新たな数列 $ B' $ を作ります。(一つも取り除かなくても、全部取り除いても構いません。)  
 このとき、$ |A'|\ =\ |B'| $ となるような取り除き方をします。(数列 $ s $ について $ |s| $ は $ s $ の長さを表します。)  
 $ A,\ B $ から取り除いた合計要素数を $ x $ とし、$ 1\ \le\ i\ \le\ |A'| $ かつ $ {A'}_i\ \neq\ {B'}_i $ を満たす整数 $ i $ の数を $ y $ とするとき、$ x\ +\ y $ として考えられる最小の値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1\ \hspace{7pt}\ A_2\ \hspace{7pt}\ A_3\ \hspace{5pt}\ \dots\ \hspace{5pt}\ A_N $ $ B_1\ \hspace{7pt}\ B_2\ \hspace{7pt}\ B_3\ \hspace{5pt}\ \dots\ \hspace{5pt}\ B_M $

## 输出格式

$ x\ +\ y $ として考えられる最小の値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
1 2 1 3
1 3 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4 6
1 3 2 4
1 5 2 6 4 3
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
5 5
1 1 1 1 1
2 2 2 2 2
```

### 输出 #3

```
5
```

## 说明/提示

### 制約

- $ 1\ \le\ N,\ M\ \le\ 1000 $
- $ 1\ \le\ A_i,\ B_i\ \le\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

$ A $ から $ A_4 $ を削除して $ A' $ を作り、$ B $ からは何も削除せず $ B' $ を作ることにすると、$ x\ =\ 1 $ となります。 また、このとき $ 1\ \le\ i\ \le\ |A'| $ かつ $ {A'}_i\ \neq\ {B'}_i $ を満たす整数 $ i $ は $ 2 $ の一つのみなので $ y\ =\ 1 $ となります。そして $ x\ +\ y $ は $ 2 $ となり、これが最小です。

### Sample Explanation 2

$ A $ からは何も取り除かず、$ B $ からは $ B_4,\ B_6 $ の $ 2 $ 要素を削除すると $ x\ =\ 2,\ y\ =\ 1 $ となり、 $ x\ +\ y $ は $ 3 $ で、これが最小です。

### Sample Explanation 3

$ A $ からも $ B $ からも何も取り除かないことも許されます。