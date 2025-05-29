## ��Ŀ����
Farmer John's cows have taken an interest in exploring the territory around the farm. Initially, all N (1 <= N <= 1,000,000,000) cows commence traveling down a road in one big group. Upon encountering a fork in the road, the group sometimes chooses to break into two smaller (nonempty) groups with each group continuing down one of the roads.  When one of those groups arrives at another fork, it might split again, and so on.

The cows have crafted a peculiar way of splitting: if they can split into two groups such that the sizes of the groups differ by exactly K (1 <= K <= 1000), then they will split in that way; otherwise, they stop exploring and just start grazing peacefully.

Assuming that there will always be new forks in the road, compute the final number of groups of peacefully grazing cows.

## �����ʽ
\* Line 1: Two space-separated integers: N and K


## �����ʽ
\* Line 1: A single integer representing the number of groups of grazing cows


## ��Ŀ����
Լ���� $ N $ ֻ��ţҪ����ȥ̽���������ܵ����ء����ǽ�����һ��·�ߣ�һֱ�ߵ�����·�ڣ�������Ϊ���е�·�ڶ��������ģ�����ʱ����һȺ��ţ���ܻ�ֳ���Ⱥ���ֱ����Ž�����������·�����ߡ���������ٴ��ߵ�����·�ڣ���ô���п��ܼ������ѳ���Ⱥ�����ߡ� 

��ţ�ķ��ѷ�ʽʮ�ֹŹ֣�  

�����һȺ��ţ���Ծ�ȷ�طֳ������֣��������ֵ�ţ��ǡ����� $ K $ ͷ����ô������·��ţȺ�ͻ���ѡ�

����ţȺ������ѣ����Ƕ������������ȥ��ƽ���سԲݡ� ����㣬���ս����ж���Ⱥ��ţ��ƽ���سԲݡ�

���ݷ�Χ��

$ 1 \le N \le 10^{9}$ 

$ 1 \le K \le 10^{3}$

```input1
6 2 

```

```output1
3 

```

## ��ʾ
There are 6 cows and the difference in group sizes is 2.


There are 3 final groups (with 2, 1, and 3 cows in them). 

6
/ \
2   4
/ \
1   3

