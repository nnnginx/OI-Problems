# AT_abc296_e [ABC296E] Transition Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc296/tasks/abc296_e

長さ $ N $ の数列 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。ここで、各 $ A_i $ $ (1\leq\ i\leq\ N) $ は $ 1\leq\ A_i\ \leq\ N $ をみたします。

高橋君と青木君が $ N $ 回ゲームを行います。$ i=1,2,\ldots,N $ 回目のゲームは次のようにして行われます。

1. 青木君が正整数 $ K_i $ を指定する。
2. 青木君の指定した $ K_i $ を聞いた後、高橋君は $ 1 $ 以上 $ N $ 以下の整数 $ S_i $ を選び、黒板に書く。
3. その後、 $ K_i $ 回次の操作を繰り返す。
  
  
  - 黒板に $ x $ が書かれているとき、それを消し、$ A_x $ を新しく書く。

$ K_i $ 回の操作の後で黒板に書かれている整数が $ i $ ならば $ i $ 回目のゲームは高橋君の勝ち、そうでないならば青木君の勝ちとなります。  
ここで、$ K_i,S_i $ は $ i=1,2,\ldots,N $ に対して独立に選ぶ事ができます。

両者が、自身が勝つために最善の行動をとったとき、$ N $ 回のゲームのうち高橋君が勝つ回数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

両者が最善の行動をとったとき、$ N $ 回のゲームのうち高橋君が勝つ回数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 2 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2
2 1
```

### 输出 #2

```
2
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ A_i\leq\ N $
- 入力はすべて整数

### Sample Explanation 1

$ 1 $ 回目のゲームにおいて、青木君が $ K_1=2 $ を指定したとき、高橋君は $ S_1 $ として、$ 1,2,3 $ のいずれを選んでも勝つことはできません。 例えば、高橋君が最初に黒板に $ S_1=1 $ と書いたとすると、$ 2 $ 回の操作で黒板に書かれている数は順に $ 1\to\ 2(=A_1) $ 、$ 2\to\ 2(=A_2) $ と変化し、 最終的に黒板に書かれている数は $ 2(\neq\ 1) $ であるため、青木君の勝ちとなります。 一方、$ 2,3 $ 回目のゲームにおいては、青木君の指定した $ K_i $ の値によらず、高橋君はそれぞれ $ 2,3 $ を最初に黒板に書くことで勝つ事ができます。 よって、両者が、自分が勝つために最善の行動をとったとき、高橋君が勝つゲームは $ 2,3 $ 回目の $ 2 $ 回であるため、$ 2 $ を出力します。

### Sample Explanation 2

$ 1 $ 回目のゲームにおいて、高橋君は、青木君が指定した $ K_1 $ が奇数のときは $ 2 $、偶数のときは $ 1 $ を最初に黒板に書く事で勝つ事ができます。 同様に $ 2 $ 回目のゲームにおいても勝つ方法が存在するため、$ 1,2 $ 回目のゲームのいずれでも高橋君は勝利する事ができ、$ 2 $ が答えとなります。