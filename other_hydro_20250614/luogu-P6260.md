## ��Ŀ����
### Warning: If you submit a malicious program, you will be banned.
### ���棺�����ύ���⽫����š�


## ��Ŀ����
A group of friends has just played a round of miniature golf. Miniature golf courses consist of a number of holes. Each player takes a turn to play each hole by hitting a ball repeatedly until it drops into the hole.
A player's score on that hole is the number of times they hit the ball. 
To prevent incompetent players slowing down the game too much, there is also an upper limit $l$ (a positive integer) on the score: if a player has hit the ball $l$ times without the ball dropping into the hole, the score for that hole is recorded as $l$ and that player's turn is over. The total score of each player is simply the sum of their scores on all the holes. Naturally, a lower score is considered better.

There is only one problem: none of the players can remember the value of the integer $l$. They decide that they will not apply any upper limit while playing, allowing each player to keep playing until the ball
drops into the hole. After the game they intend to look up the value of $l$ and adjust the scores, replacing any score on a hole that is larger than $l$ with $l$.

The game has just finished, but the players have not yet looked up $l$. They wonder what their best possible ranks are. For this problem, the rank of a player is the number of players who achieved an equal or lower total score after the scores are adjusted with $l$. For example, if the adjusted scores of the players are $3, 5, 5, 4,$ and $3$, then their ranks are $2, 5, 5, 3$ and $2$ respectively.

Given the scores of the players on each hole, determine the smallest possible rank for each player.

## �����ʽ
The first line of input contains two integers $p$ and $h$, where $p$ $(2 \leq p \leq 500)$ is the number of players and $h$ $(1 \leq h \leq 50)$ is the number of holes. The next $p$ lines each contain $h$ positive integers. The $j^{th}$ number on the $i^{th}$ of these lines is the score for player $i$ on hole $j$, and does not exceed $10^9$.


## �����ʽ
Output a line with the minimum possible rank for each player, in the same order as players are listed in the input.

## ��Ŀ����
### ��Ŀ����
������������һ��С�͵ĸ߶�������С�͵ĸ߶����������ɸ�����ɵġ�ÿ����������������Ϸ����ͣ�ػ���ֱ�����䵽ÿ����������һ�����ϵĵ÷���������Ĵ�����Ϊ�˷�ֹ���ҵ���Ұ���Ϸ�ٶȷ���̫�࣬��Ϸ������Ҳ���һ������$l$��һ���������������Ʒ��������һ�������һ�������Ѿ�����$l$�Σ�������û���䵽�����ô��������������ϵĵ÷־���$l$�����������ҵĻغϾͽ����ˡ�һ����ҵ��ܵ÷־������ڸ������ϵĵ÷�֮�͡���Ȼ�أ��������Ϸ�У���Խ��Խ�á�

������һ�����⣺û����Ҽǵ�$l$��ֵ������Ǿ��������ʱ������$l$��ֵ������ÿ����Ҳ��ϻ���ֱ����������������Ϸ������׼������$l$��ֵ����������Щ�ڶ��ϵķ�������$l$��ֵ��

��Ϸ�����ˣ������ǻ�û������$l$��������֪���Լ������������ʲô��һ���˵����������������У��÷ֱ�����˵ͻ���������ȵ������������Լ��������磬������˵ĵ÷ֱַ��� $3,5,5,4,3$����ô���ǵ��������� $2,5,5,3,2$��

����ÿ�������ÿ�����ϵĵ÷֣�Ϊÿһ����������С�Ŀ��ܵ�������

### �����ʽ

��һ�У��������� $p$ �� $h$��$p$��$2 \le p \le 500$������Ҹ�����$h$��$1 \le h \le 50$���Ƕ��ĸ�����

������$p$�У�ÿ��$h$������������$i$�е�$j$�е�����ʾ��$i$������ڵ�$j$�����ϵĵ÷֣���Щ�������ᳬ��$10^9$��

### �����ʽ

��� $p$ �У�ÿ��һ������������ $i$ �б�ʾ�� $i$ ����ҵ���С������

### ˵��/��ʾ

��Դ��ICPC World Finals 2019 Problem J 

��Ŀ���ƣ�Miniature Golf

```input1
3 3
2 2 2
4 2 1
4 4 1
```

```output1
1
2
2
```

```input2
6 4
3 1 2 2
4 3 2 2
6 6 3 2
7 3 4 3
3 4 2 4
2 3 3 5
```

```output2
1
2
5
5
4
3

```

## ��ʾ
Source: ICPC World Finals 2019 Problem J: Miniature Golf.

