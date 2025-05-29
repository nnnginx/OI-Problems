## 题目描述

This problem is based on the game of Black Vienna．In this version there are three players and $18$ cards labeled $A-R$．Three of the cards are set aside（hidden）and form the 「Black Vienna」 gang．The remaining cards are shuffled and dealt to the players so that each player has $5$ cards．Players never reveal their cards to each other．There is a separate deck of 「interrogation cards」 which contain three distinct letters in ascending order，ike $\text{ACG}$ or $\text{BHR}$．Turns rotate through players $1,2$ and $3$．On each player's turn，that player selects an interrogation card，puts it face up in front of another player，and that other player must indicate the total number of these cards being held，without saying which ones．All players see the result of the 「interrogation」. The play continues until a player deduces the three cards in the 「gang」．  
For example，suppose the cards are distributed as follows，and the game then proceeds：  

```
Player 1：DGJLP；Player 2：EFOQR；Player 3：ACHMN；Gang：BIK
Turn 1：Player 1 interrogates player 2 with BJK；answer 0
Turn 2：Player 2 interrogates player 3 with ABK；answer 1
Turn 3：Player 3 interrogates player 2 with DEF；answer 2
Turn 4：Player 1 interrogates player 2 with EIL；answer 1
Turn 5：Player 2 interrogates player 3 with FIP；answer 0
Turn 6：Player 3 interrogates player 1 with GMO；answer 1
Turn 7：Player 1 interrogates player 2 with OQR；answer 3
Turn 8：Player 2 interrogates player 3 with ADQ；answer 1
Turn 9：Player 3 interrogates player 1 with EGJ；answer 2
```

In fact，the game does not need to get to turn $9$．With enough thought，player 1 can deduce after turn $8$ that the gang is $BIK$．It is your job to analyse records of games and deduce the earliest time that the gang could be determined for sure．

Black Vienna游戏是当前很流行的桌面游戏，规则是这样的：有 $18$ 张牌，分别标着 $A-R$，游戏有三个人。游戏开始的时候每个人拿 $5$ 张牌，剩下三张牌隐藏起来，大家都只能看见自己手中的牌。之后，从第一个人到第三个人轮流拿一张“疑问牌”去问另外的一个人，“疑问牌”上有三个字母，那个人必须诚实地回答自己手中有多少疑问牌中的字母。哪个人能够最先推断出隐藏起来的牌是什么，那个人就取得胜利。现在你的任务是，给出三个人手上的牌和询问情况，你需要计算出最早在哪一次询问之后，有人能够推断出隐藏的牌。

## 输入格式

The input will consist of one to twelve data sets，followed by a line containing only $0$．  
The first line of a dataset contains the number，$t$，of turns reported．  
The next line contains four blank separated strings for the hands of players $1,2$ and $3$，followed by the cards for the gang．  
The remaining $t$ lines of the data set contain the data for each turn in order．Each line contains three blank separated tokens：the number of the player interrogated，the string of interrogation letters，and the answer provided．  
All letter strings will contain only capital letters from $A$ to $R$，in strictly increasing alphabetical order．The same interrogation string may appear in more than one turn of a game．

## 输出格式

There is one line of output for each data set．The line contains the single character `?` if no player can be sure of the gang after all the turns listed．If a player can determine the gang，the line contains the earliest turn after which one or more players can be sure of the answer．

```input1
9
DGJLP EFOQR ACHMN BIK
2 BJK 0
3 ABK 1
2 DEF 2
2 EIL 1
3 FIP 0
1 GMO 1
2 OQR 3
3 ADQ 1
1 EGJ 2
3
ABCDE FGHIJ KLMNO PQR
3 BKQ 1
1 ADE 3
2 CHJ 2
0
```

```output1
8
?
```

## 样例解释1

从第一个人角度看：

```
1 组: 2 BJK 0
 第二人：无 DGJLPBJK
 第三人：无 DGJLP

2 组: 3 ABK 1
 第二人：无 DGJLPBJK
 第三人：无 DGJLP，ABK 中有一个

3 组: 2 DEF 2
 第二人：无 DGJLPBJK，有 EF
 第三人：无 DGJLPEF，ABK 中有一个

4 组: 2 EIL 1
 第二人：无 DGJLPBJKIL，有 EF
 第三人：无 DGJLPEF，ABK 中有一个

5 组: 3 FIP 0
 第二人：无 DGJLPBJKIL，有 EF
 第三人：无 DGJLPEFIP，ABK 中有一个

6 组: 1 GMO 1 （对自己没有利用价值）

7 组：2 OQR 3
 第二人：无 DGJLPBJKIL，有 EFOQR
 第三人：无 DGJLPEFIPOQR，ABK 中有一个

8 组：3 ADQ 1
 第二人：无 DGJLPBJKIL，有 EFOQR
 第三人：无 DGJLPEFIPOQR，[ABK 中有一个，ADK 中有一个]
```

由括号部分可知：

```
 第二人：无 DGJLPBJKIL，有 EFOQR
 第三人：无 DGJLPEFIPOQRBK，有 A
```

此时，第一人知道自己和 2，3 都无 $\text{BIK}$，所以隐藏牌为 $\text{BIK}$。  
（2，3 人视角同上，前 $8$ 步无法得出结论）

## 数据规模与约定

$100\%$ 的数据满足：$2 \le t \le 15$。


