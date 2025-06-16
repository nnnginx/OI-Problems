## ��Ŀ����
Farmer John has long had a dispute with neighbor Farmer Tom over a group of V (1 <= V <= 1,000) pastures conveniently numbered 1..V. Both farmers currently graze their cows on the pastures; each pasture might be empty or might have a single cow which is owned by either Farmer John or Farmer Tom.

Farmer John's patience is at an end, and he wishes to settle the dispute with Farmer Tom by tipping over Tom's cows. Of course, he wants to strike first and to tip as many of Farmer Tom's cows as possible.

A total of E (1 <= E <= 5,000) bidirectional cowpaths connect pairs of pastures. No two pastures are connected by more than one cowpath; each path connects exactly two distinct pastures. Paths are described by their endpoints P1\_i and P2\_i (1 <= P1\_i <= V; 1 <= P2\_i <= V).

During his offense, each of Farmer John's cows can traverse a single cowpath if she wishes. Whether or not she chooses to traverse a cowpath, she can then (if she wishes) launch a cow tipping attack to a pasture connected to her pasture by a single cowpath, thus tipping the enemy cow on that pasture. Note that a cow can move and then attack -- but she is not able to attack and then move.

Each pasture can hold exactly one cow at a time; no cow can move to a pasture occupied by another cow, especially if it has been tipped. Of course, if a pasture is vacated, another cow can later move in to take its place. A tipped cow cannot be tipped again.

Farmer John wants to know two things:

\* How many of Farmer Tom's cows he can tip in the first salvo

of the war

\* How to command his cows to move and attack so as to tip

that maximal number of Farmer Tom's cows in that first salvo

Find the maximum number of cows that can be tipped and construct a sequence of move and attack commands to his cows that then obey the rules and tip that number of cows. Any such sequence is acceptable, as long as it tips the maximum number of Farmer Tom's cows.

Consider, for instance, a group of 5 pastures arranged in a line, with each pasture connected (via '--'; see diagram below) to its left and right neighbors (if they exist). In other words, there is a cowpath from Pasture 1 to Pasture 2, Pasture 2 to Pasture 3, etc. Farmer Tom ('T') has 2 cows, standing on pastures 1 and 4, while Farmer John ('J') has 2 cows standing on pastures 3 and 5 ('E' means empty):

1    2    3    4    5

T -- E -- J -- T -- J

In this case, Farmer John can tip both of Farmer Tom's cows by first moving his cow on Pasture 3 to Pasture 2, so that the pastures in order are now TJETJ. Farmer John can then have both of his cows attack to the left.  Note that although the cow in Pasture 3 could have attacked to the right without moving, the rightmost cow would then be unable to attack. The only valid solutions thus have the same move and attacks, although the order in which Farmer John commands his cows can vary slightly.

If you compute the correct maximum number but do not provide a sequence (or your sequence is wrong), you will get 50% of the points for that test case. A program will grade your output.

Partial feedback will be provided for your first 50 submissions.

## �����ʽ
\* Line 1: Two space separated integers: V and E

\* Line 2: A string of V characters (no spaces); character #i indicates whether pasture #i is empty ('E') or has a cow owned by Farmer John ('J') or Farmer Tom ('T')

\* Lines 3..E+2: Line i+2 contains two space separated integers: P1\_i and P2\_i


## �����ʽ
\* Line 1: A single integer, the maximum number of enemy cows Farmer John can have tipped

\* Lines 2.....: One of Farmer John's instructions to his cows (to be executed in the order given):

MOVE A B

or
ATTACK A B

where A is the vertex the cow occupies before taking the action and B is the vertex it is moving to or attacking, respectively. Note that when instructing a cow that has already moved to attack, the instruction specifies the location the cow is currently standing, not where it was originally.


## ��Ŀ����
### ��Ŀ����

���� $V$ ���㣬$E$ ���ߵ�����ͼ��
һ��ʼÿ�������� `T` ţ��`J` ţ������û�У�`E`����
`J` ţ���� `MOVE` ��һ�����ڵĵ㣬Ҳ���� `ATTACK` ���ڵ��ϵ�һ�� `T` ţ���������������ƣ�ֻ�ܰ��� `MOVE`,`ATTACK` ���� `MOVE` Ȼ�� `ATTACK` ���ַ�ʽ������
һ�� `T` ţ���ܱ� `ATTACK` һ�Σ��� `ATTACK` ����������ԭ�ء�
��Ҫ��֤����ʱ�̣�ÿ���������ҽ���һͷţ��
������ `T` ţ�� `ATTACK` ����������������һ�����еĲ���������

### �����ʽ

��һ���������� $V,E$����ʾ����ͼ�ĵ����ͱ�����
������һ�� $V$ ���ַ����� $i$ ���ַ���ʾ�� $i$ ����ĳ�ʼ״̬��
������ $E$ ��ÿ���������� $u,v$����ʾ����һ������ $u,v$ ������ߡ�

### �����ʽ

��һ��һ����������ʾ���� `T` ţ�� `ATTACK` ����������
�����������У�ÿ���� `MOVE u v` �� `ATTACK u v` ����ʽ��������ʾ��Ĳ���������

### ˵��/��ʾ

���ڲ��Ե� $1\sim5$��$1\leq V\leq 30,1\leq E\leq 50$��
���ڲ��Ե� $6\sim 10$��$1\leq V\leq 500,1\leq E\leq 2\times 10^3$��
���ڲ��Ե� $11\sim 15$��$1\leq V\leq 10^3,1\leq E\leq 5\times 10^3$��
ע�⣺һ��������Ҫ�������ڵ�λ�ã����磺�� $3$ �ϵ�ţ�� `MOVE` ���� $2$���� `ATTACK` �� $4$��Ӧ��дΪ��

\```
MOVE 3 2
ATTACK 2 4
\```


```input1
5 4 
TEJTJ 
1 2 
2 3 
3 4 
4 5 

```

```output1
2 
MOVE 3 2 
ATTACK 2 1 
ATTACK 5 4 

```

## ��ʾ
The other valid outputs are:

2
MOVE 3 2

ATTACK 5 4

ATTACK 2 1

and
2
ATTACK 5 4

MOVE 3 2

ATTACK 2 1

which are just reorderings of the output shown.  This might not be true on other testdata.


