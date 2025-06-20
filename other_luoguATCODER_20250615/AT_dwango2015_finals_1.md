# AT_dwango2015_finals_1 ニコニコ文字列２

## 题目描述

[problemUrl]: https://atcoder.jp/contests/dwango2015-finals/tasks/dwango2015_finals_1

ある文字列 $ A $ について、$ A=&quot;25&quot; $ または $ A=&quot;2525&quot; $ または $ A=&quot;252525&quot; $ ... というふうに $ &quot;25&quot; $ を何回か繰り返した文字列になっているとき、$ A $ はニコニコ文字列であるといいます。たとえば $ &quot;25&quot; $ や $ &quot;25252525&quot; $ はニコニコ文字列ですが、$ &quot;123&quot; $ や $ &quot;225&quot; $ はニコニコ文字列ではありません。

ニワンゴ君があるサイトで使っているパスワードは、`0` から `9` の数字から成る長さ $ N $ の文字列です。しかし、ニワンゴ君はパスワードの一部を忘れてしまいました。ニコニコ文字列となるような連続した部分文字列をパスワードの文字列から取り出す方法が $ X $ 通り以上あることは覚えています。ただし、文字列として同じであっても、取り出し位置が異なっていれば別々に数えたものとします。

パスワードとして考えられる文字列の個数を $ 1,000,000,007\ (10^9+7) $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ X $ $ S $

- $ 1 $ 行目には、$ 2 $ つの整数 $ N\ (1\ ≦\ N\ ≦\ 252),\ X\ (0\ ≦\ X\ ≦\ 252) $ が空白区切りで与えられる。これは、パスワードの長さが $ N $ であり、ニコニコ文字列となるような連続した部分文字列を取り出す方法が $ X $ 通り以上であるということを表す。
- $ 2 $ 行目には、パスワードの情報を表す $ 1 $ つの文字列 $ S $ が与えられる。$ S $ は、`0` から `9` の数字と `?` のみから成る長さ $ N $ の文字列であり、$ S $ の $ i $ 文字目が、 
  - 数字である場合、パスワードの $ i $ 文字目がその数字であることを表す。
  - `?` である場合、パスワードの $ i $ 文字目がどの数字であるかが分からないということを表す。

## 输出格式

パスワードとして考えられる文字列の個数を $ 1,000,000,007\ (10^9+7) $ で割った余りを $ 1 $ 行に出力せよ。出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
3 1
2?5
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
15 4
???5????????9??
```

### 输出 #2

```
976934094
```

## 输入输出样例 #3

### 输入 #3

```
4 10
1234
```

### 输出 #3

```
0
```

## 说明/提示

### Sample Explanation 1

パスワードとして考えられる文字列は $ &quot;225&quot; $ と $ &quot;255&quot; $ の $ 2 $ つです。

### Sample Explanation 2

パスワードの $ 1 $ 文字目は `0` でも良いことに注意してください。

### Sample Explanation 3

このように、忘れている部分が $ 1 $ 箇所もないこともありえます。 また、ニコニコ文字列となるような連続した部分文字列を取り出す方法が $ X $ 以上であるような文字列が存在しないこともありますが、この場合は条件を満たす文字列が $ 0 $ 個なので、$ 0 $ を出力すれば良いです。