## ��Ŀ����
You are cooking on a gigantic stove at a large fast-food restaurant. The stove contains $n$ heating elements arranged in a line and numbered with integers $1$ through $n$ left to right. Each element is operated by its control knob. The knobs are a bit unusual: each knob is marked with seven non-zero digits evenly distributed around a circle. The power of the heating element is equal to the positive integer obtained by reading the digits on its control knob clockwise starting from the top of the knob.

![](https://cdn.luogu.com.cn/upload/image_hosting/p2wyrucc.png)

In a single step, you can rotate one or more consecutive knobs by any number of positions in any direction. However, all knobs rotated in one step need to be rotated by the same number of positions in the same direction.

Find the smallest number of steps needed to set all the heating elements to maximal possible power.

## �����ʽ
The first line contains an integer $n(1 \le n \le 501)$ �� the number of heating elements. The $j-th$ of the following $n$ lines contains an integer $x_j$ �� the initial power of the $j-th$ heating element. Each $x_j$ consists of exactly seven non-zero digits.


## �����ʽ
Output a single integer �� the minimal number of steps needed.

## ��Ŀ����
��Ŀ����

����һ�Ҵ��͵Ŀ�Ͳ����ľ�����̨����⿡������̨����n��¯���ų�һ�ţ��������Ϊ1-n�š�ÿ��¯�Ӷ��ᱻ���Ŀ����ֱ������ơ���Щ�ֱ��ɲ�һ�㣺ÿ���ֱ����涼��1-7�ĺ���Χ��һȦ����̨�Ļ������Ǵ����Ŀ����ֱ����˿�ʼ˳ʱ���ȡ���ֶ��õ��ġ�

��ͼƬ������������1����ĳ�ʼ�ֱ�λ����ͼ��ʾ��

ÿһ���㶼��ת��һ�����������ֱ����������ⷽ��ת�����⼸�¡����ǣ�ͬһ��ת�����ֱ�ֻ����ͬһ����ת��ͬ���Ĵ�����

�ҵ����ٵĲ����������е�¯�Ӷ��趨�����ܵ���������

���������ʽ

�����ʽ

��һ�а���һ��������1<=n<=501����ʾ¯�ӵ�����������ȥ��j�а���7���������������е�һ���ǳ�ʼ������С��

�����ʽ

���һ����������ʾ��Ҫ�Ĳ�����

```input1
6
9689331
1758824
3546327
5682494
9128291
9443696

```

```output1
3

```

```input2
7
5941186
3871463
8156346
9925977
8836125
9999999
5987743

```

```output2
2

```

## ��ʾ
In the first example, one of the ways to achieve maximal possible power is: rotate knobs $2$ through $3$ by $3$ positions in the counterclockwise direction, rotate knob $3$ by $3$ positions in the counterclockwise direction, and rotate knobs $4$ through $6$ by $2$ positions in the clockwise direction.


