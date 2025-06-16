## ��Ŀ����
The cows have taken up the game of checkers with a vengeance.

Unfortunately, despite their unlimited enjoyment of playing, they are terrible at the endgame and want your help.

Given an NxN (4 <= N <= 500) checkboard, determine the optimal set of moves (i.e., smallest number of moves) to end the game on the next move. Checkers move only on the '+' squares and capture by jumping 'over' an opponent's piece in the traditional way. The piece is removed as soon as it is jumped.  See the example below where N=8:

```cpp
- + - + - + - +  The K's mark Bessie's kings; the o's represent the 
+ - + - + - + -  opponent's checkers. Bessie always moves next. The 
- + - K - + - +  Kings jump opponent's checkers successively in any 
+ - + - + - + -  diagonal direction (and removes pieces when jumped). 
- o - o - + - + 
+ - K - + - + -  For this board, the best solution requires the lower 
- o - + - + - +  left King to jump successively across all three of the 
+ - K - + - K -  opponents' checkers, thus ending the game (moving K marked as >K<): 
Original          After move 1       After move 2        After move 3 
- + - + - + - +     - + - + - + - +    - + - + - + - +     - + - + - + - + 
+ - + - + - + -     + - + - + - + -    + - + - + - + -     + - + - + - + - 
- + - K - + - +     - + - K - + - +    - + - K - + - +     - + - K - + - + 
+ - + - + - + -     + - + - + - + -    + ->K<- + - + -     + - + - + - + - 
- o - o - + - +     - o - o - + - +    - + - o - + - +     - + - + - + - + 
+ - K - + - + -    >K<- K - + - + -    + - K - + - + -     + - K ->K<- + - 
- o - + - + - +     - + - + - + - +    - + - + - + - +     - + - + - + - + 
+ ->K<- + - K -     + - + - + - K -    + - K - + - K -     + - K - + - K - 

The moves traversed these squares: 
1 2 3 4 5 6 7 8           R C 
1 - + - + - + - +    start: 8 3 
2 + - + - + - + -    move:  6 1 
3 - + - K - + - +    move:  4 3 
4 + - * - + - + -    move:  6 5 
5 - o - o - + - + 
6 * - K - * - + - 
7 - o - + - + - + 
8 + - K - + - K - 
```
Write a program to determine the game-ending sequence for an NxN input board if it exists. There is at least a king and at least one opponent piece on the board. The king can jump a piece on every move of the optimal solution.

POINTS: 330


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains N characters (each one of: '-', '+', 'K', or 'o') that represent row i of a proper checkboard. Line 2 always begins with '-'.


## �����ʽ
\* Lines 1..?: If there is no winning sequence of jump, output

'impossible' on a line by itself. If such a sequence exists, each line contains two space-separated integers that represent successive locations of a king whose moves will win the game. Any such sequence is acceptable.


## ��Ŀ����
## ��Ŀ����

��ţ�ڼ��ҵ������塣

���ҵ��ǣ�����������úܿ��ģ������������׶κܼ��ѣ���Ҫ��İ�����

����һ�� $N \times N(4 \le N \le 500)$ �����̣�ȷ�������������ԡ���**���жԷ�����**���ƶ��������ٵ�·����

�ƶ�����

1. �ضԽ��߷����ƶ���

1. ����Խ���Է����ӵ�����һ��λ�ӡ�

1. ��Խ���ĶԷ�������Ϊ���ԡ�����

1. ����ֻ�ܲٿ���������**1**������**����**�ƶ���

�뿴��������ӣ����� $N=8$ ��

1. �������ӱ��Ϊ o

1. �����Ĺ������Ϊ K

1. �����ƶ��Ĺ������Ϊ >K<

```
��ʼ״̬             �ƶ�һ�κ�          �ƶ����κ�           �ƶ����κ�
- + - + - + - +     - + - + - + - +    - + - + - + - +     - + - + - + - + 
+ - + - + - + -     + - + - + - + -    + - + - + - + -     + - + - + - + - 
- + - K - + - +     - + - K - + - +    - + - K - + - +     - + - K - + - + 
+ - + - + - + -     + - + - + - + -    + ->K<- + - + -     + - + - + - + - 
- o - o - + - +     - o - o - + - +    - + - o - + - +     - + - + - + - + 
+ - K - + - + -    >K<- K - + - + -    + - K - + - + -     + - K ->K<- + - 
- o - + - + - +     - + - + - + - +    - + - + - + - +     - + - + - + - + 
+ ->K<- + - K -     + - + - + - K -    + - K - + - K -     + - K - + - K - 

����ƶ���·�������Ϊ * ����

  1 2 3 4 5 6 7 8          �� �� 
1 - + - + - + - +    ���:  8  3 
2 + - + - + - + -    ·��:  6  1 
3 - + - K - + - +    ·��:  4  3 
4 + - * - + - + -    ·��:  6  5 
5 - o - o - + - + 
6 * - K - * - + - 
7 - o - + - + - + 
8 + - K - + - K - 
```

��дһ��������ȷ�������Ĺ������ƶ�·����������������һ��������һ���������ӡ�

### �����ʽ

��һ����һ������ $N$��

������ $N$ ����һ�� $N \times N$ �ľ���ÿ���ַ�֮��û�пո�

### �����ʽ

����һ��·�������ÿ�а��������ո�ָ�����������ʾһλ����������λ�á�

��û��������·��,��һ�����"impossible"��

```input1
8 
-+-+-+-+ 
+-+-+-+- 
-+-K-+-+ 
+-+-+-+- 
-o-o-+-+ 
+-K-+-+- 
-o-+-+-+ 
+-K-+-K- 

```

```output1
8 3 
6 1 
4 3 
6 5 

```

