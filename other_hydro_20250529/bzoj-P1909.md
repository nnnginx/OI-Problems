


## ��Ŀ����
һ���ۿڱ��ֳ��� M������(1<=M<=10)��ÿ�������������ͬʱͣ��10000 �Ҵ���ֻҪ��Щ����ȥ��ʱ�䲻�����ͻ.ÿ�Ҵ���ֻ��ͣ�����ض���һ��������n �Ҵ�(1<=N<=100000)����֪ÿ�����ĵ���ʱ�̡��뿪ʱ�̺���Ӧ�ý����������һ�����ȷ���ʹ���������Ĵ�����ͣ����
## �����ʽ
Input contains many test sets. A test data set is defined as follow:
The first line of test data set is two integers: m and n, separated by one or more spaces(1��m��10, 1��n��100000). m is the number of sections in the port, and n is the number of ships.
The next m lines, one positive integer r (that means the length of the section is r hundred meters long) per line. The length of each section does not exceed 10000 hundred meters.
The next n lines gives one ship information on each line, with three non-negative integers s, e, sec (0��s��e,1��sec��m) per line, s is the arrival time of the ship, e is the departure time of the ship, and sec is the section which the ship should be berthed in.
Input is ended by EOF. You can assume that all the input data are legal.
## �����ʽ
For each test data set you should output one integer, the maximal number of the berthed ships, per line.

```input1
2 6  //��������,��ֻ��
3   //����Ĵ�С
3  //����Ĵ�С
1 2 1  //ÿֻ����ȥ��ʱ�估��Ӧ��Ҫͣ���������
1 2 1
1 2 1
1 2 1
1 2 2
1 2 2
1 3
2
1 3 1
2 6 1
2 8 1
1 4
2
1 3 1
5 6 1
2 8 1
4 10 1

```

```output1
5
2
3
```

## ��ʾ
2004��㶫ʡ��ѧ������������ Problem B
## ��Ŀ��Դ
û��д����Դ


