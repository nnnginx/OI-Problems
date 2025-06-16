## ��Ŀ����
Mirko has bought an apartment and wants to invite to dinner as many people as possible to celebrate with him. For this he needs a large rectangular wooden table for which he will sit down with his guests. The number of people a table can accommodate is equal to its perimeter (the sum of the lengths of all four sides). Mirko wants to buy a table such that it fits in his apartment and that as many people as possible can sit down with him for dinner. The table must be placed so that its edges are parallel to the edges of the apartment.
Given the layout of the apartment, find the number of people Mirko can invite to dinner.

## �����ʽ
The first line contains two integers R and C (1 �� R, S �� 400), the dimensions of the apartment.
Each of the following R rows contains exactly S characters (without spaces), whether a square is free ('.') or blocked ('X').
Mirko can put his table only in free squares.

## �����ʽ
Output the number of guests Mirko can invite to dinner after he buys his table on a single line.

## ��Ŀ����
## ��Ŀ����
�׶�������һ�ױ���������Ҫ���뾡������˺���һ����ף������Ҫһ�Ŵ��ľ�ʾ������������������ļα����¡�ÿ�����ӿ����ɵ��������������ܳ����ı߳��ȵ��ܺͣ����׶�����Ҫ��һ�ż��������Ĺ�Ԣ����£�Ҳ�������¾�������˺���һ��������͵����ӡ����ӱ�����ó������߶��빫Ԣ��ǽƽ�е����ӡ���Ŀ������Ԣ�ڲ��Ĳ��֣������׶�����������������˳���͡�
## ���������ʽ
### �����ʽ��
��һ�а�����������R��S��1<=R,S<=400),����Ԣ�ĳߴ磨RΪ��SΪ���������µ�R����ÿһ�ж�������S��׼ȷ���ַ���û�пո񣩣��������������������û�ж�����('.') �������ж�����('X')���׶���ֻ�Ȱ����ӷ���û�ж����������������
### �����ʽ
����׶����ڷ����������Ӻ��ܹ�����������͵�����

��л@marcoolmap �ṩ�ķ���

```input1
2 2
..
..
```

```output1
7
```

```input2
4 4
X.XX
X..X
..X.
..XX
```

```output2
9
```

```input3
3 3
X.X
.X.
X.X
```

```output3
3
```

