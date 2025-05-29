## ��Ŀ����
It's a hot summer day, and Bessie the cow is feeling quite lazy. She wants to locate herself at a position in her field so that she can reach as much delicious grass as possible within only a short distance.

There are $N$ patches of grass $(1 <= N <= 100,000)$ in Bessie's field. The $ith$ such patch contains $g_i$ units of grass $(1 <= g_i <= 10,000)$ and is located at a distinct point $(x_i, y_i)$ in the field $(0 <= x_i,$ $y_i <= $ $1,000,000)$.  Bessie would like to choose a point in the field as her initial location (possibly the same point as a patch of grass, and possibly even a point with non-integer coordinates) so that a maximum amount of grass is within a distance of $K$ steps from this location $(1 <= K <= 2,000,000)$.

When Bessie takes a step, she moves 1 unit north, south, east, or west of her current position.  For example, to move from $(0,0)$ to $(3,2)$, this requires 5 total steps.  Bessie does not need to take integer-sized steps -- for example, 1 total step could be divided up as half a unit north and half a unit east.

Please help Bessie determine the maximum amount of grass she can reach, if she chooses the best possible initial location.


## �����ʽ
* Line 1: The integers $N$ and $K$.

* Lines 2..1+N: Line $i+1$ describes the $ith$ patch of grass using 3 integers: $g_i, x_i, y_i.$


## �����ʽ
* Line 1: The maximum amount of grass Bessie can reach within $K$ steps, if she locates herself at the best possible initial position.

## ��Ŀ����
```
  Bessie��������N(1<=N<=100,000)��ݵأ�ÿ��ݵص������� (xi, yi) (0<=xi,yi<=1,000,000),���泤��gi(1<=gi<=10,000)����λ�����ݡ� 
  Bessie�����������������ߣ�һ����һ����һ����λ���ȣ��������ӣ�0,0���ߵ���3,2����Ҫ5������������һ����k (1<=k<=2,000,000) ����
  ����������һ��λ�ã�ʹ���Ӹ�λ�ó������Եõ���൥λ������(�������߶�Σ���ÿ�ζ��Ӹ�λ�ó���)�� 
  �����ʽ�� 
  ��1�У���������N��K 
  ��2~N+1�У���������gi��xi��yi 
  �����ʽ�� 
  ��1�У�Bessie���ܻ�õ���൥λ������
```

```input1
4 3
7 8 6
3 0 0
4 6 0
1 4 2
```

```output1
8
```

## ��ʾ
INPUT DETAILS:

Bessie is willing to take at most 3 steps from her initial position.  There
are 4 patches of grass.  The first contains 7 units of grass and is located
at position $(8,6)$, and so on.

OUTPUT DETAILS:

By locating herself at $(3,0)$, the grass at positions $(0,0)$, $(6,0)$, and
$(4,2)$ is all within $K$ units of distance.

