## ��Ŀ����
Bessie and Bonnie have found a treasure chest full of marvelous gold coins! Being cows, though, they can't just walk into a store and buy stuff, so instead they decide to have some fun with the coins.

The N (1 <= N <= 5,000) coins, each with some value C\_i (1 <= C\_i <= 5,000) are placed in a straight line. Bessie and Bonnie take turns, and for each cow's turn, she takes exactly one coin off of either the left end or the right end of the line. The game ends when there are no coins left.

Bessie and Bonnie are each trying to get as much wealth as possible for themselves. Bessie goes first. Help her figure out the maximum value she can win, assuming that both cows play optimally.

Consider a game in which four coins are lined up with these values:

30  25  10  35

Consider this game sequence:

Bessie    Bonnie       New Coin

Player   Side   CoinValue   Total     Total         Line

Bessie   Right     35        35         0       30  25  10

Bonnie   Left      30        35        30         25  10

Bessie   Left      25        60        30           10

Bonnie   Right     10        60        40           --

This is the best game Bessie can play.

С A ��С B ������Ϸ��

��ʼʱ���� $n$ ��Ӳ�ұ��ڳ���һ�У������������� $i$ ��Ӳ�ҵļ�ֵΪ $c_i$��

С A ��С B ÿ��һ�غϣ���һ���˵Ļغ��У�������ѡ��**��ǰ**Ӳ�����������������Ҳ��Ӳ�ң���������������ȡ���������ֵ�ۼӵ��Լ���õ��ۼƼ�ֵ�У�Ȼ�������һ���˵Ļغϡ���Ӳ��ȫ����ȡ��ʱ����Ϸ������

�������˫���������ܵ�ʹ�Լ��ۼƼ�ֵ��������£�����С A ���е�һ�غϣ���ô���ܻ�õ��ۼƼ�ֵ����Ƕ��١�

## �����ʽ
����ĵ�һ����һ������ $n$������Ӳ�ҵĸ�����

�� $2$ ���� $(n + 1)$ �У�ÿ��һ���������� $(i + 1)$ �е���������� $i$ ��Ӳ�ҵļ�ֵ $c_i$��

## �����ʽ
���һ��һ������������С A �ܻ�õ�����ۼƼ�ֵ��

```input1
4 
30 
25 
10 
35 

```

```output1
60 

```

## ��ʾ
#### ����������� $1$ ����

��ʼʱ��Ӳ������Ϊ $\{30,~25,~10,~35\}$��

��һ�غϣ�С A ȡ�����Ҳ��Ӳ�ң����б�Ϊ $\{30,~25,~10\}$��С A ���ۼӼ�ֵΪ $35$��

�ڶ��غϣ�С B ȡ��������Ӳ�ң����б�Ϊ $\{25,~10\}$��С B ���ۼӼ�ֵΪ $30$��

�����غϣ�С A ȡ��������Ӳ�ң����б�Ϊ $\{10\}$��С A ���ۼӼ�ֵΪ $35 + 25 = 60$��

���Ļغϣ�С B ȡ��������Ӳ�ң����б�Ϊ�գ�С B ���ۼӼ�ֵΪ $30 + 10 = 40$����Ϸ������

С A ��õ�����ۼƼ�ֵΪ $60$��

#### ���ݷ�Χ��Լ��

����ȫ���Ĳ��Ե㣬$1 \leq n \leq 5 \times 10^3$��$1 \leq c_i \leq 5 \times 10^3$��

**��ʾ����ע�⣬����Ŀռ�����Ϊ $64$ Mib��**

