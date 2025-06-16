## ��Ŀ����
Farmer John's milk production and shipping system is an intricate one! He uses milking machines for his many cows to harvest the milk that then flows into pipes.

Each of these pipes connects a milking machine to a joint, where it might be joined by exactly one more pipe (the milk flowing through both pipes merges). The milk then flows through additional pipes (which all start and end at joints) until it reaches the long central pipe connecting to the distribution room.

The milk then goes through a reverse process of splitting at various joints until it is flows into milk tanks that are picked up and taken to market.

Farmer John notices that there is at most one way for milk to travel from one joint to any other joint. Furthermore, since Farmer John is an efficient man by nature, he has made sure that milk will flow through each and every pipe; in other words, no pipe is unneeded.

If we think of a milking machine, joint, or milk tank as a node, there are N (2 <= N <= 100,000) nodes in total (and N-1 pipes

connecting them). The input describes each pipe as an ordered pair of nodes, A\_i (1 <= A\_i <= N) and B\_i (1 <= B\_i <= N; A\_i < B\_i) indicating milk flows from node A\_i to node B\_i. If there is no pipe coming in to A\_i, it is a milking machine. Likewise, if no pipe goes out from B\_i, it is a tank.

The demand of chocolate milk has skyrocketed in recent months, and Farmer John wants to install a chocolate inserter at one of the joints so he can create delicious chocolate milk for customers.

Being thrifty, Farmer John has only bought one chocolate inserter, so he wants to place it at a joint through which all the milk passes. He knows that such a joint exists.

Help Farmer John find all the possible places he can install the chocolate inserter.  (Note that Farmer John cannot install the chocolate inserter at the same location as a milking machine.)

As an example, consider a milking setup like this one:

```cpp

           1 ----+
                 |
                 v
           2 --> 4 --> 6 ------------------> 7 --> 8
                       ^                     |
                       |                     |
           3 --> 5 ----+                     + --> 9

```
Visual inspection shows that the chocolate inserter can be installed at either joint 6 or 7, as all milk flows through those joints.


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N: Line i+1 contains two space-separated integers that describe a pipe's connectivity: A\_i and B\_i


## �����ʽ
\* Lines 1..??: Integers, one per line and in ascending order, each denoting a possible joint at which to install the chocolate inserter.

## ��Ŀ����
### ��Ŀ����
ũ��Լ����ţ��������������һ�����ӵĹ��̣����ü�������������ô��ͷ��ţ���̣�Ȼ������ܵ���

ÿһ���ܵ���һ̨��������һ����������һ̨���̨�������Ľӿ��������������������ܵ����ţ�̾ͻ���ˣ���Ȼ��ţ�����븽�ӹܵ������ڸ����ӿ�֮��Ĺܵ���ֱ����������ܵ���ͨ�򴢴��ҡ� Ȼ����Щţ���־���һ������Ĺ���ͨ���ܵ�����������ţ��Ͱ����������г���

Լ�����ֶ���ţ����˵�����ֻ��һ�ַ�ʽ��һ���ӿ�������һ���ӿڡ���������Լ����һ����Ч�ʵ��ˣ�����Ҫȷ��ÿһ���ܵ�����ţ�̾�����Ҳ����˵��û�ж���Ĺܵ���

������ǰ�ÿ�����̻����ӿں��̹޶�����һ���ڵ㣬�͹��� $N$ ���ڵ㣬��������Ľڵ�� $A_{i}$ �� $B_{i}$ ������ţ�̴� $A_{i}$ �ڵ����� $B_{i}$ �ڵ㣬���û�����Ӧ�ĸ��ڵ㣬�Ǿ�˵������һ����������ͬ�������û�ж�Ӧ��β�ڵ㣬������һ���̹ޡ�

�⼸�����ɿ���ţ�̵�����������������Լ����Ҫ��ĳһ���ӿڴ���װһ���ɿ���������Եõ��ɿ���ţ�̣�Ϊ�˽�Լ��Լ��ֻ����һ���ɿ���������������������������ŵ�һ������ţ�̶��ܾ����Ľӿڣ���ʵ�ϣ������ֽӿڴ��ڡ�

����Լ���ҵ������Ľڵ㣨ע�⣺���ܰ��ɿ�����������ڼ��̻����
```

           1 ----+
                 |
                 v
           2 --> 4 --> 6 ------------------> 7 --> 8
                       ^                     |
                       |                     |
           3 --> 5 ----+                     + --> 9

```
���е�ţ�̶�������6�Ż�7�Žڵ㣬�����ɿ�����������Է����������ڵ��ϡ�

### �����ʽ
�� $1$ ��һ������ $N$��

�� $2$ ���� $N$ �У������ո�ָ������������������� $i$ ���ܵ����ӵ������ڵ㣺$A_{i}$ �� $B_{i}$��

### �����ʽ
�� $1$ �е� �����У�ÿ��һ���������������ÿ�����԰�װ�ɿ���������Ľڵ㡣

```input1
9 
1 4 
3 5 
2 4 
5 6 
6 7 
7 8 
4 6 
7 9 

```

```output1
6 
7 

```

