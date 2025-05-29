## ��Ŀ����
The Windblume Festival in Mondstadt is coming! People are preparing windblumes for Barbatos and for those they love and adore. The Windblume Festival is also an opportunity to improve the relationships people have.

![](https://cdn.luogu.com.cn/upload/image_hosting/nbhhi3bg.png)

During the festival, a famous game will be played every year, invented by Jean, the Acting Grand Master of the Knights of Favonius. In the game, $n$ players numbered from $1$ to $n$ stand in a circle, each holding an integer with them. Each turn, one player will be removed. The game will end when there is only one player left.

For each turn, let $k$ be the number of players remaining and $a_i$ be the integer player $i$ holds. Two adjacent players, $x$ and $(x \bmod k + 1)$ are selected and player $(x \bmod k + 1)$ is removed from the game. Player $x$'s integer will then change from $a_x$ to $(a_x - a_{x \bmod k + 1})$. Player $y$ in this turn will become player $(y - 1)$ in the next turn for all $x < y \le k$, though the integer they hold will not change.

Jean wants to know the maximum possible integer held by the last remaining player in the game by selecting the players in each round optimally.

## �����ʽ
There are multiple test cases. The first line of the input contains one integer $T$ indicating the number of test cases. For each test case:

The first line contains one integer $n$ ($1 \le n \le 10^6$) indicating the initial number of players.

The next line contains $n$ integers $a_i$ ($-10^9 \le a_i \le 10^9$) where $a_i$ is the integer held by player $i$ at the beginning.

It is guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.

## �����ʽ
For each test case output one line containing one integer indicating the maximum possible integer.

## ��Ŀ����
��һ������Ϊ $n$ ������������ $a$, ÿ�β�����������ѡ��һ���±� $x$���� $ a_x = a_x - a_{(x\bmod n)+1}$��֮���Ƴ� $a_{(x\bmod n)+1}$��
  
����ʣ��һ��Ԫ�أ�Ҫ��������Ԫ�ء�

���ݷ�Χ $1\le n\le10^6,-10^9\le a_i\le 10^9$��

```input1
5
4
1 -3 2 -4
11
91 66 73 71 32 83 72 79 84 33 93
12
91 66 73 71 32 83 72 79 84 33 33 93
13
91 66 73 71 32 83 72 79 84 33 33 33 93
1
0

```

```output1
10
713
746
779
0

```

## ��ʾ
For the first sample test case follow the strategy shown below, where the underlined integers are the integers held by the players selected in each turn.

$\{\underline{1}, -3, 2, \underline{-4}\}$ (select $x = 4$) $\to$ $\{-3, \underline{2, -5}\}$ (select $x = 2$) $\to$ $\{\underline{-3, 7}\}$ (select $x = 2$) $\to$ $\{10\}$.

