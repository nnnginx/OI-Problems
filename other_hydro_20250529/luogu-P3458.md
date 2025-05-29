## ��Ŀ����
Vicomte de Bajteaux is the owner of a renowned collection of boulders. Up to now, he has kept it in thecellars of his palace, but recently, he has decided to display the collection in his vast gardens.

The gardens have a shape of rectangle, whose sides are $1\ 000\ 000\ 000$ units long and are parallel to east-westand north-south geographical directions. For each boulder, vicomte has determined coordinates ofthe point, which he would like it to be placed in (the coordinates are simply distances to the southern and    western side of the garden), and gave them to his servants. Unfortunately he has forgot to tell them the orderof the coordinates (i.e. for some of the boulders the first coordinate of a point is the so called "$y$ coordinate",i.e. the ordinate, while for others the so called "$x$ coordinate", i.e. the abscissa).

The servants, unaware of thisfact, have placed the boulders assuming customary coordinate ordering (as in standard Cartesian coordinates:

the abscissa, commonly known as "$x$ coordinate", first).

To protect his collection, vicomte has decided to surround it with a fence. For aesthetic reasons thefence has to be a rectangle, with sides parallel to the sides of the garden. The garden layout has been planned,      so that the total length of the fence be minimal (i.e. in the space of all coordinate orderings, the original          ordering of vicomte requires the minimal length of the fence - we assume that the rectangle may have sides of zero length).

The servants have to move the boulders so that the length of the fence required is minimal lest their mistake become obvious. Each boulder may only be moved in a way that preserves the coordinate set: by      interchanging its coordinates. As the boulders are heavy, the servants would like to minimize their effort, by      minimizing the weight of the boulders to be moved.

## Task

Write a programme which:

reads the present positions of the boulders in the gardens and their respective weights, determines a sequence of moves, which minimizes the length of the fence required to protect the    boulders and also minimizes the weight of the boulders to be moved, writes the outcome to the standard output.

## �����ʽ
The first line of the standard input contains a single integer $n$ ($2 \le n \le 1\ 000\ 000$), denoting the number of boulders in the collection. The following $n$  lines contain three integers $x_i$, $y_i$ and $m_i$ each ($0 \le x_i, y_i \le 1\ 000\ 000\ 000$, $1 \le m \le 2000$), separated by single spaces, denoting the present coordinates and the weight of $i$'th boulder. No unordered pair of coordinates will appear in the input more than once.


## �����ʽ
The first line of the standard output should contain two integers, separated by a single space - the minimal length of fence possible and the minimal weight of the boulders to be moved in order to obtain such a length.


The second line should contain a sequence of $n$ zeros and/or ones - $i$'th element of the sequence should be a one if in the optimal solution the $i$'th boulder is to be moved and zero otherwise. Should more than one correct solutions exist, your programme is to write out any one of them.


## ��Ŀ����
### ��Ŀ����

**���� POI 2007 Stage 2. Day 1��[Skalniak](https://szkopul.edu.pl/problemset/problem/s5ECsFKlMHti0g29uVkdKlQw/site/?key=statement)��**

Vicomte de Bajteaux �ղ������ʯͷ��׼�������Ƿŵ���԰�

��԰��һ�������Σ��߳�Ϊ $1\ 000\ 000\ 000$��Vicomte de Bajteaux ����������Ϊ����ʯͷ���û�԰���������Ǹ������������˳��������һЩ��������� $(x,y)$ ����ʽ������һЩ��������� $(y,x)$ ����ʽ����������ʯͷ�Ѿ���������˳��ź��ˡ�

Ϊ�˱���ʯͷ��Vicomte de Bajteaux ����ʵ�ʵ�����滮��һ��դ����Χס��Щʯͷ��ʹ��դ�����ܳ���С��Ϊ�����ۣ�դ��������ƽ����������ľ��Ρ�Ϊ���ô�����ô���ԣ�����Ҫ��������ѡ��һ����ʯͷ�������Ǵ� $(x,y)$ �ƶ��� $(y,x)$������С��դ���ĳ��ȵĻ�������С����Ҫ�ƶ���ʯͷ�����ء�

### �����ʽ

��һ��һ������ $n (1 \le n \le 1\ 000\ 000)$����ʾʯͷ�ĸ�����

������ $n$ ��ÿ���������� $x_i, y_i, m_i$��$0 \le x_i,y_i \le 1\ 000\ 000\ 000, 1 \le m_i \le 2\ 000$������ʾʯͷ��ǰ���ڵ������������

������ $x$ �� $y$ ��ɵ��������Գ��ֳ���һ�Ρ�

### �����ʽ

��һ����������������ֱ��ʾդ������С���Ⱥ���Ҫ�ƶ���ʯͷ����������Сֵ��

�ڶ������һ������Ϊ $n$ �� 01 ������ʾȡ��ʯͷ��������Сֵ��һ���ƶ��������� $i$ ���ַ�Ϊ $1$ ��ʾ��Ҫ���� $i$ ��ʯͷ�� $(x_i, y_i)$ �ƶ��� $(y_i, x_i)$��Ϊ $0$ ���ʾ����Ҫ�����ж�⣬�������һ�ֽⷨ�����ԡ�

### ��������

![](https://cdn.luogu.com.cn/upload/image_hosting/gjo0jemf.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/09zdeg0c.png)

���������� [LibreOJ](https://loj.ac/p/2655)��

```input1
5
2 3 400
1 4 100
2 2 655
3 4 100
5 3 277
```

```output1
10 200
01010
```

