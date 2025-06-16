## ��Ŀ����
A set of grid points in a plane (points whose both cartesian coordinates are integers) which we shall refer to as the pattern, as well as a group of other sets of grid points on the plane are given. We would like to know which of the sets are similar to the pattern, i.e. which of them can be transformed by rotations, translations, reflections and dilations so that they are identical to the pattern. For instance: the set of points $\{(0,0),(2,0),(2,1)\}$ is similar to the set $\{(6,1),(6,5),(4,5)\}$, it is however not similar to the set $\{(4,0),(6,0),(5,-1)\}$.

TaskWrite a programme which:

reads from the standard input the description of the pattern and the family of the investigated sets of points,determines which of the investigated sets of points are similar to the pattern,writes the outcome to the standard output.

��Ŀ������


����һ������ƽ���ϸ��ļ��ϣ����Ķ�����xy�����Ϊ�����������ǽ��������ģʽ���ϡ���


��������������ļ�������ƽ���ϵ�ļ��ϡ�������Ҫ��������������Щ���Ϻ͡�ģʽ���ϡ��ǡ����ơ��ģ������ü��Ͽ���ͨ�� ��ת��ƽ�ƣ���ת�������� ʹ�øü��Ϻ͡�ģʽ���ϡ���ȫ��ͬ��


����{(0,0),(2,0),(2,1)}������Ϻ�{(6,1),(6,5),(4,5)}������������Ƶģ�����{(4,0),(6,0),(5,-1)}��������ǲ����Ƶġ�


����


дһ������ʹ��


�ܴӱ�׼�����ȡ��ģʽ���ϡ�����Ҫ���죨�Ƿ����ƣ��ļ��ϣ��ж���Щ���Ϻ͡�ģʽ���ϡ����ƣ���������������׼���


�����ʽ��


��׼����ĵ�һ����һ������ k (1<=k<=25000)������ģʽ���ϡ��еĵ���


������k�У�ÿ������������һ���ո�ָ�����i+1�е��������ֱ����ģʽ���ϡ��е�i�����x�����y����(-20000<=x,y<=20000)


��ģʽ���ϡ��еĵ�������ͬ��


������һ��һ������n��������n����Ҫ����ļ���


��������n������Ҫ����ļ��ϵ�������


ÿ�������ĵ�һ�а���һ������l������ü����еĵ���(1<=l<=25000)


������l��ÿ�а����ü�����һ�����x�����y���꣬��һ���ո�ָ�(-20000<=x,y<=20000��Ϊ����)


������ͬһ�����еĵ�������ͬ��


�����ʽ��


��ĳ���Ӧ�����׼��������n�У�ÿ�д������һ����Ҫ����ļ��ϵĽ����


�����i����Ҫ����ļ����롰ģʽ���ϡ����ƣ����i��Ӧ��������TAK�����������е�yes


�����i��Ӧ��������NIE�����������е�no


## �����ʽ
In the first line of the standard input there is a single integer $k$ ($1\le k\le 25\ 000$) - the number of points the pattern consists of. In the following $k$ lines there are pairs of integers, separated by single spaces. The $(i+1)$'st line contains the coordinates of $i$'th point belonging to the pattern: $x_{i}$ and $y_{i}$ ($-20\ 000\le x_{i},y_{i} \le 20\ 000$). The points forming the pattern are pairwise different. In the next line there is the number of sets to be investigated: $n$ ($1\le n\le 20$). Next, there are $n$ descriptions of these sets. The description of each set begins with a line containing a single integer $l$ - the number of points belonging to that particular set($1\le l\le 25\ 000$).These points are described in the following lines, a single point per line. The description of a point consists of two integers separated by a single space - its coordinates $x$ and $y$ ($-20\ 000\le x,y\le 20\ 000$).The points which belong to the same set are pairwise different.


## �����ʽ
Your programme should write to the standard output $n$ lines - one for each of the investigated sets of points. The $i$'th line should contain the word TAK (i.e. yes in Polish), if the $i$'th of the given sets of points is similar to the pattern, or the word NIE (i.e. no in Polish) if the set does not satisfy this condition.


```input1
3
0 0
2 0
2 1
2
3
4 1
6 5
4 5
3
4 0
6 0
5 -1
```

```output1
TAK
NIE
```

