# AT_abc303_g [ABC303G] Bags Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc303/tasks/abc303_g

$ N $ 個の袋が左右一列に並んでいて、左から $ i $ 番目の袋には $ x_i $ 円が入っています。

十分多くのお金を持っている高橋君と青木君が、高橋君を先手として交互に次の操作をします。

- 以下の $ 3 $ 種類の操作のうち $ 1 $ つを選んで行う。
  - 右端または左端の袋を $ 1 $ 個選んで取る。
  - $ A $ 円をすぬけ君に支払う。そして、「右端または左端の袋を $ 1 $ 個選んで取る」という操作を $ \min(B,n) $ ($ n $ は残っている袋の個数) 回繰り返す。
  - $ C $ 円をすぬけ君に支払う。そして、「右端または左端の袋を $ 1 $ 個選んで取る」という操作を $ \min(D,n) $ ($ n $ は残っている袋の個数) 回繰り返す。

残っている袋が無くなった時点での高橋君の利得を「(高橋君が取った袋に入っている金額の総和) $ - $ (高橋君がすぬけ君に支払った金額の総和)」とし、これを $ X $ 円とします。また、青木君の利得についても同様に定め、$ Y $ 円とします。

高橋君が $ X-Y $ を最大化、青木君が $ X-Y $ を最小化することを目的に最適な操作をしたときの $ X-Y $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $ $ C $ $ D $ $ x_1 $ $ x_2 $ $ \ldots $ $ x_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 10 2 1000000000 1
1 100 1 1 1
```

### 输出 #1

```
90
```

## 输入输出样例 #2

### 输入 #2

```
10 45 3 55 4
5 10 15 20 25 30 35 40 45 50
```

### 输出 #2

```
85
```

## 输入输出样例 #3

### 输入 #3

```
15 796265 10 165794055 1
18804175 185937909 1934689 18341 68370722 1653 1 2514380 31381214 905 754483 11 5877098 232 31600
```

### 输出 #3

```
302361955
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 3000 $
- $ 1\ \leq\ x_i\ \leq\ 10^9 $
- $ 1\ \leq\ A,C\ \leq\ 10^9 $
- $ 1\ \leq\ B,D\ \leq\ N $
- 入力はすべて整数

### Sample Explanation 1

高橋君と青木君が最適な操作をしたとき、$ X=92,\ Y=2 $ となります。