## ��Ŀ����
ICPC2020 WF F

## ��Ŀ����
In 1921, the amateur archaeologist Alfred Watkins coined the term
"ley lines" to refer to straight lines between numerous places of
geographical and historical interest. These lines have often been
associated with mysterious and mystical theories, many of which still
persist.

One of the common criticisms of ley lines is that lines one draws on a
map are actually of non-zero width, and finding "lines" that connect
multiple places is trivial, given a sufficient density of points and a
sufficiently thick pencil. In this problem you will explore that
criticism.

For simplicity, we will ignore the curvature of the earth, and just assume
we are dealing with a set of points on a plane, each of which has a
unique $(x, y)$ coordinate, and no three of which lie on a single
straight line. Given such a set, and the thickness of your pencil,
what is the largest number of points through which you can draw a
single line?

## �����ʽ
The first line of input consists of two integers $n$ and $t$, where
$n$ ($3 \le n \le 3\,000$) is the number of points in the set
and $t$ ($0 \le t \le 10^9$) is the thickness of the pencil.
Then follow $n$ lines,
each containing two integers $x$ and $y$ ($-10^9 \le x, y \le 10^9$),
indicating the coordinates of a point in the set.

You may assume that the input is such that the answer would not change
if the thickness $t$ was increased or decreased by $10^{-2}$, and that no
three input points are collinear.

## �����ʽ
Output the maximum number of points that lie on a single "line" of
thickness $t$.

## ��Ŀ����
1921 �꣬ҵ�࿼��ѧ�� Alfred Watkins ����� _Ley lines_ �ĸ��ָ���������ڶ�������ʷ��ʤ��ֱ�ߡ���Щ�߳��������ص�������ϵ��һ�����������������������

�� _Ley lines_ ��һ�����������ǣ������ڵ�ͼ�ϻ��Ƶ��ߵĿ��ʵ���ϲ���Ϊ $0$�����ǵ��㹻�ܼ��ĵ���㹻���Ǧ�ʣ��ҵ����Ӷ���ط��ġ��ߡ��Ǻ����׵ġ�Ϊ��̽���������飬�����������һ����άƽ��������ʵ����

���ڣ������άƽ������ $n$ ���㣬�� $i$ ���������Ϊ $(x_i,y_i)$������û����������ͬһ��ֱ���ϡ�����һ�����Ϊ $t$ ��Ǧ�ʣ�����֪��������֧Ǧ�ʻ�һ���ߣ�����ܹ����Ӷ��ٸ���ͬ�ĵ㡣����Լ����� $t$ ���ӻ���� $10^{-2}$ ������£����ǲ���ı�ġ�

���ݷ�Χ��

- $3\leqslant n\leqslant 3000$��$0\leqslant t\leqslant 10^9$��
- $-10^9\leqslant x_i,y_i\leqslant 10^9$��

Translated by Eason_AC

```input1
4 2
0 0
2 4
4 9
3 1
```

```output1
3
```

```input2
3 1
0 10
2000 10
1000 12
```

```output2
2
```

