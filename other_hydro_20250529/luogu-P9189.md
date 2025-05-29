## ��Ŀ����
Due to the disorganized structure of his mootels (much like motels but with
bovine rather than human guests), Farmer John has decided to take up the role of
the mootel custodian to restore order to the stalls.

Each mootel has $N$ stalls labeled $1$ through $N$ and $M$ corridors that connect pairs of stalls to each other
bidirectionally. The $i$ th stall is painted with color $C_i$ and initially has a
single key of color $S_i$ in it. FJ will have to rearrange the keys to appease
the cows and restore order to the stalls.

FJ starts out in stall $1$ without holding any keys and is allowed to repeatedly
do one of the following moves:
- Pick up a key in the stall he is currently in. FJ can hold multiple keys at
a time.
- Place down a key he is holding into the stall he is currently
in. A stall may hold multiple keys at a time.
- Enter stall $1$ by
moving through a corridor.
- Enter a stall other than stall $1$ by
moving through a corridor. He can only do this if he currently holds a key that
is the same color as the stall he is entering.

Unfortunately, it seems that the keys are not in their intended locations. To
restore order to FJ's mootel, the $i$th stall requires that a single key of
color $F_i$ is in it. It is guaranteed that $S$ is a permutation of $F$.

For $T$ different mootels, FJ starts in stall $1$ and needs
to place every key in its appropriate location, ending back in stall $1$. For
each of the $T$ mootels, please answer if it is possible to do this.

## �����ʽ
The first line contains $T$, the number of mootels (test cases).

Each test case will be preceded by a blank line. Then, the first line 
of each test case contains two integers $N$ and $M$.

The second line of each test case contains $N$ integers. The $i$-th integer on
this line $C_i$ means that stall $i$ has color $C_i$.

The third line of each test case contains $N$ integers. The $i$-th integer on
this line $S_i$ means that stall $i$ initially holds a key of color $S_i$.

The fourth line of each test case contains $N$ integers. The $i$-th integer on
this line $F_i$ means that stall $i$ needs to have a key of color $F_i$ in it.

The next $M$ lines of each test case follow. The $i$-th of these lines contains
two distinct integers $u_i$ and $v_i$. This represents
that a corridor exists between stalls $u_i$ and $v_i$. No corridors are
repeated.


## �����ʽ
For each mootel, output `YES` on a new line if there exists a way for FJ to return
a key of color $F_i$ to each stall $i$ and end back in stall $1$. Otherwise,
output `NO` on a new line.

## ��Ŀ����
### ��Ŀ����

�������� mootels�������������ùݣ���ס����ţ�������ˣ��ṹ���ң�ũ�� John �������� mootel �Ĺ���Ա���Իָ�ţ��������

ÿ�� mootel �� $N$ ��ţ�������Ϊ $1$ �� $N$���Լ� $M$ ��˫�����ӵ����ȡ��� $i$ ��ţ����Ϳ����ɫ $C_i$���������������һ����ɫΪ $S_i$ ��Կ�ס�FJ ��Ҫ���°���Կ�׵�λ�ã��԰�����ţ���ָ�ţ��������

FJ ��ţ�� $1$ ��ʼ������û���κ�Կ�ף����ҿ����ظ�ִ�����²���֮һ��
- ʰȡ��ǰ����ţ���е�һ��Կ�ס�FJ ����ͬʱ���ж��Կ�ס�
- �����г��е�һ��Կ�׷��뵱ǰ���ڵ�ţ����һ��ţ������ͬʱ��Ŷ��Կ�ס�
- ͨ�����Ƚ���ţ�� $1$��
- ͨ�����Ƚ���ţ�� $1$ ���������ţ����ֻ�е� FJ ��ǰ���е�Կ����ɫ��Ŀ��ţ������ɫ��ͬʱ������ִ�д˲�����

���ҵ��ǣ�Կ���ƺ���δ��������Ӧ�е�λ�á�Ϊ�˻ָ� FJ �� mootel �����򣬵� $i$ ��ţ����Ҫ��һ����ɫΪ $F_i$ ��Կ�ס���֤ $S$ �� $F$ ��һ�����С�

���� $T$ ����ͬ�� mootel��FJ ��ţ�� $1$ ��ʼ����Ҫ��ÿ��Կ�׷ŵ���Ӧ�е�λ�ã������ջص�ţ�� $1$������ÿ�� mootel����ش��Ƿ���������һ����

### �����ʽ

��һ�а��� $T$����ʾ mootel ��������������������������

ÿ����������ǰ��һ�����С�Ȼ��ÿ�����������ĵ�һ�а����������� $N$ �� $M$��

ÿ�����������ĵڶ��а��� $N$ ���������� $i$ ������ $C_i$ ��ʾţ�� $i$ ����ɫΪ $C_i$��

ÿ�����������ĵ����а��� $N$ ���������� $i$ ������ $S_i$ ��ʾţ�� $i$ �����һ����ɫΪ $S_i$ ��Կ�ס�

ÿ�����������ĵ����а��� $N$ ���������� $i$ ������ $F_i$ ��ʾţ�� $i$ ��Ҫ��һ����ɫΪ $F_i$ ��Կ�ס�

ÿ������������������ $M$ �У�ÿ�а���������ͬ������ $u_i$ �� $v_i$�����ʾţ�� $u_i$ �� $v_i$ ֮����һ�����ȡ�û���ظ������ȡ�

### ��ʾ

���ڵ�һ�������ĵ�һ������������������һ�ֿ��ܵĲ������С�

```
��ǰţ����1�����е�Կ�ף�[]��ţ���е�Կ�ף�[3, 4, 3, 4, 2] ��ʰȡ��ɫΪ 3 ��Կ�ף�
��ǰţ����1�����е�Կ�ף�[3]��ţ���е�Կ�ף�[x, 4, 3, 4, 2] ����ţ�� 1 �ƶ���ţ�� 2��������Ϊ������ɫΪ C_2=3 ��Կ�ף�
��ǰţ����2�����е�Կ�ף�[3]��ţ���е�Կ�ף�[x, 4, 3, 4, 2] ��ʰȡ��ɫΪ 4 ��Կ�ף�
��ǰţ����2�����е�Կ�ף�[3, 4]��ţ���е�Կ�ף�[x, x, 3, 4, 2] ����ţ�� 2 �ƶ���ţ�� 1 ��ţ�� 4 ��ţ�� 5��������Ϊ������ɫΪ C_4=4 �� C_5=3 ��Կ�ף�
��ǰţ����5�����е�Կ�ף�[3, 4]��ţ���е�Կ�ף�[x, x, 3, 4, 2] ��ʰȡ��ɫΪ 2 ��Կ�ײ�������ɫΪ 3 ��Կ�ף�
��ǰţ����5�����е�Կ�ף�[2, 4]��ţ���е�Կ�ף�[x, x, 3, 4, 3] ����ţ�� 5 �ƶ���ţ�� 4 ��ţ�� 1 ��ţ�� 3��������Ϊ������ɫΪ C_4=4 �� C_3=2 ��Կ�ף�
��ǰţ����3�����е�Կ�ף�[2, 4]��ţ���е�Կ�ף�[x, x, 3, 4, 3] ��ʰȡ��ɫΪ 3 ��Կ�ײ�������ɫΪ 4 ��Կ�ף�
��ǰţ����3�����е�Կ�ף�[2, 3]��ţ���е�Կ�ף�[x, x, 4, 4, 3] ����ţ�� 3 �ƶ���ţ�� 2 ��������ɫΪ 3 ��Կ�ף�
��ǰţ����2�����е�Կ�ף�[2]��ţ���е�Կ�ף�[x, 3, 4, 4, 3] ����ţ�� 2 �ƶ���ţ�� 1 ��������ɫΪ 2 ��Կ�ף�
��ǰţ����1�����е�Կ�ף�[]��ţ���е�Կ�ף�[2, 3, 4, 4, 3]
```

���ڵ�һ�������ĵڶ�������������������һ�ַ�ʽ�� FJ ����ɫΪ $F_i$ ��Կ�׷Ż�ÿ��ţ�� $i$ �����ջص�ţ�� $1$��

$0 \le M \le 10^5$��$1 \le C_i, S_i, F_i, u_i, v_i \le N \le 10^5$��  
$1 \le T \le 100$��$1 \le \sum N \le 10^5$��$1 \le \sum M \le 2 \cdot 10^5$��

- �������� 3-6 ���� $N, M \le 8$��
- �������� 7-10 ���� $C_i = F_i$��
- �������� 11-18 û�ж������ơ�

```input1
2

5 5
4 3 2 4 3
3 4 3 4 2
2 3 4 4 3
1 2
2 3
3 1
4 1
4 5

4 3
3 2 4 1
2 3 4 4
4 2 3 4
4 2
4 1
4 3

```

```output1
YES
NO

```

```input2
5

2 0
1 2
2 2
2 2

2 1
1 1
2 1
2 1
1 2

2 1
1 1
2 1
1 2
1 2

2 1
1 1
1 2
2 1
1 2

5 4
1 2 3 4 4
2 3 5 4 2
5 3 2 4 2
1 2
1 3
1 4
4 5

```

```output2
YES
YES
NO
YES
NO

```

## ��ʾ
For the first test case of the first sample, here is a possible sequence of moves:

```
Current stall: 1. Keys held: []. Keys in stalls: [3, 4, 3, 4, 2]
(pick up key of color 3)
Current stall: 1. Keys held: [3]. Keys in stalls: [x, 4, 3, 4, 2]
(move from stall 1 to 2, allowed since we have a key of color C_2=3)
Current stall: 2. Keys held: [3]. Keys in stalls: [x, 4, 3, 4, 2]
(pick up key of color 4)
Current stall: 2. Keys held: [3, 4]. Keys in stalls: [x, x, 3, 4, 2]
(move from stall 2 to 1 to 4 to 5, allowed since we have keys of colors C_4=4 and C_5=3)
Current stall: 5. Keys held: [3, 4]. Keys in stalls: [x, x, 3, 4, 2]
(pick up key of color 2 and place key of color 3)
Current stall: 5. Keys held: [2, 4]. Keys in stalls: [x, x, 3, 4, 3]
(move from stall 5 to 4 to 1 to 3, allowed since we have keys of colors C_4=4 and C_3=2)
Current stall: 3. Keys held: [2, 4]. Keys in stalls: [x, x, 3, 4, 3]
(pick up key of color 3 and place key of color 4)
Current stall: 3. Keys held: [2, 3]. Keys in stalls: [x, x, 4, 4, 3]
(move from stall 3 to stall 2 and place key of color 3)
Current stall: 2. Keys held: [2]. Keys in stalls: [x, 3, 4, 4, 3]
(move from stall 2 to stall 1 and place key of color 2)
Current stall: 1. Keys held: []. Keys in stalls: [2, 3, 4, 4, 3]
```

For the second test case of the first sample, there exists no way for FJ to return a key of color
$F_i$ to each stall $i$ and end back at stall $1$.

$0 \le M \le 10^5$, $1 \le C_i, S_i, F_i, u_i, v_i \le N \le 10^5$.   
$1 \le T \le 100$, $1 \le \sum N \le 10^5$, $1 \le \sum M \le 2\cdot 10^5$.

- Test cases 3-6 satisfy $N,M\le 8$.
- Test cases 7-10 satisfy $C_i=F_i$.
- Test cases 11-18 satisfy no additional constraints.


