## 题目描述
Bessie and her friends are playing hoofball in the annual Superbull championship, and Farmer John is in charge of making the tournament as exciting as possible. A total of $N$ $(1 <= N <= 2000)$ teams are playing in the Superbull. Each team is assigned a distinct integer team ID in the range 1...2^30-1 to distinguish it from the other teams. The Superbull is an elimination tournament -- after every game, Farmer John chooses which team to eliminate from the Superbull, and the eliminated team can no longer play in any more games. The Superbull ends when only one team remains.

Farmer John notices a very unusual property about the scores in matches! In any game, the combined score of the two teams always ends up being the bitwise exclusive OR (XOR) of the two team IDs. For example, if teams 12 and 20 were to play, then 24 points would be scored in that game, since 01100 XOR 10100 = 11000.

Farmer John believes that the more points are scored in a game, the more exciting the game is. Because of this, he wants to choose a series of games to be played such that the total number of points scored in the Superbull is maximized. Please help Farmer John organize the matches.

## 输入格式
The first line contains the single integer $N$. The following $N$ lines contain the N team IDs.

## 输出格式
Output the maximum possible number of points that can be scored in the Superbull.

## 题目大意
### 题目描述

Bessie 和她的朋友们正在一年一度的 Superbull 锦标赛中比赛，Farmer John 负责让比赛尽可能精彩。总共有 $N$ $(1 \leq N \leq 2000)$ 支队伍参加 Superbull。每支队伍都被分配了一个唯一的整数队伍 ID，范围在 $1 \ldots 2^{30}-1$ 之间，用于区分不同队伍。Superbull 是淘汰制比赛——每场比赛后，Farmer John 会选择淘汰其中一支队伍，被淘汰的队伍将不再参与后续比赛。当只剩一支队伍时，Superbull 结束。

Farmer John 发现比赛得分有一个特殊性质：任意一场比赛中，两支队伍的得分总和总是等于两队 ID 的按位异或（XOR）。例如，若队伍 12 和 20 比赛，则该场比赛总得分为 $24$，因为 $01100 \oplus 10100 = 11000$（即 $12 \oplus 20 = 24$）。

Farmer John 认为比赛总得分越高越精彩。因此，他希望安排一系列比赛，使得 Superbull 所有比赛的总得分最大化。请帮助他设计比赛方案。

### 输入格式

第一行包含整数 $N$。接下来的 $N$ 行每行包含一个队伍 ID。

### 输出格式

输出 Superbull 所有比赛可能获得的最大总得分。

### 说明/提示

**输出样例解释**：  
一种获得 37 分的方案如下：  
1. Farmer John 让队伍 3 和 9 比赛，选择淘汰 9，此时剩余队伍为 6、9、10  
2. 让队伍 6 和 9 比赛，选择淘汰 9，此时剩余队伍为 6 和 10  
3. 最后让队伍 6 和 10 比赛  
总得分为 $(3 \oplus 9) + (6 \oplus 9) + (6 \oplus 10) = 10 + 15 + 12 = 37$。

**关于按位异或**：  
按位异或运算（记作 $\oplus$）对两个二进制数的每一位进行逻辑异或操作。当且仅当某一位上两个数不同时，结果的该位为 1。例如：  
$10100$（十进制 20）$\oplus$ $01100$（十进制 12）$= 11000$（十进制 24）

```input1
4
3
6
9
10
```

```output1
37
```

## 提示
OUTPUT DETAILS: One way to achieve 37 is as follows: FJ matches teams 3 and 9, and decides that 9 wins, so teams 6, 9, and 10 are left in the tournament. He then matches teams 6 and 9, and lets team 6 win. Teams 6 and 10 are then left in the tournament. Finally, teams 6 and 10 face off, and team 10 wins. The total number of points scored is (3 XOR 9) + (6 XOR 9) + (6 XOR 10) = 10 + 15 + 12 = 37.

NOTE: The bitwise exclusive OR operation, commonly denoted by the ^ symbol, is a bitwise operation that performs the logical exclusive OR operation on each position in two binary integers. The result in each position is 1 if only the first bit is 1 or only the second bit is 1, but is 0 if both bits are 0 or both are 1. For example: 10100 (decimal 20) XOR 01100 (decimal 12) = 11000 (decimal 24)

[Problem credits: Alex Yang, 2015] 

