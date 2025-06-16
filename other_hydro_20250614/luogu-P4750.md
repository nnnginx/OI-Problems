## ��Ŀ����
A satellite is surveying a possible rover landing area on the moon. The landing area is modeled as a square grid embedded in the standard coordinate system.

The satellite has taken $n$ photos, each capturing a square area of the surface. Careful camera calibration has ensured that all photos are aligned with the grid �� all four vertices have integer coordinates. Due to the satellite��s changing orbit there are two types of photos:
   - Photos of type ``A`` have sides that are parallel to coordinate axes. Such a photo is specified by giving the integer coordinates $(x, y)$ of the square��s middle point and the length of its side $a$ �� always an even integer.
   - Photos of type ``B`` have sides at a $45^{\circ}$ angle to the coordinate axes. Such a photo is specified by giving the integer coordinates $(x, y)$ of the square��s middle point and the length of its diagonal $d$ �� always an even integer.

Find the total surface area captured in the satellite photos.


## �����ʽ
The first line contains an integer $n(1 \le n \le 200 000)$ �� the number of photos. The $j-th$ of the following $n$ lines is either of the form ��$A \ x_j \ y_j  \ a_j$�� or ��$B \ x_j \ y_j \ d_j$�� representing a photo of type ``A`` or ``B``,respectively.

The $x_j$ and $y_j$ are the integer coordinates of the middle point of the photo $(-1 000 \le x_j, y_j \le 1 000)$. The $a_j$ and $d_j$ are even integers $(2 \le a_j, d_j \le 1 000)$ �� the side length and the diagonal length, respectively.

## �����ʽ
Output a number with exactly two digits after the decimal point �� the total area of the surface. The answer has to exactly correspond to the judge��s solution (no rounding errors are tolerated).

## ��Ŀ����
��������ĸ��ʽ���ò�����

����ľ���

��Ŀ����

һ����������Ϊ̽�⳵��������Ѱ��һ�����ʵĽ���������������������ƽ��ֱ������ϵ�е�һ����������

��������Ѿ�����n����Ƭ��ÿ����Ƭ����������������һ�����������򡣾���������ľ�ϸУ׼�����Ա�֤������Ƭ���ǵ����򶼺�������롪���������ĸ��ǵ����궼Ϊ�������������ǵĹ��һֱ�ڱ仯��������Ƭ��������ʽ��
��A����Ƭ�ı�Ե��������ƽ�С�������������Ƭ����Ŀ������������ĵ�����(x,y)�����ı߳�a��aΪż������
��B����Ƭ�ı�Ե���������45��ǡ�������������Ƭ����Ŀ������������ĵ�����(x,y)�����Խ��ߵĳ���d��dΪż������

�������ͼƬ���㵽ƽ����ܴ�С��

���������ʽ

�����ʽ��

��һ����һ������n(1��n��200000)��ʾ��Ƭ��������������n���е�j�еĸ�ʽ��"A xj yj aj"��"B xj yj dj" ���ֱ��ʾ������Ƭ��������A��B��

xj��yj������ͼƬ���ĵ�����(1000��xj,yj��1000)��aj��djΪż��(2��aj,dj��1000)���ֱ��ʾ�����εı߳��ͶԽ��߳��ȡ�

�����ʽ��

���ƽ���ܵĴ�С��������λС�����𰸱���ͱ�׼���ϸ���ȣ��������������̨I(^��^)�J����

```input1
2
A 0 0 2
B 1 0 2
```

```output1
5.00
```

```input2
8
A -7 10 4
B 3 10 8
A -6 6 6
A -2 5 8
B 3 -1 8
B -7 -4 8
A 3 9 2
B 8 6 6

```

```output2
205.50
```

