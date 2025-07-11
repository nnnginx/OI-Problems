# AT_abc321_f [ABC321F] #(subset sum = K) with Add and Erase

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc321/tasks/abc321_f

箱を用意します。最初、箱は空です。  
この箱に対して、以下の $ 2 $ 種類の操作を合計 $ Q $ 個、入力で与えられた順に施します。

> \+ $ x $

タイプ $ 1 $ : 箱の中に整数 $ x $ の書かれたボールを $ 1 $ つ追加する。

> \- $ x $

タイプ $ 2 $ : 箱の中にある、整数 $ x $ の書かれたボールを $ 1 $ つ取り除く。  
**但し、取り除く前の時点で箱の中に整数 $ x $ が書かれたボールが含まれることが保証されます。**

各操作後の箱に関して、以下の問題を解いてください。

> 箱からボールをいくつか取り出して、ボールに書かれた整数の総和を $ K $ とする方法の総数を $ 998244353 $ で割った余りを求めてください。  
> 但し、箱の中に入っている全てのボールは区別可能です。

## 输入格式

入力は以下の形式で標準入力から与えられる。  
但し、 $ \rm{Query} $$ _{i} $ は $ i $ 個目の操作を表す。

> $ Q $ $ K $ $ \rm{Query} $$ _{1} $ $ \rm{Query} $$ _{2} $ $ \vdots $ $ \rm{Query} $$ _{Q} $

## 输出格式

全体で $ Q $ 行出力せよ。  
そのうち $ i $ 行目には、 $ i $ 個目までの操作を終えた時点での答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
15 10
+ 5
+ 2
+ 3
- 2
+ 5
+ 10
- 3
+ 1
+ 3
+ 3
- 5
+ 1
+ 7
+ 4
- 3
```

### 输出 #1

```
0
0
1
0
1
2
2
2
2
2
1
3
5
8
5
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \le\ Q\ \le\ 5000 $
- $ 1\ \le\ K\ \le\ 5000 $
- タイプ $ 1 $ の操作に関して、 $ 1\ \le\ x\ \le\ 5000 $
- 全ての操作は問題文中の条件を満たす。

### Sample Explanation 1

この入力には、操作が $ 15 $ 個含まれます。 最後の操作の後、箱の中に入ったボールは $ (5,10,1,3,1,7,4) $ となります。 総和を $ 10 $ にする方法は以下の $ 5 $ 通りです。 - $ 5+1+3+1 $ ( $ 1,3,4,5 $ 番目のボールを取り出す ) - $ 5+1+4 $ ( $ 1,3,7 $ 番目のボールを取り出す ) - $ 5+1+4 $ ( $ 1,5,7 $ 番目のボールを取り出す ) - $ 10 $ ( $ 2 $ 番目のボールを取り出す ) - $ 3+7 $ ( $ 4,6 $ 番目のボールを取り出す )