## ��Ŀ����
You are trying to schedule a special event on one of five possible days.

Your job is to determine on which day you should schedule the event, so that the largest number of interested people are able to attend.

## �����ʽ
The first line of input will contain a positive integer $N$, representing the number of people interested in attending your event. The next $N$ lines will each contain one person's availability using one character for each of Day 1, Day 2, Day 3, Day 4, and Day 5(in that order).

The character `Y` means the person is able to attend and a period (`.`) means the person is
not able to attend.

The following table shows how the available 15 marks are distributed:
| Marks | Description |
| :----------: | :----------: |
| 6 | There will be exactly one day on which every person will be able to attend. |
| 6 | There will be exactly one day on which the largest number of people will be able to attend. |
| 3 | There might be more than one day on which the largest number of people will be able to attend. |


## �����ʽ
The output will consist of one line listing the day number(s) on which the largest number of
interested people are able to attend.

If there is more than one day on which the largest number of people are able to attend,output all of these day numbers in increasing order and separated by commas (without spaces).

## ��Ŀ����
��Ĺ�˾��Ҫ��һ�����飬һ���� $5$ ����Կ��ᡣ�����˾�� $N$ λԱ����ÿ��Ա�����ճ̰��Ŷ���ͬ������Ϊһ����˾�Ķ��³�����Ҫ��ȡ����Ա�������������Ҫ֪���ļ������������Ա����࣬��׼�����⼸����ѡһ�쿪�ᡣ

����Ҫʵ��һ�����򣬵�һ������һ�� $N$��$1\leq N \leq 20$������ʾ�� $N$ ��Ա����Ȼ�� $N$ �У�ÿ�� $5$ ���ַ���`Y` ��ʾ��Ա������������`.` ��ʾ���ܣ�������������ļ������������Ա����࣬����ж��죬����һ�� `,` �����

```input1
3
YY.Y.
...Y.
.YYY.
```

```output1
4
```

```input2
5
YY..Y
.YY.Y
.Y.Y.
.YY.Y
Y...Y
```

```output2
2,5
```

## ��ʾ
**��������������**��

- Subtask $1$��$6$ points��������ֻ��һ��ȫ���˶����Կ��ᡣ
- Subtask $2$��$6$ points��������ֻ��һ�쿪��������ࡣ
- Subtask $3$��$3$ points�����п����ж�������������


