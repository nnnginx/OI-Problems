## ��Ŀ����
The president of the political party in power is holding a conference in the party headquarters.
Politicians, members of the party, live in a two-dimensional grid, one member in each cell (except in cells containing obstacles). The headquarters are located in cell (0, 0). This is also where the president of the party lives.

ִ����������������������þ��л��顣��Ա�Ƕ���һ����άƽ��������У�һ����Ա��һ�������У����˺����ϰ��ĸ��ӣ�������λ�ڣ�0,0����������ǵ�λ�á�

Politicians make steps in one of the four directions (up, down, left, right), moving to one of the four adjacent cells in one step. They can't enter cells with obstacles. The conference will be attended by all party members that can reach headquarters in S steps or less. Each member coming to the conference will take the shortest route to headquarters (or any such route, if there is more than one).

��Ա��ѡ���ϡ��¡������ĸ������е�һ�����ƶ������ڵĸ�����ȥ�����ǲ��ܽ������ϰ��ĸ��ӡ����齫����������$S$�����ڵ�����õĵ�Ա�μӡ�ÿ�������������·�����ܲ�������ж������·��������һ������

The president has observed that politicians change their party affiliation with each step they take,becoming a member of the other party (there are only two parties on the political scene).
Write a program that determines how many politicians come to the conference as members of the party in power, and how many come as members of the opposing party.

����Ƿ��֣�������ÿ��һ�����ͻ�ı����ǵĵ��ɹ�ϵ����Ϊ��һ�������ĳ�Ա������ʵ�������ƣ�����дһ�������������ж��ٴ�����ִ���������ٴ����Ƿ��Ե���


## �����ʽ
The first line contains two integers B and S (0 �� B �� 10 000, 1 �� S �� 10 000 000), the number of obstacles and the largest number of steps from the task description.

Each of the following B lines contains two integers, the coordinates of one obstacle. The absolute value of both coordinates will be less than 1000.

No two obstacles will be in the same cell and there will be no obstacle in cell (0, 0).

## �����ʽ
Output two integers on a single line separated by a space, the number of politicians that come to the conference as members of the party in power and the opposing party, respectively.

```input1
0 2
```

```output1
9 4
```

```input2
4 5
-1 1
0 -1
0 1
1 0
```

```output2
10 16
```

```input3
4 50000
1 1
-1 -1
1 -1
-1 1
```

```output3
2500099997 2500000000
```

## ��ʾ
Croatian Olympiad in Informatics 2007
Task 3

