# AT_bitflyer2018_final_d 数列 XOR

## 题目描述

[problemUrl]: https://atcoder.jp/contests/bitflyer2018-final/tasks/bitflyer2018_final_d

長さ $ N $ の $ 2 $ つの整数列 $ (A_1,\ A_2,\ ...,\ A_N) $, $ (B_1,\ B_2,\ ...,\ B_N) $ があります． あなたは，数列 $ A $ に対して次の操作を繰り返し行うことができます：

- 整数 $ i $ ($ 1\ \leq\ i\ \leq\ N-1) $ を選ぶ．そして，$ A_i $ を $ A_i $ $ xor $ $ A_{i+1} $ に置き換えるか，$ A_{i+1} $ を $ A_i $ $ xor $ $ A_{i+1} $ に置き換えるかのいずれかを行う．

ただし，$ xor $ はビットごとの排他的論理和を表します．

この操作を繰り返すことで，$ A $ と $ B $ を一致させることができるかを判定してください．

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ ... $ A_N $ $ B_1 $ $ B_2 $ ... $ B_N $

## 输出格式

問題文中の操作の繰り返しで，$ A $ と $ B $ を一致させることができるなら `Yes` を，できないなら `No` を出力せよ．

## 输入输出样例 #1

### 输入 #1

```
4
4 6 1 2
4 0 3 2
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
5
1 1 1 1 1
2 2 2 2 2
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
10
9078757738433288 290842434722050 159090006056 289488767243292968 141906289967362 3848861155586 19265097448903424 5761445266577952 616899717105952 343731622434
546704308666859716 487893585065153542 489415167130509384 152982254363317262 324189516636095686 286066742397022348 90758284568626244 239298268501286990 196514071259067468 466853324654813188
```

### 输出 #3

```
No
```

## 输入输出样例 #4

### 输入 #4

```
12
377856130335197936 431521378213127644 96779183645318069 27884533191077098 175463727782485301 417798313887768470 882780118961099438 695638305642195413 844098458810131862 714758857685818365 982440320392901313 58851425009165345
200247916520409945 1079265167001944511 228890967431065270 594413217207808713 799020374004987514 1064838643421037658 816982417931746301 59262707979926837 802875123164857614 244683246935893681 50108983568402635 248665965512365971
```

### 输出 #4

```
Yes
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100000 $
- $ A_i,\ B_i $ は整数
- $ 0\ \leq\ A_i\ \leq\ 2^{60}\ -\ 1 $
- $ 0\ \leq\ B_i\ \leq\ 2^{60}\ -\ 1 $

### Sample Explanation 1

はじめ，$ A $ は $ (4,\ 6,\ 1,\ 2) $ です． - $ i=2 $ を選んで，$ A_2 $ を $ A_2 $ $ xor $ $ A_3 $ で置き換えると，$ A $ は $ (4,\ 7,\ 1,\ 2) $ になります． - $ i=1 $ を選んで，$ A_2 $ を $ A_1 $ $ xor $ $ A_2 $ で置き換えると，$ A $ は $ (4,\ 3,\ 1,\ 2) $ になります． - $ i=3 $ を選んで，$ A_3 $ を $ A_3 $ $ xor $ $ A_4 $ で置き換えると，$ A $ は $ (4,\ 3,\ 3,\ 2) $ になります． - $ i=2 $ を選んで，$ A_2 $ を $ A_2 $ $ xor $ $ A_3 $ で置き換えると，$ A $ は $ (4,\ 0,\ 3,\ 2) $ になります． よって，$ A $ と $ B $ を一致させることができます．

### Sample Explanation 2

どのように操作をしても，$ A $ と $ B $ を一致させることはできません．