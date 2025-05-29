## ��Ŀ����
Bessie and her friends are playing hoofball in the annual Superbull championship, and Farmer John is in charge of making the tournament as exciting as possible. A total of $N$ $(1 <= N <= 2000)$ teams are playing in the Superbull. Each team is assigned a distinct integer team ID in the range 1...2^30-1 to distinguish it from the other teams. The Superbull is an elimination tournament -- after every game, Farmer John chooses which team to eliminate from the Superbull, and the eliminated team can no longer play in any more games. The Superbull ends when only one team remains.

Farmer John notices a very unusual property about the scores in matches! In any game, the combined score of the two teams always ends up being the bitwise exclusive OR (XOR) of the two team IDs. For example, if teams 12 and 20 were to play, then 24 points would be scored in that game, since 01100 XOR 10100 = 11000.

Farmer John believes that the more points are scored in a game, the more exciting the game is. Because of this, he wants to choose a series of games to be played such that the total number of points scored in the Superbull is maximized. Please help Farmer John organize the matches.

## �����ʽ
The first line contains the single integer $N$. The following $N$ lines contain the N team IDs.

## �����ʽ
Output the maximum possible number of points that can be scored in the Superbull.

## ��Ŀ����
### ��Ŀ����

Bessie ����������������һ��һ�ȵ� Superbull �������б�����Farmer John �����ñ��������ܾ��ʡ��ܹ��� $N$ $(1 \leq N \leq 2000)$ ֧����μ� Superbull��ÿ֧���鶼��������һ��Ψһ���������� ID����Χ�� $1 \ldots 2^{30}-1$ ֮�䣬�������ֲ�ͬ���顣Superbull ����̭�Ʊ�������ÿ��������Farmer John ��ѡ����̭����һ֧���飬����̭�Ķ��齫���ٲ��������������ֻʣһ֧����ʱ��Superbull ������

Farmer John ���ֱ����÷���һ���������ʣ�����һ�������У���֧����ĵ÷��ܺ����ǵ������� ID �İ�λ���XOR�������磬������ 12 �� 20 ��������ó������ܵ÷�Ϊ $24$����Ϊ $01100 \oplus 10100 = 11000$���� $12 \oplus 20 = 24$����

Farmer John ��Ϊ�����ܵ÷�Խ��Խ���ʡ���ˣ���ϣ������һϵ�б�����ʹ�� Superbull ���б������ܵ÷���󻯡����������Ʊ���������

### �����ʽ

��һ�а������� $N$���������� $N$ ��ÿ�а���һ������ ID��

### �����ʽ

��� Superbull ���б������ܻ�õ�����ܵ÷֡�

### ˵��/��ʾ

**�����������**��  
һ�ֻ�� 37 �ֵķ������£�  
1. Farmer John �ö��� 3 �� 9 ������ѡ����̭ 9����ʱʣ�����Ϊ 6��9��10  
2. �ö��� 6 �� 9 ������ѡ����̭ 9����ʱʣ�����Ϊ 6 �� 10  
3. ����ö��� 6 �� 10 ����  
�ܵ÷�Ϊ $(3 \oplus 9) + (6 \oplus 9) + (6 \oplus 10) = 10 + 15 + 12 = 37$��

**���ڰ�λ���**��  
��λ������㣨���� $\oplus$������������������ÿһλ�����߼������������ҽ���ĳһλ����������ͬʱ������ĸ�λΪ 1�����磺  
$10100$��ʮ���� 20��$\oplus$ $01100$��ʮ���� 12��$= 11000$��ʮ���� 24��

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

## ��ʾ
OUTPUT DETAILS: One way to achieve 37 is as follows: FJ matches teams 3 and 9, and decides that 9 wins, so teams 6, 9, and 10 are left in the tournament. He then matches teams 6 and 9, and lets team 6 win. Teams 6 and 10 are then left in the tournament. Finally, teams 6 and 10 face off, and team 10 wins. The total number of points scored is (3 XOR 9) + (6 XOR 9) + (6 XOR 10) = 10 + 15 + 12 = 37.

NOTE: The bitwise exclusive OR operation, commonly denoted by the ^ symbol, is a bitwise operation that performs the logical exclusive OR operation on each position in two binary integers. The result in each position is 1 if only the first bit is 1 or only the second bit is 1, but is 0 if both bits are 0 or both are 1. For example: 10100 (decimal 20) XOR 01100 (decimal 12) = 11000 (decimal 24)

[Problem credits: Alex Yang, 2015] 

