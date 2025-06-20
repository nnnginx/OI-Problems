# AT_joig2022_c 投票 (Voting)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joig2022-open/tasks/joig2022_c

JOI 高校において，ある議題に関して「賛成」か「反対」かを問う採決が行われ，$ N $ 人の生徒が順番に投票を行った．生徒は自分の投票前に，それまでに投票した他の生徒がどちらに投票したかを知ることができた．

$ i $ 番目 ($ 1\ \leqq\ i\ \leqq\ N $) に投票した生徒は，次の条件を満たしたとき「賛成」に投票し，満たさなかったとき「反対」に投票した．

- 直前に投票した $ X_i $ 人の生徒，すなわち $ i-1,i-2,...,i-X_i $ 番目に投票した生徒のうち，$ Y_i $ 人以上が「賛成」に投票した．

ただし， $ Y_i=0 $ のときは他の生徒の投票に関わらず「賛成」に投票し，$ Y_i=X_i+1 $ のときは他の生徒の投票に関わらず「反対」に投票したとする．

各生徒の投票についての情報が与えられたとき，「賛成」に投票した生徒の人数を求めるプログラムを作成せよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ X_1 $ $ Y_1 $ $ X_2 $ $ Y_2 $ $ \vdots $ $ X_N $ $ Y_N $

## 输出格式

標準出力に，「賛成」に投票した生徒の人数を $ 1 $ 行で出力せよ．

## 输入输出样例 #1

### 输入 #1

```
4
0 1
1 0
1 1
3 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5
0 0
1 1
2 3
3 1
4 3
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
10
0 0
1 2
1 1
1 0
3 1
2 3
1 1
5 3
8 4
7 2
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ \leqq\ N\ \leqq\ 500\,000 $．
- $ 0\ \leqq\ X_i\ \leqq\ i-1 $ ($ 1\ \leqq\ i\ \leqq\ N $)．
- $ 0\ \leqq\ Y_i\ \leqq\ X_i+1 $ ($ 1\ \leqq\ i\ \leqq\ N $)．
- 入力される値はすべて整数である．

### 小課題

1. ($ 28 $ 点) $ N\ \leqq\ 3\,000 $．
2. ($ 32 $ 点) $ X_i\ =\ i-1 $ ($ 1\ \leqq\ i\ \leqq\ N $)．
3. ($ 40 $ 点) 追加の制約はない．

### 採点に関する注意

すべての提出はジャッジシステム上で採点される．

提出されたソースコードは，小課題に対応するすべての採点用入力データについて正しい結果を返したとき，その小課題について正解と認められる．

各提出の得点は，提出されたソースコードについて正解と認められた小課題の得点の合計である．

この課題の得点は，**この課題に対するすべての提出の得点の最大値**である．

現在の得点は「提出結果」タブの「自分の得点状況」から確認できる．

### Sample Explanation 1

投票は，以下のように $ 4 $ 人の生徒によって順番に行われた． 1. $ 1 $ 番目に投票した生徒は，$ Y_1=X_1+1 $ であるため，「反対」に投票した． 2. $ 2 $ 番目に投票した生徒は，$ Y_2=0 $ であるため，「賛成」に投票した． 3. 直前に投票した $ X_3(=1) $ 人の生徒のうち「賛成」に投票したのは $ 1 $ 人で，これは $ Y_3(=1) $ 人以上である．そのため，$ 3 $ 番目に投票した生徒は「賛成」に投票した． 4. 直前に投票した $ X_4(=3) $ 人の生徒のうち「賛成」に投票したのは $ 2 $ 人で，これは $ Y_4(=3) $ 人以上ではない．そのため，$ 4 $ 番目に投票した生徒は「反対」に投票した． 「賛成」に投票した生徒は $ 2 $ 人である．したがって，$ 2 $ を出力する． この入力例は小課題 $ 1,3 $ の制約を満たす．

### Sample Explanation 2

この入力例はすべての小課題の制約を満たす．

### Sample Explanation 3

この入力例は小課題 $ 1,3 $ の制約を満たす．