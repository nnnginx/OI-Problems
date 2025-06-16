## ��Ŀ����
The cows are so very silly about their dinner partners. They have organized themselves into three groups (conveniently numbered 1, 2, and 3) that insist upon dining together. The trouble starts when they line up at the barn to enter the feeding area.

Each cow i carries with her a small card upon which is engraved Di (1 �� Di �� 3) indicating her dining group membership. The entire set of N (1 �� N �� 30,000) cows has lined up for dinner but it's easy for anyone to see that they are not grouped by their dinner-partner cards.

FJ's job is not so difficult. He just walks down the line of cows changing their dinner partner assignment by marking out the old number and writing in a new one. By doing so, he creates groups of cows like 111222333 or 333222111 where the cows' dining groups are sorted in either ascending or descending order by their dinner cards.

FJ is just as lazy as the next fellow. He's curious: what is the absolute mminimum number of cards he must change to create a proper grouping of dining partners? He must only change card numbers and must not rearrange the cows standing in line.

FJ����ţ���ڳ���ʱ��ɵ�����ǰ��Լ���֯�����飨������Ϊ1, 2��3�������һ���ò͡��������ڹȲ��Ŷӽ���ιʳ��ʱ���鷳�Ϳ�ʼ�ˡ�


ÿͷ��ţ���������һ��С��Ƭ��С��Ƭ�Ͽ̵���Di��1��Di��3����ʾ��������һ�顣���е�N��1��N��30000��ͷ��ţ�ŶӳԷ��������ǲ����ܰ���Ƭ�ϵķ���վ�á�


FJ�Ĺ�����������ô�ѡ���ֻ������ţ��·������ȥ���Ѿɵĺ�������������һ���µġ�ͨ������������������һȺ��ţ������111222333��333222111����ţ�ľͲ��鰴���ǵ���Ϳ�Ƭ������������С�


FJ�����κ���һ�����衣���ܺ��棺���������ܽ����ʵ��ķ��飬ʹ����ֻҪ�޸����ٴ��������֣�������ţ���Ѿ��ܳ�ʱ��û�гԵ����ˣ����ԡ����衱�������������ǣ�FJֻ�ø������ţ����������������Ѿ��źöӵ���ţ��


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i describes the i-th cow's current dining group with a single integer: Di

- ��1�У�һ��������n

- ��2~n+1�У���i-1��������i����ţĿǰ���顣


## �����ʽ
\* Line 1: A single integer representing the minimum number of changes that must be made so that the final sequence of cows is sorted in either ascending or descending order

һ����������ʾ������������С�仯�����Ա���������������������С�


```input1
5
1
3
2
1
1

```

```output1
1

```

## ��ʾ
��л@һ˼ǧ�� �ṩ����


