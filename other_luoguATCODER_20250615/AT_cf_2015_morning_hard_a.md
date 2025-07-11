# AT_cf_2015_morning_hard_a 一次元オセロ

## 题目描述

小A在玩一维奥赛罗。一维奥赛罗是一种在无限长的一行格子内摆放棋子的游戏。棋子的一面是黑色，而另一面是白色。

它的规则如下：

1. 首先按照白色棋子  $A_1$ 个，黑色棋子  $A_2$ 个，白色棋子  $A_3$ 个，...，白色棋子  $A_N$ 个这样的顺序进行摆放。
2. 把黑色的棋子放在任意一个空闲位置。这时，所放置的位置左右的2格中必须正好1格有白色的棋子。
3. 将距离放置的黑色棋子最近的其他黑色棋子之间的白色陀螺全部翻过来做成黑色的棋子，这样的若干对黑色棋子总是唯一确定的。
4. 黑白棋子交换。
5. 重复  $2$～  $4$。
6.   步骤$3$ 或  $4$结束时，如果所有的棋子颜色相同，则游戏结束。

因为要把很多棋子翻过来是很困难的，所以小A想把棋子翻过来的次数减少一些。请在游戏结束前，求小A翻转棋子的次数之和的最小值。

## 输入格式

第一行是一个整数  $N(3\leqslant N<10^5,N$ 为奇数 $)$。

第二行是  $N$ 个整数，分别表示  $A_1,A_2,...,A_N$。

## 输出格式

游戏结束时小A反转棋子的最少次数。输出这个数。

## 输入输出样例 #1

### 输入 #1

```
5
1 2 3 4 5
```

### 输出 #1

```
20
```

## 输入输出样例 #2

### 输入 #2

```
9
100000000 20 15 11 14 20 15 11 15
```

### 输出 #2

```
554
```

## 说明/提示

像图片中所示的一样反转棋子，一共反转了  $1+4+5+10=20$ 次棋子，使得游戏结束。

翻译By @[liuziwen0224](/user/141683)