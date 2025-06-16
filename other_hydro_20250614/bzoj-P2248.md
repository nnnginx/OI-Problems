

## ��Ŀ����
>John and Brus are playing a military strategic game on a PC. The game is played on the flat world map. At the beginning of the game Brus places his army. Then John has to choose strategic points for his army according to the following rules: 
>each strategic point must be a lattice point (x, y) (a lattice point is a point with integer coordinates) such that |x| + |y| < N; 
John can choose any positive number of strategic points; 
all the strategic points must be distinct; 
each of the strategic points must be free (i.e. not occupied by Brus��s army); 
each pair of different strategic points must be connected (possibly via some other strategic points). 
>Here two different lattice points (x1, y1) and (x2, y2) are connected if |x1 �C x2| + |y1 �C y2| = 1. If A, B and C are strategic points, A and B are connected, B and C are connected, then A and C are also connected. 
Your task is to find the number of ways for John to choose strategic points for his army.

## ���ķ���

John �� Brus ������һ������ս����Ϸ����Ϸ��һ��ˮƽ��ͼ�Ͻ��У�����Ϸ��ʼʱ Brus �᲼�����ľ��ӣ�Ȼ�� John ��ҪΪ���ľ���ѡ��ս�Ե㣬ѡ��ս�Ե�����ѭ���¹���

- ս�Ե������ $(x,y)$ ��Ϊ���������� $|x|+|y| \lt n$��
- ��ͬս�Ե���뻥����ͬ��
- ����ѡ�� Brus �Ѿ�ռ��ĵ���Ϊս�Ե㡣
- ս�Ե�֮������ͨ���˴�����ָͨ��������ͨ����

����Ҫ��� John ����ս�Ե�ķ������� 

## �����ʽ
>The first line contains single integer T �C the number of test cases. Each test case starts with a line containing two integers N and M separated by a single space. N is the number mentioned in the first rule. M is the number of lattice points on the world map already occupied by Brus��s army. Each of the following M lines contains two integers Xk and Yk separated by a single space. Each lattice point (Xk, Yk) is occupied by Brus��s army.

��һ��һ������ $T$����������������

ÿ�����ݵĵ�һ�а��������� $n,m$������ $n$ Ϊ��һ�������е� $n$��$m$ Ϊ Brus �Ѿ�ռ��ĵ�ĸ�����

������ $m$ �У�ÿ���������� $x,y$�������� Brus ռ��ĵ�����ꡣ
## �����ʽ
>For each test case print a single line containing the number of ways for John to choose strategic points for his army.

��ÿ�����ݣ�������Ӧ�Ĵ𰸡�

```input1
2 
2 1 
7 7 
2 3 
0 0 
4 -7 
7 -4

```
```output1
20 
4

```
$1\le T\le 74,1\le n\le 7,1\le m\le 225,-7\le x,y\le 7$������ $x,y$ ������ͬ��
## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
û��д����Դ


