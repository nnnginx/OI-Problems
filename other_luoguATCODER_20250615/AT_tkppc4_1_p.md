# AT_tkppc4_1_p Flip Cards

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tkppc4-1/tasks/tkppc4_1_p

 ある日、sanadaはkaageに $ N $ 枚のカードを引くように言われました。  
 sanadaはとりあえず、言われるがままにカードを引きました。  
 このカードには表と裏にそれぞれ数が書かれており、$ 2 $ 面に書かれた数の合計は常に $ M $ でした。sanadaが引いた $ N $ 枚のカードにおいて、$ i $ 枚目の表に書かれていた数は $ A_i $ です。

 次に、kaageは以下の操作を $ K $ 回以内の任意の回数（$ 0 $ 回でも可）することを指示しました。

- $ 1\ \leq\ x\leq\ y\leq\ N $ を満たす任意の整数 $ x,y $ を選び、$ x $ 枚目から $ y $ 枚目までの全てのカードの表裏を反転する。

 不審に思ったsanadaは、kaageの家にスパイを送り込み、$ N $ 枚のカードの表に書かれた数の合計が多いほどkaageが勉強しなくてはいけないことを知りました。  
 kaageを勉強させたいsanadaのために、適切な回数・適切な操作を行うことで $ N $ 枚のカードの表に書かれた数の合計を最大いくつにできるか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられます。

> $ N $ $ M $ $ K $  
> $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

適切な回数、適切な操作を行ったとき、全てのカードの表に書かれた数の合計の最大値を $ 1 $ 行に出力してください。

## 输入输出样例 #1

### 输入 #1

```
3 6 13 3 4
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
8 9 21 3 8 7 5 3 5 1
```

### 输出 #2

```
52
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 10^6 $
- $ 0\ \leq\ K\ \leq\ N $
- $ 1\ \leq\ M\ \leq\ 10^9 $
- $ 1\ \leq\ A_i\ \leq\ M-1 $

### 小課題

 この課題には $ 3 $ つの小課題があります。

1. (400 点) $ N\ \leq\ 2000 $
2. (400 点) $ N\ \leq\ 10^5 $
3. (300 点) 追加の制約はない。

### 注意

**小課題 $ 1 $ のみを狙ったコードを提出する際には$ N $ が $ 2000 $より大きいならすぐ終了するといった処理を書き加えることを勧めます。**

### Sample Explanation 1

この場合、例えば一度も操作を行わないときに、カードの表にある数全ての合計を最大の $ 10 $ にできます。

### Sample Explanation 2

例えば次のように区間を選んで操作することで、最大値 $ 52 $ を達成できます。 - $ 1 $ 回目: $ 1 $ 枚目から $ 5 $ 枚目のカードの表裏を反転させる。操作後のカードの並びは {$ 8,\ 6,\ 1,\ 2,\ 4,\ 3,\ 5,\ 1 $} となる。 - $ 2 $ 回目: $ 3 $ 枚目から $ 8 $ 枚目のカードの表裏を反転させる。操作後のカードの並びは {$ 8,\ 6,\ 8,\ 7,\ 5,\ 6,\ 4,\ 8 $} となる。