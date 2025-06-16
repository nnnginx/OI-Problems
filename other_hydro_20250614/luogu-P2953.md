## ��Ŀ����
Bessie is playing a number game against Farmer John, and she wants you to help her achieve victory.

Game i starts with an integer N\_i (1 <= N\_i <= 1,000,000). Bessie goes first, and then the two players alternate turns. On each turn, a player can subtract either the largest digit or the smallest non-zero digit from the current number to obtain a new number. For example, from 3014 we may subtract either 1 or 4 to obtain either 3013 or 3010, respectively. The game continues until the number becomes 0, at which point the last player to have taken a turn is the winner.

Bessie and FJ play G (1 <= G <= 100) games. Determine, for each game, whether Bessie or FJ will win, assuming that both play perfectly (that is, on each turn, if the current player has a move that will guarantee his or her win, he or she will take it).

Consider a sample game where N\_i = 13. Bessie goes first and takes 3, leaving 10. FJ is forced to take 1, leaving 9. Bessie takes the remainder and wins the game.

�����Լ������һ��������Ϸ��������Ҫ���������

��Ϸһ��������G(1��G��100)������i����Ϸ��ʼ��һ��������Ni(l��Ni��1,000,000)����

Ϸ�����������ģ�˫����������������ǰ�����ּ�ȥһ����������������ǵ�ǰ���ֵ�������룬Ҳ��������С�ķ�0���룮���統ǰ������3014�������߿��Լ�ȥ1���3013��Ҳ���Լ�ȥ4���3010�����ɴβ���֮��������ֻ���0����ʱ�����ٲ�����һ��Ϊ��ң�    ���������ȿ�ʼ��������������Լ�����㹻������ִ����õĲ��ԣ������������Ӯ�ң�

���磬һ����Ϸ��ʼ��13.���罫13��ȥ3���10��Լ��ֻ�ܽ�10��ȥ1���9�������ٽ�9��ȥ9���0�������Ӯ��


## �����ʽ
\* Line 1: A single integer: G

\* Lines 2..G+1: Line i+1 contains the single integer: N\_i


## �����ʽ
\* Lines 1..G: Line i contains 'YES' if Bessie can win game i, and 'NO' otherwise.


```input1
2 
9 
10 

```

```output1
YES 
NO 

```

## ��ʾ
For the first game, Bessie simply takes the number 9 and wins. For the second game, Bessie must take 1 (since she cannot take 0), and then FJ can win by taking 9.


