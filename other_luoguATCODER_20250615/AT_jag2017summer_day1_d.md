# AT_jag2017summer_day1_d くさかべ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2017summer-day1/tasks/jag2017summer_day1_d

日下部さんは壁に反射するのが大好きで、今日も元気に壁に反射して遊んでいます。

今日の壁は、直角三角形の部屋の壁です。 下図のように三角形の頂点をそれぞれ $ A,B,C $ と呼ぶことにします。 日下部さんは頂点 $ C $ から点 $ P $ に向かってまっすぐ歩き、点 $ P $ に着くと、角 $ BPC $ = 角 $ APQ $ となるような辺 $ AC $ 上の点 $ Q $ に向かって再びまっすぐ歩きました。

 ![ba130de932710340d919adab948af555.png](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_jag2017summer_day1_d/94a7154ec35c33adc31c305fb0850c7b365271b2.png)

線分 $ AB $ の長さは $ X $、線分 $ BC $ の長さは $ Y $、線分 $ AQ $ の長さは $ Z $ でした。 このとき、線分 $ AP $ の長さはいくらでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ X $ $ Y $ $ Z $

## 输出格式

線分 $ AP $ の長さを出力せよ。 ただし、絶対誤差または相対誤差が $ 10^{-9} $ 以下ならば正解とみなされる。

## 输入输出样例 #1

### 输入 #1

```
6 8 5
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
100 100 1
```

### 输出 #2

```
1.40428377656192537870
```

## 说明/提示

### 制約

- $ 1≦X,Y≦100 $
- $ 1≦Z\ <\ \sqrt{X^2+Y^2} $
- $ X,Y,Z $ は整数である