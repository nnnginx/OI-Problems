## ��Ŀ����
Art critics worldwide have only recently begun to recognize the creative genius behind the great bovine painter, Picowso.


Picowso paints in a very particular way. She starts with an $N \times N$ blank canvas, represented by an $N \times N$ grid of zeros, where a zero indicates an empty cell of the canvas. She then draws $N^2$ rectangles on the canvas, one in each of $N^2$ colors (conveniently numbered $1 \ldots N^2$). For example, she might start by painting a rectangle in color 2, giving this intermediate canvas:


```
2 2 2 0

2 2 2 0

2 2 2 0

0 0 0 0
```




She might then paint a rectangle in color 7:

```
2 2 2 0

2 7 7 7

2 7 7 7

0 0 0 0
```




And then she might paint a small rectangle in color 3:

```
2 2 3 0

2 7 3 7

2 7 7 7

0 0 0 0
```


Each rectangle has sides parallel to the edges of the canvas, and a rectangle could be as large as the entire canvas or as small as a single cell. Each color from $1 \ldots N^2$ is used exactly once, although later colors might completely cover up some of the earlier colors.


Given the final state of the canvas, please count how many of the $N^2$ colors could have possibly been the first to be painted.

## �����ʽ
The first line of input contains $N$, the size of the canvas ($1 \leq N \leq 1000$).

The next $N$ lines describe the final picture of the canvas, each containing $N$ integers that are in the range $0 \ldots N^2$. The input is guaranteed to have been drawn as described above, by painting successive rectangles in different colors.


## �����ʽ
Please output a count of the number of colors that could have been drawn first.


## ��Ŀ����
### ��Ŀ����

������ص��������ۼ�����ſ�ʼ��ʶ��ΰ�����ţ���� Picowso �Ĵ�����š�

Picowso ��һ�ַǳ����صķ�ʽ����������һ�� $N \times N$ �Ŀհ׻�����ʼ��������һ�� $N \times N$ ���������ʾ���������ʾ������һ���յ�Ԫ��Ȼ�����ڻ����ϻ��� $N^2$ �����Σ�ÿ������ʹ�� $N^2$ ����ɫ�е�һ�֣�������ñ�� $1 \ldots N^2$ ��ʶ�������磬��������������ɫ 2 ����һ�����Σ��õ������м仭����

```
2 2 2 0

2 2 2 0

2 2 2 0

0 0 0 0
```

Ȼ������������ɫ 7 ����һ�����Σ�

```
2 2 2 0

2 7 7 7

2 7 7 7

0 0 0 0
```

��������������ɫ 3 ����һ��С���Σ�

```
2 2 3 0

2 7 3 7

2 7 7 7

0 0 0 0
```

ÿ�����εı߶��뻭���ı�Եƽ�У����ο��Դ�����������Ҳ����С��һ����Ԫ��ÿ����ɫ�� $1 \ldots N^2$ ǡ��ʹ��һ�Σ����ܺ�������ɫ���ܻ���ȫ����һЩ��ǰ����ɫ��

��������������״̬��������ж�������ɫ�����ǵ�һ�������Ƶġ�

### �����ʽ

����ĵ�һ�а��� $N$����ʾ�����Ĵ�С��$1 \leq N \leq 1000$����

�������� $N$ ����������������״̬��ÿ�а��� $N$ ����������Χ�� $0 \ldots N^2$�����뱣֤�ǰ���������ʽͨ���������Ʋ�ͬ��ɫ�ľ������ɵġ�

### �����ʽ

����������ǵ�һ�������Ƶ���ɫ��������

### ˵��/��ʾ

����������У���ɫ 2 �����ǵ�һ�������Ƶġ���ɫ 3 ��Ȼ��������ɫ 7 ֮����ƣ�����ɫ 7 ��Ȼ��������ɫ 2 ֮����ơ���������û�п���������ɫ�������ƶ�����Ҳ�����ǵ�һ�������Ƶġ�

```input1
4
2 2 3 0
2 7 3 7
2 7 7 7
0 0 0 0
```

```output1
14
```

## ��ʾ
In this example, color 2 could have been the first to be painted. Color 3 clearly had to have been painted after color 7, and color 7 clearly had to have been painted after color 2. Since we don't see the other colors, we deduce that they also could have been painted first.

