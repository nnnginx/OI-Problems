# AT_abc278_f [ABC278F] Shiritori

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc278/tasks/abc278_f

$ N $ 個の文字列 $ S\ _\ 1,S\ _\ 2,\ldots,S\ _\ N $ が与えられます。 $ S\ _\ i\ (1\leq\ i\leq\ N) $ は英小文字からなる長さ $ 10 $ 以下の空でない文字列で、互いに異なります。

先手太郎君と後手次郎君がしりとりをします。 このしりとりでは、先手太郎君と後手次郎君の手番が交互に訪れます。 はじめの手番は先手太郎君の手番です。 それぞれのプレイヤーは自分の手番において整数 $ i\ (1\leq\ i\leq\ N) $ を $ 1 $ つ選びます。 このとき、$ i $ は次の $ 2 $ つの条件を満たしていなければなりません。

- $ i $ は、しりとりが開始してからこれまでの $ 2 $ 人の手番で選ばれたどの整数とも異なる
- この手番がしりとりの最初の手番であるか、直前に選ばれた整数を $ j $ として、$ S\ _\ j $ の最後の文字と $ S\ _\ i $ の最初の文字が等しい
 
条件を満たす $ i $ を選べなくなったプレイヤーの負けで、負けなかったプレイヤーの勝ちです。

$ 2 $ 人が最適に行動したときに勝つのはどちらかを判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

$ 2 $ 人が最適に行動したとき、先手太郎君が勝つなら `First`、後手次郎君が勝つなら `Second` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
enum
float
if
modint
takahashi
template
```

### 输出 #1

```
First
```

## 输入输出样例 #2

### 输入 #2

```
10
catch
chokudai
class
continue
copy
exec
havoc
intrinsic
static
yucatec
```

### 输出 #2

```
Second
```

## 输入输出样例 #3

### 输入 #3

```
16
mnofcmzsdx
lgeowlxuqm
ouimgdjxlo
jhwttcycwl
jbcuioqbsj
mdjfikdwix
jhvdpuxfil
peekycgxco
sbvxszools
xuuqebcrzp
jsciwvdqzl
obblxzjhco
ptobhnpfpo
muizaqtpgx
jtgjnbtzcl
sivwidaszs
```

### 输出 #3

```
First
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 16 $
- $ N $ は整数
- $ S\ _\ i\ (1\leq\ i\leq\ N) $ は英小文字からなる長さ $ 10 $ 以下の空でない文字列
- $ S\ _\ i\neq\ S\ _\ j\ (1\leq\ i\lt\ j\leq\ N) $
 
### Sample Explanation 1

例えば、ゲームは以下のように進行します。 この進行例では $ 2 $ 人の行動が必ずしも最適とは限らないことに注意してください。 - 先手太郎君が $ i=3 $ を選ぶ。$ S\ _\ i= $`if` である。 - 後手次郎君が $ i=2 $ を選ぶ。$ S\ _\ i= $`float` であり、`if` の最後の文字と `float` の最初の文字は等しい。 - 先手太郎君が $ i=5 $ を選ぶ。$ S\ _\ i= $`takahashi` であり、`float` の最後の文字と `takahashi` の最初の文字は等しい。 - 後手次郎君は $ i\neq2,3,5 $ であって $ S\ _\ i $ の最初の文字が `i` と等しいものを選べないため、負ける。 このとき、先手太郎君が勝ちます。