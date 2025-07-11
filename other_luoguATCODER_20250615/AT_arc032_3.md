# AT_arc032_3 [ARC032C] 仕事計画

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc032/tasks/arc032_3

大工のチョーさん(Daiku Cho)は $ N $ 個の仕事を頼まれています。$ i $ 番目の仕事は時刻 $ a_i $ に始まり、$ b_i $ に終わります。

チョーさんは一度に複数の仕事をこなすことはできないので、これらの仕事のうち、仕事を行う時刻が重ならないようになるべく多くの仕事を選びたいです。ただし、終了と同時に別の仕事に取り掛かることはできます。

最も多く選ぶ方法が複数あるときは、選んだ仕事の番号を開始時刻の順に並べた列が辞書順最小となるように選ぼうと思っています。

大工のチョーさんは仕事上手ですが、スケジュールを管理するのは上手くないようです。チョーさんが引き受ける最適な仕事の組み合わせを求めてください。

ただし、長さ $ L $ の列 $ A=\{a_1,a_2,…,a_L\} $ と $ B=\{b_1,b_2,…,b_L\} $ に対し、辞書順で $ A $ が $ B $ より小さいとは、

- $ i\ <\ k $ で $ a_i $=$ b_i $
- $ i=k $ で $ a_i $&lt;$ b_i $

となるような $ k(1≦k≦L) $ が存在するということです。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ : $ a_N $ $ b_N $

- $ 1 $ 行目には、チョーさんが頼まれた仕事の数を表す整数 $ N\ (1\ ≦\ N\ ≦\ 100,000) $ が与えられる。
- $ 2 $ 行目から $ N $ 行には、チョーさんが頼まれた仕事の情報が与えられる。そのうち $ i $ 行目には、$ i $ 番目の仕事の開始時刻と終了時刻を表す $ 2 $ つの整数 $ a_i,\ b_i(0\ ≦\ a_i\ <\ b_i\ ≦\ 1,000,000) $ がスペース区切りで与えられる。

## 输出格式

$ 1 $ 行目には、チョーさんが引き受ける仕事の数を出力せよ。

$ 2 $ 行目には、チョーさんが引き受ける仕事を、時刻が早いものから順に $ 1 $ つの空白で区切って出力せよ。

末尾の改行を忘れないこと。また、末尾に余計な空白を付け加えないこと。

## 输入输出样例 #1

### 输入 #1

```
4
0 5
0 3
3 7
5 10
```

### 输出 #1

```
2
1 4
```

## 输入输出样例 #2

### 输入 #2

```
5
0 5
0 3
3 7
5 10
7 12
```

### 输出 #2

```
3
2 3 5
```

## 输入输出样例 #3

### 输入 #3

```
8
1 5
3 9
2 5
1 2
8 10
9 11
7 15
10 14
```

### 输出 #3

```
4
4 3 5 8
```

## 说明/提示

### Sample Explanation 1

チョーさんは最大で $ 2 $ つの仕事を選ぶことができます。その選び方は $ 3 $ 通りあり、チョーさんは仕事 $ 1 $ と $ 4 $、または仕事 $ 2 $ と $ 3 $、または仕事 $ 2 $ と $ 4 $ を選ぶことができます。 この内、辞書順で小さくなる選び方は仕事 $ 1 $ と $ 4 $ を選んだときです。なぜならば、それらの仕事番号を \*\*仕事の開始時刻順\*\* に並べたときに $ \{1,4\} $ となり、それが辞書順最小となるからです(21:12修正)。 !\[\](http://arc032.contest.atcoder.jp/img/arc/032/C1.png)