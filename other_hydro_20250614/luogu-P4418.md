## ��Ŀ����
Near a military base there is a system of trenches, modeled as line segments on a plane. During nighttime, when most soldiers are fast asleep, three guards stand watch of the trenches. Two guards can see each other if there is a trench (or a row of trenches) along the entire straight line segment between them and there is no third guard on that line segment.
For security reasons, the guards must be placed so that each guard sees the other two. How many ways can they be placed?

## �����ʽ
The first line contains the integer N (1 �� N �� 20), the number of trenches. Each of the next N lines contains the description of one trench: four positive integers X1, Y1, X2, Y2 (all less than or equal to 1000), where X1 and Y1 are coordinates of one end, while X2 and Y2 are coordinates of the other end of the trench.
Trenches in the input may overlap and share endpoints.

## �����ʽ
Output the number of ways the guards can be placed on a single line.

## ��Ŀ����
��Ŀ������

�ھ��»��ظ�����һ��ս���������е�ս����ƽ���ϵ��߶�Ϊģ�͡���ҹ�䣬�������ʿ����˯��ʱ����������վ��ս���Աߡ����������֮�������ֱ�߶�����һ��ս������һ��ս�������Ҹ�ֱ�߶���û�е�����������ô�����������Կ����˴ˡ����ڰ�ȫԭ�򣬱��밲�ž������Ա�ÿ�����������������������������ж����ֱ����ŵķ�ʽ��

�����ʽ��

��һ�а�������n��1��n��20����ս������Ŀ����������n���е�ÿһ�ж�����һ��ս�����������ĸ�������X1,Y1,X2,Y2����С�ڻ����1000��������X1��Y1��һ�˵����꣬��X2��Y2��ս����һ�˵����ꡣ�����е�ս�������ص�������˵㡣

�����ʽ��

����һ���У��ж����ְ��ž����ķ�ʽ��

```input1
6
0 0 1 0
0 0 0 1
1 0 1 1
0 1 1 1
0 0 1 1
1 0 0 1
```

```output1
8
```

```input2
4
5 1 7 1
1 1 5 1
4 0 4 4
7 0 3 4
```

```output2
1
```

```input3
3
2 2 3 2
3 2 3 3
3 3 2 3
```

```output3
0
```

