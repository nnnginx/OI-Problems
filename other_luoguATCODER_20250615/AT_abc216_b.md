# AT_abc216_b [ABC216B] Same Name

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc216/tasks/abc216_b

$ N $ 人の人がいます。$ i\ \,\ (1\ \leq\ i\ \leq\ N) $ 人目の人の姓は $ S_i $、名は $ T_i $ です。

同姓同名であるような人の組が存在するか、すなわち $ 1\ \leq\ i\ \lt\ j\ \leq\ N $ かつ $ S_i=S_j $ かつ $ T_i=T_j $ を満たすような整数対 $ (i,j) $ が存在するか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ T_1 $ $ S_2 $ $ T_2 $ $ \hspace{0.6cm}\vdots $ $ S_N $ $ T_N $

## 输出格式

同姓同名であるような人の組が存在するなら `Yes` を、存在しないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
tanaka taro
sato hanako
tanaka taro
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
3
saito ichiro
saito jiro
saito saburo
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
4
sypdgidop bkseq
bajsqz hh
ozjekw mcybmtt
qfeysvw dbo
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 1000 $
- $ N $ は整数
- $ S_i,T_i $ は英小文字のみからなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列

### Sample Explanation 1

$ 1 $ 人目の人と $ 3 $ 人目の人が同姓同名です。

### Sample Explanation 2

同姓同名であるような人の組は存在しません。