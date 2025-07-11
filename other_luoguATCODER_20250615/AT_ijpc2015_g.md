# AT_ijpc2015_g IOI

## 题目描述

[problemUrl]: https://atcoder.jp/contests/ijpc2015/tasks/ijpc2015_g

すぬけ君はIOI(International Olympiad in Inverting)に$ h-1 $人の選手を引率して団長として参加することになった。

IOIでは縦 $ h× $ 横 $ w $ の大きさの反転パズルを団長と選手が協力して解く。 具体的には団長と選手合わせて$ h $人がそれぞれ1行ずつ担当し、その行のマス目だけ押すことができる。

さて、IOIのコンテストはいよいよ明日になったがすぬけ君は急用で帰国しなければならなくなった。 幸いまぬけ君もチームに同行していたのですぬけ君の代わりにコンテストに参加してくれることになったが、まぬけ君はまぬけなので反転パズルを解くことができない。

 そこですぬけ君は反転パズルの初期状態と団長の担当する行番号を入力するとまぬけ君の押すべきマス目の列番号の一覧を出力してくれる機械を作ることにした。

 ただし、反転パズルとは白黒に塗られた盤面が与えられ、各人が担当する行のマスを選び、選ばれたマス及びそのマスに辺で隣接するマスの白黒を反転することを繰り返し、最終的にすべてのマスを白にすることを目的とするパズルである。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ w $ $ h $ $ r $ $ a $ $ x_1 $ $ b_1 $ $ y_{1,1} $ $ y_{1,2} $ ... $ y_{1,b1} $ ... ... $ x_a $ $ b_a $ $ y_{a,1} $ $ y_{a,2} $ ... $ y_{a,b_a} $

 一行目の入力は、$ w,h $ はそれぞれ盤面の列と行の数を、$ r $ は団長の担当する行番号を表している。

二行目以降の入力は盤面が$ 1≦i≦a,1≦j≦b_i $についてマス$ (x_i,y_{i,j}) $は黒マスでそれ以外は白マスであることを表している。

- $ 1\ ≦\ w\ ≦\ 60 $
- $ 1\ ≦\ h\ ≦\ 1000000000000000000\ (=10^{18}) $
- $ 1\ ≦\ r\ ≦\ h $
- $ 1\ ≦\ a\ ≦\ 100 $
- $ 1\ ≦\ i\ ≦\ a $に対して 
  - $ 1\ ≦\ x_i\ ≦\ h $
  - $ 1\ ≦\ b_i\ ≦\ w $
  - $ 1\ ≦y_{i,1} $
  - $ x_i\ ≠\ x_j(i\ ≠\ j) $

部分点制約

subtask1(10点):$ w,h\ ≦10 $

subtask2(25点):$ h\ ≦10000 $

subtask3(10点):$ h\ ≦1000000 $

subtask4(25点):$ a\ ≦10 $

subtask5(15点):$ a\ ≦50 $

subtask6(15点):追加の制約はない

## 输出格式

无

## 输入输出样例 #1

### 输入 #1

```
3 3 1
3
1 1 2
2 1 1
3 1 3
```

### 输出 #1

```
1 2
```

## 输入输出样例 #2

### 输入 #2

```
3 3 2
3
1 1 2
2 1 1
3 1 3
```

### 输出 #2

```
2 1 3
```

## 输入输出样例 #3

### 输入 #3

```
3 3 3
3
1 1 2
2 1 1
3 1 3
```

### 输出 #3

```
2 2 3
```

## 输入输出样例 #4

### 输入 #4

```
10 10 5
3
3 2 5 7
5 4 1 4 6 9
6 1 10
```

### 输出 #4

```
5 2 4 5 6 10
```

## 说明/提示

### Sample Explanation 3

\### 入力例$ 4 $ ``` 10 10 5 3 3 2 5 7 5 4 1 4 6 9 6 1 10 ``` ### 出力例$ 4 $ ``` 5 2 4 5 6 10 ```