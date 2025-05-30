## 题目描述
[problemUrl]: https://atcoder.jp/contests/jsc2019-qual/tasks/jsc2019_qual_d

AtCoder 本社は $ N $ 室の部屋からなる施設であり、部屋には $ 1 $ から $ N $ の番号がついています。どの $ 2 $ 部屋の間にも、それらを直接結ぶ通路が $ 1 $ 本通っています。

社長の高橋君はセキュリティのため、全ての通路に **レベル** を設定するようあなたに依頼しました。ここで、レベルは正の整数値であり、以下の条件を満たさなければなりません。

- 全ての部屋 $ i\ (1\ \leq\ i\ \leq\ N) $ について、部屋 $ i $ から出発し、レベルが等しい通路のみをいくつか通って部屋 $ i $ に戻るとき、通路を通る回数は必ず偶数になる。

あなたの仕事は、通路ごとのレベルをうまく設定して、レベルの最大値を最小化することです。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ N $

## 输出格式
目的を達成するような設定の仕方を次のように出力してください。

> $ a_{1,2} $ $ a_{1,3} $ ... $ a_{1,N} $ $ a_{2,3} $ ... $ a_{2,N} $ . . . $ a_{N-1,N} $

ここで、$ a_{i,j} $ は部屋 $ i $ と部屋 $ j $ の間の通路に設定するレベルです。

答えが複数ありえる場合、どれを出力してもかまいません。

## 题目大意
### 题目描述

AtCoder 的最高级办公室由 $N$ 个房间组成，房间编号 $1\sim N$，任意两个房间之间有一条走廊。

由于一些原因，Takahashi 需要给每一条走廊确定一个正整数作为安全程度，满足：

- 从任意一个房间出发，仅经过相同安全系数的走廊回到这个房间，穿过的走廊数恒为偶数。

你需要构造一组给每条走廊确定安全程度的方案，使得安全程度的最大值最小。

### 输入格式

输入一行一个正整数 $N$（$2\le N\le 500$）表示房间个数。

### 输出格式

输出一种满足条件的方案，格式如下：

> $a_{1,2}\quad a_{1,3}\quad \ldots \quad a_{1,N}\\a_{2,3}\quad \ldots \quad a_{2_N}\\\vdots\\a_{N-1,N}$

其中 $a_{i,j}$ 表示房间 $i$ 和 $j$ 间的走廊的安全程度。

若有多组符合条件的解，输出任意一组。

### 样例解释

如图为一种可行方案。例如，从房间 $2$ 出发，路线 $2\rightarrow 3\rightarrow 2\rightarrow 3\rightarrow 2\rightarrow 1\rightarrow 2$ 经过了 $6$ 条安全程度均为 $1$ 的走廊回到房间 $2$，且 $6$ 为偶数，符合条件。

```input1
3
```

```output1
1 2
1
```

## 提示
### 制約

- $ N $ は $ 2 $ 以上 $ 500 $ 以下の整数

### Sample Explanation 1

この出力例は下の画像のようになります。 !\[\](https://img.atcoder.jp/jsc2019-qual/D-sample.png) たとえば部屋 $ 2 $ から出発して、$ 2\ \to\ 3\ \to\ 2\ \to\ 3\ \to\ 2\ \to\ 1\ \to\ 2 $ という経路でレベル $ 1 $ の通路のみを通って元の部屋に戻るとき、通路を通る回数は $ 6 $ 回です。

