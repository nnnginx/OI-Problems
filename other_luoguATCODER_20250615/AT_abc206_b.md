# AT_abc206_b [ABC206B] Savings

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc206/tasks/abc206_b

シカのAtCoDeerくんは、空の貯金箱を持っています。  
 AtCoDeerくんは、その貯金箱に、$ 1 $ 日目の朝に $ 1 $ 円、$ 2 $ 日目の朝に $ 2 $ 円 $ \dots $ というように、$ i $ 日目の朝に $ i $ 円を貯金箱に入れます。  
 また、AtCoDeerくんは、毎日夜に貯金箱にいくら入っているかを確認します。  
 AtCoDeerくんが貯金箱に $ N $ 円以上入っていることを初めて確認するのは、何日目の夜でしょうか?

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
12
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
100128
```

### 输出 #2

```
447
```

## 说明/提示

### 制約

- $ 1\ \le\ N\ \le\ 10^9 $
- $ N $ は整数

### Sample Explanation 1

\- $ 1 $ 日目の朝に $ 1 $ 円貯金する。 この日の夜、貯金箱の中身は $ 1 $ 円である。 - $ 2 $ 日目の朝に $ 2 $ 円貯金する。 この日の夜、貯金箱の中身は $ 3 $ 円である。 - $ 3 $ 日目の朝に $ 3 $ 円貯金する。 この日の夜、貯金箱の中身は $ 6 $ 円である。 - $ 4 $ 日目の朝に $ 4 $ 円貯金する。 この日の夜、貯金箱の中身は $ 10 $ 円である。 - $ 5 $ 日目の朝に $ 5 $ 円貯金する。 この日の夜、貯金箱の中身は $ 15 $ 円である。 よって、AtCoDeerくんが貯金箱に $ 12 $ 円以上入っていることを初めて確認するのは、 $ 5 $ 日目の夜です。