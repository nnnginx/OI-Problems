# AT_abc326_c [ABC326C] Peak

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc326/tasks/abc326_c

高橋くんは数直線上に $ N $ 個のプレゼントを置きました。そのうち $ i $ 個目のプレゼントは座標 $ A_i $ に置かれました。

あなたは数直線上の長さ $ M $ の半開区間 $ [x,x+M) $ を選び、そこに含まれるプレゼントを全て獲得します。  
 より詳しくは、以下の手順でプレゼントを獲得します。

- まず、実数 $ x $ をひとつ選択する。
- その後、プレゼントのうち置かれている座標が $ x\ \le\ A_i\ <\ x+M $ を満たすものを全て獲得する。
 
最大でいくつのプレゼントを獲得することができますか?

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
8 6
2 3 5 7 11 13 17 19
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
10 1
3 1 4 1 5 9 2 6 5 3
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
10 998244353
100000007 0 1755647 998244353 495 1000000000 1755648 503 1755649 998244853
```

### 输出 #3

```
7
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ N\ \le\ 3\ \times\ 10^5 $
- $ 1\ \le\ M\ \le\ 10^9 $
- $ 0\ \le\ A_i\ \le\ 10^9 $
 
### Sample Explanation 1

例えば、半開区間 $ [1.5,7.5) $ を指定します。 このとき、座標 $ 2,3,5,7 $ にある $ 4 $ つのプレゼントを全て獲得することができ、これが獲得可能な最大の個数です。

### Sample Explanation 2

同一の座標に複数のプレゼントが置いてあることもあります。