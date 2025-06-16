## ��Ŀ����
Hostile Bitotia launched a sneak attack on Byteotia and occupied a significant part of its territory.

The King of Byteotia, Byteasar, intends to organise resistance movement in the occupied area.

Byteasar naturally started with selecting the people who will form the skeleton of the movement.

They are to be partitioned into two groups:

the conspirators who will operate directly in the occupied territory, and    the support group that will operate inside free Byteotia.

There is however one issue - the partition has to satisfy the following conditions:

Every pair of people from the support group have to know each other - this        will make the whole group cooperative and efficient.

The conspirators must not know each other.

None of the groups may be empty, i.e., there has to be at least one conspirator        and at least one person in the support group.

Byteasar wonders how many ways there are of partitioning selected people into    the two groups.

And most of all, whether such partition is possible at all.

As he has absolutely no idea how to approach this problem, he asks you for help.




## �����ʽ
The first line of the standard input holds one integer $n$ ($2\le n\le 5000$),      denoting the number of people engaged in forming the resistance movement.

These people are numbered from 1 to $n$ (for the sake of conspiracy!).

The $n$ lines that follow describe who knows who in the group.

The $i$-th of these lines describes the acquaintances of the person $i$ with a sequence of integers separated by single spaces.

The first of those numbers, $k_i$ ($0\le k_i\le n-1$), denotes the number of acquaintances of the person $i$.

Next in the line there are $k_i$ integers $a_{i,1},a_{i,2},\cdots,a_{i,k_i}$ - the numbers of $i$'s acquaintances.The numbers $a_{i,j}$ are given in increasing order and satisfy $1\le a_{i,j}\le n$,$a_{i,j}\ne i$. You may assume that if $x$ occurs in the sequence $a_i$ (i.e., among $i$'s acquaintances), then also $i$ occurs in the sequence $a_x$(i.e., among $x$'s acquaintances).


## �����ʽ
In the first and only line of the standard output your program should print out one integer:

the number of ways to partition selected people into the conspirators and the support group.

If there is no partition satisfying aforementioned conditions, then 0 is obviously the right answer.


## ��Ŀ����
## ����

Byteotia��������ռ���ˣ�����Byteasar���ڴ�����֯���ֿܵ��˶���������ҪѡһЩ���������ⳡ�˶�������Щ�˱���Ϊ�����֣�һ���ֳ�Ϊͬı�߻�ڱ�ռ��������һ�����Ǻ�����֯��δ��ռ�����������ת���������������һ�����⣺ 

1. ������֯����������˶����������ˣ��Դٽ���������߹���Ч�ʡ� 
2. ͬı�ߵ��������������˶����������ˡ� 
3. ÿһ���ֶ�����Ҫ��һ���ˡ�������֪���ж����ַ��䷽������������������ȻҲ�п��ܲ����ں�������

���ڹ�����������⽻�����������

## ����

��һ��һ������n��2<=n<=5000����ʾ��n���˲���õֿ��˶������Ϊ1..n��

 ֮����n�У���i�еĵ�һ����ki��0<=ki<=n-1����ʾi��ʶki����,����ki������ʾi�����ˡ�

�����������i��x�����ˣ�x����i�������г���ͬʱiҲ�������x�����������С�

## ���

���������ķ���������

```input1
4
2 2 3
2 1 3
3 1 2 4
1 3
```

```output1
3
```

