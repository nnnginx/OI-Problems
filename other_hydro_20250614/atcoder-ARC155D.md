## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc155/tasks/arc155_d

$ 2 $ つの非負整数 $ x,\ y $ に対し $ \gcd(x,y) $ を $ x $ と $ y $ の最大公約数とします（ただし、 $ x=0 $ のときは $ \gcd(x,y)=\gcd(y,x)=y $ とします）。

黒板に $ N $ 個の整数が書かれており、そのうち $ i $ 番目の整数は $ A_i $ です。これら $ N $ 個の整数の最大公約数は $ 1 $ です。

高橋君と青木君が $ 2 $ 人で対戦ゲームをします。整数 $ G $ を $ G=0 $ で初期化した後、$ 2 $ 人は高橋君から始めて交互に以下の操作を繰り返します。

- 黒板に書かれている数のうち、$ \gcd(G,a)\neq\ 1 $ をみたす数 $ a $ を選んで消し、$ G $ を $ \gcd(G,a) $ で置き換える。
 
先に操作を行えなくなったほうが負けです。

各 $ i\ (1\leq\ i\ \leq\ N) $ について、高橋君が最初の手番で $ i $ 番目の整数を選んだ後、両者が最善を尽くした場合、どちらが勝つか判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式
$ N $ 行出力せよ。$ i $ 行目には高橋君が最初の手番で $ i $ 番目の整数を選んだ後、両者が最善を尽くした場合、高橋君が勝つ場合は `Takahashi` を、青木君が勝つ場合は `Aoki` を出力せよ。

## 题目大意
非负整数 $x,y$ 的最大公约数记为 $\gcd(x,y)$，规定 $\gcd(x,0)=\gcd(0,x)=x$。

黑板上写了 $N$ 个整数 $A_1,A_2,...,A_N$，这 $N$ 个数的最大公约数是 $1$。Takahashi 和 Aoki 在玩游戏，有一个变量 $G$ 初值为 $0$，他们轮流进行以下操作：

> 从黑板上选择一个数 $a$，必须满足 $\gcd(a,G)\ne 1$，从黑板上擦掉这个数，并将 $G$ 的值改为 $\gcd(a,G)$。

Takahashi 先手，谁无法操作就输了，两人都采取最优策略。

请你对于 $i=1,2,..,N$ 分别判断，假如第一步 Takahashi 选择的数是 $A_i$，最后谁会获胜。

```input1
4
2 3 4 6
```

```output1
Takahashi
Aoki
Takahashi
Aoki
```

```input2
4
2 155 155 155
```

```output2
Takahashi
Takahashi
Takahashi
Takahashi
```

```input3
20
2579 25823 32197 55685 73127 73393 74033 95252 104289 114619 139903 144912 147663 149390 155806 169494 175264 181477 189686 196663
```

```output3
Takahashi
Aoki
Takahashi
Aoki
Takahashi
Takahashi
Takahashi
Takahashi
Aoki
Takahashi
Takahashi
Aoki
Aoki
Aoki
Aoki
Aoki
Takahashi
Takahashi
Aoki
Takahashi
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 2\ \leq\ A_i\ \leq\ 2\ \times\ 10^5 $
- $ N $ 個の整数 $ A_i\ (1\leq\ i\ \leq\ N) $ の最大公約数は $ 1 $
- 与えられる入力はすべて整数
 
### Sample Explanation 1

例えば高橋君が最初の手番で $ 4 $ 番目の整数 $ A_4=6 $ を選んだ場合、青木君が $ 2 $ 番目の整数 $ A_2=3 $ を選ぶと $ G=3 $ となります。この後高橋君が選べる整数は存在しないので、青木君の勝利となります。よって $ 4 $ 行目には `Aoki` を出力します。

### Sample Explanation 2

黒板には同じ整数が複数個書かれていることがあります。

