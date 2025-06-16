## ��Ŀ����
Farmer John always wants his cows to have enough water and thus has made a map of the N (1 <= N <= 700) water pipes on the farm that connect the well to the barn. He was surprised to find a wild mess of different size pipes connected in an apparently haphazard way. He wants to calculate the flow through the pipes.

Two pipes connected in a row allow water flow that is the minimum of the values of the two pipe's flow values. The example of a pipe with flow capacity 5 connecting to a pipe of flow capacity 3 can be reduced logically to a single pipe of flow capacity 3:

```plain
+---5---+---3---+    ->    +---3---+
```

Similarly, pipes in parallel let through water that is the sum of their flow capacities:

```plain
   +---5---+
---+       +---    ->    +---8---+
   +---3---+
```

Finally, a pipe that connects to nothing else can be removed; it contributes no flow to the final overall capacity:

```plain
   +---5---+
---+               ->    +---3---+
   +---3---+--
```

All the pipes in the many mazes of plumbing can be reduced using these ideas into a single total flow capacity.

Given a map of the pipes, determine the flow capacity between the well (A) and the barn (Z).

Consider this example where node names are labeled with letters:

```plain
         +-----------6-----------+
A+---3---+B                      +Z
         +---3---+---5---+---4---+
                 C       D
```

Pipe BC and CD can be combined:

```plain
         +-----------6-----------+
A+---3---+B                      +Z
         +-----3-----+-----4-----+
                     D
```

Then BD and DZ can be combined: 

```plain
         +-----------6-----------+
A+---3---+B                      +Z
         +-----------3-----------+
```

Then two legs of BZ can be combined: 

```plain
         B
A+---3---+---9---+Z
```

Then AB and BZ can be combined to yield a net capacity of 3:

```plain
A+---3---+Z
```

Write a program to read in a set of pipes described as two endpoints and then calculate the net flow capacity from 'A' to 'Z'. All

networks in the test data can be reduced using the rules here.

Pipe i connects two different nodes a\_i and b\_i (a\_i in range

'A-Za-z'; b\_i in range 'A-Za-z') and has flow F\_i (1 <= F\_i <= 1,000). Note that lower- and upper-case node names are intended to be treated as different.

The system will provide extra test case feedback for your first 50 submissions.


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N + 1: Line i+1 describes pipe i with two letters and an integer, all space-separated: a\_i, b\_i, and F\_i


## �����ʽ
\* Line 1: A single integer that the maximum flow from the well ('A') to the barn ('Z')


## ��Ŀ����
Լ����ϣ��������ţ���㹻��ˮ�ȣ������������ũ����ˮ�ܵ�ͼ��������ţ��õ���ˮ����������ũ����һ���� $N$ ��ˮ�ܡ�Լ������ˮ��������Ҳ���������ͼ������м򻯡����򻯵ķ�ʽ�������ģ�

- ����ˮ�ܴ�����������ý�С�������Ǹ�ˮ�ܴ�����������
- ����ˮ�ܲ����������������Ϊ����ˮ�������͵�һ��ˮ�ܴ������ǡ�

��Ȼ���������һ��ˮ��һ��ʲôҲû�����ӣ����Խ����Ƴ� ��

��д�����������ˮ�� $\verb!A!$ ��ţ�� $\verb!Z!$ �������������ݱ�֤���������ˮ�����綼���������������� ��

**ע��**������������ÿ�������ô�д��ĸ**����**Сд��ĸ��ʾ��Ҳ����˵����������ܳ�����Сд��ĸ�����Ľڵ㡣

```input1
5 
A B 3 
B C 3 
C D 5 
D Z 4 
B Z 6 

```

```output1
3 

```

