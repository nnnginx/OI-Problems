## ��Ŀ����
����ϵ�������ɸ�����ֱ�������Σ���ÿ������ֱ�������ε�ֱ�Ƕ��㶼�����·���������������ƽ�С��������������θ��ǵ��������Ϊ��ɫ����ż���������θ��ǵ��������Ϊ��ɫ������ͼ��ʾ��
![](https://cdn.luogu.com.cn/upload/pic/18669.png)
��֪ $N$������ֱ�������εĶ������꼰���������ɫ���������

Mirko and Slavko have built their own LED display. The display is initially
white. During each of the $N$ parts of the testing phase, Mirko attached three
electrodes to the display in such way that they formed a right isosceles
triangle. He noticed that, after attaching the electrodes, all pixels in the
enclosing triangle are inverted (white pixels become black, and black pixels
become white).

Watching Mirko play with the electrodes, Slavko observed interesting shapes
emerging on the screen. Mathematically inclined as he is, first thing that
crossed his mind was how to calculate total area covered by black pixels. Help
him by writing a program to do just that!

## �����ʽ
�����һ�а���һ������ $N$����ʾ����ֱ��������������

������ $N$�У�ÿ���������� $X, Y, R$���ֱ��ʾ����ֱ�������εĶ������� $(X, Y)$������ $R$��

First line of input contains an integer $N(1 \leq N \leq 10)$, number of triangles
formed by Mirko's fiddling with electrodes. Each of the following $N$ lines
contains three integers $X, Y$ and $R (1 \leq X, Y, R \leq 10^6
)$, describing a triangle. $(X, Y)$ are the coordinates of the lower left corner of the triangle, while $R$ represents the length of the two sides of the triangle.

## �����ʽ
�������һ��ʵ������ʾ��ɫ�������������1λС����

The first and only line of output should contain the area covered by black
pixels, rounded to one decimal place.

```input1
3
1 1 2
7 1 6
5 3 4
```

```output1
24.0
```

```input2
5
5 5 99
5 5 99
5 5 99
5 5 99
5 5 99
```

```output2
4900.5
```

```input3
4
5 5 99
5 5 99
5 5 99
5 5 99
```

```output3
0.0
```

## ��ʾ
$1 \leq N \leq 10, 1 \leq X, Y, R \leq 10^6$

