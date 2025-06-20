# AT_abc314_f [ABC314F] A Certain Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc314/tasks/abc314_f

とあるゲームの大会に、プレイヤー $ 1 $ 、プレイヤー $ 2 $ 、$ \ldots $ 、プレイヤー $ N $ の $ N $ 人のプレイヤーが参加します。 大会の開始直前、各プレイヤーはそれぞれ $ 1 $ 人のみからなるチームをなし、全部で $ N $ 個のチームがあります。

大会では全部で $ N−1 $ 回の試合があり、各試合では $ 2 $ つの異なるチームが選ばれ、一方が先攻を、もう一方が後攻を受け持って対戦し、その結果ちょうど一方のチームが勝ちます。 具体的には、$ i\ =\ 1,\ 2,\ \ldots,\ N-1 $ について $ i $ 回目の試合は下記の通りに進行します。

- プレイヤー $ p_i $ の属するチームが先攻、プレイヤー $ q_i $ の属するチームが後攻として、対戦を行う。
- その結果、先攻チームの人数を $ a $ 、後攻チームの人数を $ b $ として、$ \frac{a}{a+b} $ の確率で先攻のチームが、$ \frac{b}{a+b} $ の確率で後攻のチームが勝つ。
- その後、勝負した $ 2 $ チームは $ 1 $ つのチームに併合される。

なお、各試合の対戦結果は他の試合の対戦結果とは独立です。

$ N $ 人のプレイヤーそれぞれについて、大会全体で自分が所属するチームが勝つという出来事が起こる回数の期待値 $ \text{mod\ }\ 998244353 $ を出力してください。

 期待値 $ \text{mod\ }\ 998244353 $ の定義この問題で求める期待値は必ず有理数になることが証明できます。 また、この問題の制約下では、求める期待値を既約分数 $ \frac{y}{x} $ で表したときに $ x $ が $ 998244353 $ で割り切れないことが保証されます。

このとき $ xz\ \equiv\ y\ \pmod{998244353} $ を満たすような $ 0 $ 以上 $ 998244352 $ 以下の整数 $ z $ が一意に定まります。この $ z $ を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ p_1 $ $ q_1 $ $ p_2 $ $ q_2 $ $ \vdots $ $ p_{N-1} $ $ q_{N-1} $

## 输出格式

各 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、大会全体でプレイヤー $ i $ が所属するチームが勝つという出来事が起こる回数の期待値 $ \text{mod\ }\ 998244353 $ である $ E_i $ を、 下記の形式にしたがって空白区切りで出力せよ。

> $ E_1 $ $ E_2 $ $ \ldots $ $ E_N $

## 输入输出样例 #1

### 输入 #1

```
5
1 2
4 3
5 3
1 4
```

### 输出 #1

```
698771048 698771048 964969543 964969543 133099248
```

## 输入输出样例 #2

### 输入 #2

```
15
9 2
8 10
13 6
12 11
7 10
4 10
14 2
5 4
1 15
15 2
6 9
8 11
6 3
2 8
```

### 输出 #2

```
43970290 310168785 806914186 501498951 950708909 272140427 335124893 168750835 310168785 168750835 280459129 280459129 272140427 476542843 43970290
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ p_i,\ q_i\ \leq\ N $
- $ i $ 回目の試合の直前、プレイヤー $ p_i $ が属するチームとプレイヤー $ q_i $ が属するチームは異なる。
- 入力はすべて整数

### Sample Explanation 1

チームに所属するプレイヤーの番号が $ x_1,\ x_2,\ \ldots,\ x_k $ であるチームを、チーム $ \lbrace\ x_1,\ x_2,\ \ldots,\ x_k\ \rbrace $ と呼びます。 - $ 1 $ 回目の試合では、プレイヤー $ 1 $ が所属するチーム $ \lbrace\ 1\ \rbrace $ とプレイヤー $ 2 $ が所属するチーム $ \lbrace\ 2\ \rbrace $ が対戦し、 $ \frac{1}{2} $ の確率でチーム $ \lbrace\ 1\ \rbrace $ が、$ \frac{1}{2} $ の確率でチーム $ \lbrace\ 2\ \rbrace $ が勝ちます。 その後、$ 2 $ つのチームは併合され、$ 1 $ つのチーム $ \lbrace\ 1,\ 2\ \rbrace $ になります。 - $ 2 $ 回目の試合では、プレイヤー $ 4 $ が所属するチーム $ \lbrace\ 4\ \rbrace $ とプレイヤー $ 3 $ が所属するチーム $ \lbrace\ 3\ \rbrace $ が対戦し、 $ \frac{1}{2} $ の確率でチーム $ \lbrace\ 4\ \rbrace $ が、$ \frac{1}{2} $ の確率でチーム $ \lbrace\ 3\ \rbrace $ が勝ちます。 その後、$ 2 $ つのチームは併合され、$ 1 $ つのチーム $ \lbrace\ 3,\ 4\ \rbrace $ になります。 - $ 3 $ 回目の試合では、プレイヤー $ 5 $ が所属するチーム $ \lbrace\ 5\ \rbrace $ とプレイヤー $ 3 $ が所属するチーム $ \lbrace\ 3,\ 4\ \rbrace $ が対戦し、 $ \frac{1}{3} $ の確率でチーム $ \lbrace\ 5\ \rbrace $ が、$ \frac{2}{3} $ の確率でチーム $ \lbrace\ 3,\ 4\ \rbrace $ が勝ちます。 その後、$ 2 $ つのチームは併合され、$ 1 $ つのチーム $ \lbrace\ 3,\ 4,\ 5\ \rbrace $ になります。 - $ 4 $ 回目の試合では、プレイヤー $ 1 $ が所属するチーム $ \lbrace\ 1,\ 2\ \rbrace $ とプレイヤー $ 4 $ が所属するチーム $ \lbrace\ 3,\ 4,\ 5\ \rbrace $ が対戦し、 $ \frac{2}{5} $ の確率でチーム $ \lbrace\ 1,\ 2\ \rbrace $ が、$ \frac{3}{5} $ の確率でチーム $ \lbrace\ 3,\ 4,\ 5\ \rbrace $ が勝ちます。 その後、$ 2 $ つのチームは併合され、$ 1 $ つのチーム $ \lbrace\ 1,\ 2,\ 3,\ 4,\ 5\ \rbrace $ になります。 プレイヤー $ 1,\ 2,\ 3,\ 4,\ 5 $ それぞれの、大会全体で自分が所属するチームが勝つという出来事が起こる回数の期待値 $ E_1,\ E_2,\ E_3,\ E_4,\ E_5 $ は、それぞれ $ \frac{9}{10},\ \frac{9}{10},\ \frac{53}{30},\ \frac{53}{30},\ \frac{14}{15} $ です。