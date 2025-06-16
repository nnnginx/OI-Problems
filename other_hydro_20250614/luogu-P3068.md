## ��Ŀ����
Farmer John is throwing a party and wants to invite some of his cows to show them how much he cares about his herd.  However, he also wants to invite the smallest possible number of cows, remembering all too well the disaster that resulted the last time he invited too many cows to a party.

Among FJ's cows, there are certain groups of friends that are hard to separate.  For any such group (say, of size k), if FJ invites at least k-1 of the cows in the group to the party, then he must invite the final cow as well, thereby including the entire group.  Groups can be of any size and may even overlap with each-other, although no two groups contain exactly the same set of members.  The sum of all group sizes is at most 250,000.

Given the groups among FJ's cows, please determine the minimum number of cows FJ can invite to his party, if he decides that he must definitely start by inviting cow #1 (his cows are conveniently numbered 1..N, with N at most 1,000,000).



## �����ʽ
\* Line 1: Two space-separated integers: N (the number of cows), and G (the number of groups).

\* Lines 2..1+G: Each line describes a group of cows.  It starts with an integer giving the size S of the group, followed by the S cows in the group (each an integer in the range 1..N).



## �����ʽ
\* Line 1: The minimum number of cows FJ can invite to his party.




## ��Ŀ����
ũ��Լ��Ҫ�ٰ�һ���ۻᣬ��Ҫ����һЩ��ţ���μӡ���Լ������ţ����Ȧ�У���һЩ��ţ�Ǻû��ѣ�����ÿһ����ţ����Ȧ��û��һ����ȫ��֮��ͬ�ģ����������ţ����Ȧ�� $k$ ͷ��ţ�����Լ���Ѿ������� $k-1$ ͷ����ôʣ�µ���ͷţҲ�����롣Լ�����������������������Ҫ�������ͷ��ţ�����Ǽ��� $1$ ����ţ�Ѿ��������ˡ�

**�������ʽ��**

��һ�� $N$ �� $G$ ��ʾ���� $N$ ͷ��ţ�� $G$ ������Ȧ��

������ $G$ �У�ÿ�п�ͷ����һ������ $k$����ʾ����Ȧ���� $k$ ͷţ���������� $k$ ����������ʾ����Ȧ���ţ��

**�������ʽ��**

һ�У�һ����������ʾԼ��������Ҫ�����ţ��ͷ����

**�����ݷ�Χ��**

$1 \leq  N\leq1000000$��

�����е���ţ����Ȧ�Ĵ�С֮��Ϊ $M$���� $1 \leq  M\leq250000$��

```input1
10 4 
2 1 3 
2 3 4 
6 1 2 3 4 6 7 
4 4 3 2 1 

```

```output1
4 

```

## ��ʾ
There are 10 cows and 4 groups.  The first group contains cows 1 and 3, and so on.


In addition to cow #1, FJ must invite cow #3 (due to the first group constraint), cow #4 (due to the second group constraint), and also cow #2 (due to the final group constraint).



