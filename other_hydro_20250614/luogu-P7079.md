## ��Ŀ����


Little Dmitry and little Petr want to arrange a contest. Their little friends submitted several task proposals and now Dmitry and Petr want to select some of them for the contest. As they are just little boys, they cannot estimate quality of tasks, but they know for sure that in good contest title of the first problem starts with A , the title of the second one -- with $B$ , and so on.

Given titles of the proposed tasks, help little brothers to determine the maximal number of problems in a good contest they can arrange.



## �����ʽ


The first line contains single integer $n$ -- the number of problem proposals received by the little brothers $(1 \le n \le 100)$ .

Next $n$ lines contain titles of proposed problems, one per line. The length of each title does not exceed $30$ characters. Each title starts with an uppercase letter and contains only English letters, digits and underscores.



## �����ʽ


Output a single number -- the maximal number of problems in a good contest. In case there is no good contest that may be arranged, output $0$ .



## ��Ŀ����
**��Ŀ����**

СD��СP��Ҫ���б�����

�����յ�����ཨ���飬����������Ҫ����Щ����������ѡһЩ�õĽ��顣

���ǲ��ɵĽ���������±�׼����һ������Ŀ�ͷΪA���ڶ�������Ŀ�ͷΪB���Դ����ơ�

����������ǣ�ȷ���������ܲ��ɵĽ�������������

**�����ʽ**

��һ�У�һ�������� $n$����ʾ��������

�� $2$ �� $n+1$ �У�һ��һ���ַ�������ʾ�������ơ�

**�����ʽ**

һ����������ʾ�������ܲ��ɵĽ�������������

**˵��/��ʾ**

���� $100\%$ �����ݣ�$1\leq n \leq 100$

```input1
12
Arrangement_of_Contest
Ballot_Analyzing_Device
Correcting_Curiosity
Dwarf_Tower
Energy_Tycoon
Flight_Boarding_Optimization
Garage
Heavy_Chain_Clusterization
Intellectual_Property
J
Kids_in_a_Friendly_Class
Lonely_Mountain

```

```output1
12

```

```input2
3
Snow_White_and_the_7_Dwarfs
A_Problem
Another_Problem

```

```output2
1

```

```input3
2
Good_Problem
Better_Problem

```

```output3
0

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



