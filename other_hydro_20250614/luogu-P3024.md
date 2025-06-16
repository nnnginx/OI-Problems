## ��Ŀ����
One day, Bessie decides to challenge Farmer John to a game of 'Cow Checkers'. The game is played on an M\*N (1 <= M <= 1,000,000; 1 <= N <= 1,000,000) checkerboard that initially contains a single checker piece on the checkboard square coordinates (X, Y) (0 <= X < M; 0 <= Y < N). The bottom leftmost square of the checkerboard has

coordinates (0, 0), and the top rightmost square has coordinates (M-1, N-1). Bessie always moves first, and then the two players alternate turns.  Each turn comprises one of three types of moves:

1) Move the checker piece to any square on the same row to the left of its current position.

2) Move the checker piece to any square on the same column below its current position.

3) Move the checker piece to any spot k squares below and k squares to the left of the current square (where k is any positive integer such that this new spot is still on the checkerboard).

The first player unable to make a move (i.e., because the checker is at (0, 0)) loses. Given that Bessie always goes first, determine who will win the game if both play optimally.

Play and report the winner for T games (1 <= T <= 1,000) reading in a new X,Y starting value for each new game.

��һ�죬Bessie׼����һ��������ţ�������Ϸ������սFarmer John��


�����Ϸ�����̴�СΪ M\*N (1 <= M <= 1,000,000; 1 <= N <= 1,000,000) �����������ֻ��һ�������ڣ�x,y�������̵����½������ǣ�0,0�������Ͻǵ������ǣ�M-1��N-1����


ÿ����ϷBessie���ǵ�һ����ʼ��֮��������������


ÿ�������ʱ���������߷���


1.���������ⲽ


2.���������ⲽ


3.������k��Ȼ��������k����k�����ȡֵ��ֻҪ���߳����̣�


�����ߵ���0,0������Ϊʤ���ߡ�


��Ϸ����T�Σ�ÿ�ζ������һ���µ����꣨x,y���������ÿһ��Ӯ�ҵ����֡�


## �����ʽ
\* Line 1: Two space-separated integers: M and N

\* Line 2: A single integer: T

\* Lines 3..T+2: Two space-separated integers: X and Y

��һ�У�M N


�ڶ��У�T


�����е���T+2��:��һ�ֵ�X Y


## �����ʽ
\* Lines 1..T: Should contain either 'Farmer John' or 'Bessie' depending on who wins each  game.

��T�У�ÿһ�������һ�ֵ�Ӯ��


```input1
3 3 
1 
1 1 

```

```output1
Bessie 

```

## ��ʾ
Farmer John and Bessie are playing one game on a 3\*3 checkerboard with the checker piece initially at (1, 1) (i.e. at the center of the board).


Bessie initially can only move the checker piece to either (1, 0) or (0, 1), or (0, 0). Bessie can immediately win by moving the piece to (0, 0).


����ڣ�1,1����һ��ʼ������ѡ��1,0��,��0,1������0,0��ֻҪBessie�ڿ�ʼʱ�������Ƶ���1,0����0,1�����ͱ�ʤ���ɡ�


��л@ 2014nhc  �ṩ�ķ���


