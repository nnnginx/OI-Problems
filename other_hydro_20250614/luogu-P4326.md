## ��Ŀ����
The 19th century German mathematician Hermann Minkowski investigated a non-Euclidian geometry, called the taxicab geometry. In taxicab geometry the distance between two points T1(x1, y1) and T2(x2, y2) is defined as:
D(T1,T2) = |x1 - x2| + |y1 - y2|
All other definitions are the same as in Euclidian geometry, including that of a circle:
A circle is the set of all points in a plane at a fixed distance (the radius) from a fixed point (the centre of the circle).
We are interested in the difference of the areas of two circles with radius R, one of which is in normal (Euclidian) geometry, and the other in taxicab geometry. The burden of solving this difficult problem has fallen onto you.

## �����ʽ
The first and only line of input will contain the radius R, an integer smaller than or equal to 10000.

## �����ʽ
On the first line you should output the area of a circle with radius R in normal (Euclidian) geometry.
On the second line you should output the area of a circle with radius R in taxicab geometry.
Note: Outputs within ��0.0001 of the official solution will be accepted.

## ��Ŀ����
19���͵ĵ¹���ѧ�Һն������ɿɷ�˹��(Hermann Minkowski)�о���һ����Ϊ���⳵����ѧ�ķ�ŷ���Ρ�
�ڳ��⳵������$T_1(x_1,y_1)$ $T_2(x_2,y_2)$����֮��ľ��뱻����Ϊ$dis(T_1,T_2)=|x_1-x_2|+|y_1-y_2|$(�����پ���)��
�����������ŷ����ü�����ͬ��  
����Բ�Ķ��壺��ͬһƽ���ڣ�������(Բ��)�ľ�����ڶ���(�뾶)�ĵ�ļ��ϡ�

���Ƕ�ŷ����ü�������⳵�������ֶ����°뾶Ϊ$R$��Բ������ܸ���Ȥ��������������ص��������������ˡ�


## ���������ʽ

### �����ʽ

����һ��ΪԲ�İ뾶$R$�� $(R \leq 10000)$

### �����ʽ

��һ�����ŷ����ü����°뾶Ϊ$R$��Բ��������ڶ���������⳵�����°뾶Ϊ$R$��Բ�������

ע�⣺���������׼�𰸾���������$0.0001$���ᱻ��Ϊ��ȷ

```input1
1
```

```output1
3.141593
2.000000
```

```input2
21
```

```output2
1385.442360
882.000000
```

```input3
42
```

```output3
5541.769441
3528.000000
```

