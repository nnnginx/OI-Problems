## 题目描述

A wizard is in a labyrinth where there are $V$ rooms and $V-1$ doors connecting some pairs of rooms in both directions，in such a way that there is always a sequence of doors one can traverse to go from a room to any other room．
Additionally，there are $C$ locks and $C$ keys of $C$ different colours（one of each）in some of the doors and rooms of the maze，respectively；each door has at most one lock，and there is at most one key placed in each room．It should be an easy matter for the wizard to bypass the lock system，were it not for the fact that he forgot his spell book，without which his wizardry is utterly useless．The wizard is currently in room $X$，and he wants to get his spell book，located in room $Y$，without taking too long．At every step he may go to an adjacent room through one of the doors．Of course，if the door is locked，he needs to be carrying the key of the same colour as the lock（unless，of course，that door has already been unlocked）．The wizard can carry only one key at a time and after picking up a key it is not possible for him to drop it somewhere in the maze in order to take it again afterwards．Once a door has been unlocked，the key is thrown away since it is no longer any use．
Given the maze and the positions of the $C$ keys and $C$ locks，determine how to reach $Y$ from $X$，if possible．Any path whose length does not exceed $4 \times(C＋1)\times V$ is acceptable．

一个巫师目前正被困在一个有着 $V$ 个房间和 $V-1$ 个连接着某些房间的门的迷宫里。当然，门都是可双向通行的，且总是可以从一个房间经过一系列的门到达另一个房间。在某些房间里有钥匙，在某些门上有锁。

锁和钥匙共有 $C$ 种颜色，每一种颜色都对应着唯一的钥匙和唯一的锁，一把钥匙可以开相同颜色的锁。一个门上最多有一把锁，一个房间里最多有一把钥匙。如果巫师没有丢失咒语书，锁对巫师形同虚设。现在，丢失了咒语书的巫师发不出任意一个巫术。

巫师目前在 $X$ 号房间。他希望不花太多的时间就可以拿到他落在 $Y$ 房间的咒语书。他一步可以走到相邻的房间。当然喽，如果门上有锁，他还必须带上和锁同色的钥匙（如果锁被打开就没必要了）。巫师一次只能带一把钥匙，并且一旦拿起了一把钥匙，就不能把它随意地丢在迷宫里的某一个位置并在之后的某一时间捡起它。只有当钥匙开了门以后才能丢弃它。

给出迷宫的形态和 $C$ 个钥匙和 $C$ 个锁的位置。如果可以从 $X$ 到 $Y$，请给出方案。任何一个不超过 $4 \times(C + 1)\times V$ 步的方案都是可以被接受的。

## 输入格式

**本题有多组数据**

The first line of each case contains four integers：the number $V$ of rooms in the maze ，the number $C$ of locks ，and rooms $X$ and $Y$ numbered $0,1,\dots ,V-1$．

Then comes a（possibly empty）line with $C$ integers indicating the location of each of the keys，in order of increasing colour．

The next $V-1$ lines describe the maze：each contains three integers $A,B,L$，meaning that there is a door between rooms $A$ and $B$ which can be unlocked with the key of colour $L$，if $0 \le L < C$ ；a value of $-1$ for $L$ indicates that no lock is needed．

The last line has $V,C,X,Y = 0,0,0,0$．

每一个测试数据的第一行包含4个整数：$V$ 代表房间数, $C$ 代表颜色数，和 $X，Y$。房间被编号为 $0，1 \dots V-1。

接下来的一行包含了 $C$ 的整数表示 $C$ 把钥匙的位置，钥匙的颜色是递增的。

接下来的 $V-1$ 行描述了迷宫的形态：每一行包含了三个整数 $A,B,L$。表示在房间 $A$ 与 $B$ 间有一道双向门，门上挂着一把颜色为 $L$ 的锁；若 $L = -1$ ，表示门没锁。

最后一行为 $V,C,X,Y = 0,0,0,0$

## 输出格式

**每一个输入数据对应一行输出。**

如果没有解，输出 `Impossible`。否则按 $L:V_0 \dots V_L$ 的格式输出。$L$ 是总步数，应该有 $L \le 4 \times （C + 1） \times V$。

$X = V_0,V_1,\dots,V_{L-1}$，$V_L = Y$ 是一次经过的 $L + 1$ 个点。任意两对数应该用一个空格分开，具体请参见样例。

```input1
1 0 0 0
3 1 0 2
1
0 1 -1
0 2 0
3 2 0 2
1 2
0 1 1
0 2 0
5 3 0 4
2 0 3
0 1 0
0 2 -1
1 3 1
2 4 2
0 0 0 0
```

```output1
0: 0
3: 0 1 0 2
Impossible
10: 0 2 0 1 0 1 3 1 0 2 4
```

## 题目来源

鸣谢李青林

## 数据规模与约定

$100\%$ 的数据满足：$1 \le V \le 1.5 \times 10^3$，$0 \le C < V$。