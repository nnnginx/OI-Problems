## ��Ŀ����
A mirror trap is a cuboid made of mirrors, the reflecting sides of which are facing the interior of the cuboid. Precisely in the geometric centre of the cuboid there is a miniature laser (whose dimensions we shall neglect). The task is to aim the laser in such a way that the beam travels the longest total distance possible and returns to the laser itself. By total distance we shall denote the sum of distances traveled by the laser beam in each of the three directions parallel to the edges of the mirrors (i.e. we are using the so called Manhattan (city) metric).

�����������ɾ��ӹ��ɵĳ����壬���ӵķ�������ų�������ڲ����ڳ�����ļ������ķ���һ��΢�ͼ��������ߴ���ԣ����������ǵ������ǰѼ�����ĳһ�������䣬����ʹ�����ڻص�����������֮ǰ��ͨ�����ܾ��뾡���ܳ���ͨ�����ܾ����ʾΪ���������뾵�ӷ�����ƽ�е���������ľ���֮�ͣ�Ҳ���������٣����У�������

The dimensions of the trap are even integers. The edges and vertices of the trap, where distinct sides meet, do not reflect the laser beam. Inside the cuboid we shall introduce a cartesian coordinate system. Its axes are parallel to the edges of the trap and the laser shall be placed in the origin. The laser may be aimed at any integer point (a point whose all coordinates are integers) within the trap, the points on the surface of the mirrors included (with the single exception of the laser itself, i.e. the point $(0,0,0)$).

��ͬ�Ĳ�������������ıߺͶ��㲻�ᷴ�伤������������ı߳����������ڳ����������У�ʹ�õѿ�������ϵ������ϵ���ݺ���ֱ�ƽ��������ĳ��Ϳ���������λ����ԭ�㡣������������׼�����ڵ�����һ����������侵�ı����ϵĵ㣨Ψһ��������Ǽ����������㣨0,0,0������

TaskWrite a programme which:

reads from the standard input the dimensions of the mirror trap,calculates such a point, that a laser beam fired from the laser it the direction of this point:

shall be reflected from the mirrors (but not necessarily from all of them),  shall neither intersect an edge nor a vertex of the mirror trap,  shall return to the laser, possibly from a different direction,  shall travel the longest total distance possible (in the sense of the definition provided).

writes the outcome to the standard output.

���ǵ�����

���������������ĳߴ磬ͨ����д�ĳ�������һ���㣬��������ָ����һ�㣺��һ������Ӧ�ڷ��侵������һ�������з��侵�����䣬���ǲ�������ıߡ������ཻ�������Ҫ�ص���������������Ҫһ���ķ���ͬʱ������ʹ���ܾ��볤��


## �����ʽ
A single test consists of many mirror traps to be analysed. The first line of the standard input contains a single integer $1\le K\le 1000$, denoting the number of traps to be analysed. In the lines $2..K+1$ there are descriptions of the traps, a single per line. The description of the trap consists of three numbers $5\le x,y,z\le 1000$, separated by single spaces. The mirror trap has the dimensions of $2x\times 2y\times 2z$.

�����ж�����塣����ĵ�һ�а���һ������ K��1��K��1000������ʾҪ�������������� ��2.K + 12..K + 1���У���һ�������������ÿ��һ���� ����������������ÿո�ָ�������5��x��y��z��1000��ɡ� ��������ĳߴ�Ϊ2x��2y��2z��


## �����ʽ
Your programme should write exactly $K$ lines to the standard output. The $i$'th line should contain a solution for the $i$'th trap: three integers $k_x,k_y,k_z$separated by single spaces, $-x\le k_{x}\le x$, $-y\le k_{y}\le y$, $-z\le k_{z}\le z$,$ \{k_{x},k_{y},k_{z}\}\neq\{0,0,0\}$. Those numbers signify that in the $i$'th trap the laser should be aimed at the point, whose coordinates are $\{k_{x},k_{y},k_{z}\}$.

Should there be a greater number of correct solutions, your programme ought to output any one of them.

���K�С� ��K��Ӧ������K������Ľ���������ɿո�ָ���3����x��y��z����ʾ��������Ҫ��׼�ĵ�����ꡣ

����ж����ͬ����ȷ�������������������һ����


```input1
2
5 6 7
5 6 6
```

```output1
4 5 6
4 6 5
```

## ��ʾ
��л@SLYZ\_0120 �ṩ���롣


