## ��Ŀ����
Byteburg, the capital of Byteotia, is a picturesque city situated in a valley in the midst of mountains. Unfortunately,  recent heavy rainfall has caused a flood - all the Byteburg is now completely under water. Byteasar,  the king of Byteotia, has summoned his most enlightened advisors, including you, to a council. After long  deliberations the council agreed to bring a few pumps, set them up in the flooded area and drain Byteburg.

The king has asked you to determine the minimum number of pumps sufficing to drain the city.

You are provided with a map of the city and the valley it is situated in. The map is in the shape of a $m\times n$ rectangle, divided into unitary squares. For each such square the map tells its height above sea level and alsowhether it is a part of Byteburg or not. The whole area depicted in the map is under water. Furthermore, it issurrounded by much higher mountains, making the outflow of water impossible. Obviously, there is no needto drain the area that does not belong to Byteburg.

Each pump can be placed in any unitary square depicted in the map. The pump will be drawing thewater until its square is completely drained. Of course, the communicating tubes principle makes its work,      so draining one square results in lowering the water level or complete draining of those squares from which      the water can flow down to the one with the pump. Water can flow only between squares with a common side      (or, more exact, squares whose projections onto horizontal plane have a common side, since the squares may       be at different level). Apart from that, the water obviously only flows down.

## Task

Write a programme that:

- reads description of the map from the standard input,

- determines the minimum number of pumps needed to drain whole Byteburg,

- writes out the outcome to the standard output.

## �����ʽ
In the first line of the standard input there are two integers $m$ and $n$, separated by a single space, $1 \le n, m \le 1\ 000$. The following $m$ lines contain the description of the map. The $(i+1)$'th line describes the $i$'th row of unitary squares in the map. It contains $n$ integers $x_{i,1}, x_{i,2}, ..., x_{i_n}$, separated by single spaces,$-1\ 000 \le x_{i,j} \le 1\ 000$ ,$x_{i,j} \ne 1000$ . The number $x_{i,j}$ describes the $j$'th square of the $i$'th line. The ground level in this square is $|x_{i,j}|$ above sea level. If $x_{i,j} > 0$, then the square is part of Byteburg, otherwise it is outside the city. Notice, that the area of Byteburg need not be connected. In fact the city may have several separate parts.


## �����ʽ
Your programme should write out one integer to the standard output - the minimum number of pumpsneeded to drain Byteburg.


## ��Ŀ����
### ��Ŀ����

**���� POI 2007 Stage 2. Day 1��[The Flood](https://szkopul.edu.pl/problemset/problem/VutzcR1iPvGuYRGZgvNksmV1/site/?key=statement)��**

����һ�� $m \times n$ �ĵ�ͼ����ͼ�����е㶼����ˮ��û�ˡ���֪����ͼ��ÿ������ĺ��θ߶ȣ�����һ���ֵ����� Byteburg �ǡ�����Ҫ���þ������ٵľ��ͳ�ˮ������ Byteburg �ǴӺ�ˮ�н�ȳ��������ͳ�ˮ�����ɸø��ӵ�����ˮ��ֱ���ø��Ӳ�����ˮ��ûΪֹ��

ˮ�����й����ߵĸ��Ӽ�Ӹ����������

### �����ʽ

��һ���������� $m,n$��$1 \le m,n \le 1000$����

������ $m$ ��ÿ�� $n$ ������ $x_{i1}, x_{i2}, \ldots, x_{in} (-1000 \le x_{ij} \lt 1000)$����ʾ��ͼ���� $i$ �е� $j$ �и��ӵĺ��θ߶�Ϊ $\lvert x_{ij} \rvert$������� $x_{ij} \gt 0$������������� Byteburg ���ڣ������ڳ��⡣����֤ Byteburg ���γ�һ����ͨ�顣

### �����ʽ

���һ��һ����������ʾ������Ҫ�ĳ�ˮ����������

### ��������

![](https://cdn.luogu.com.cn/upload/image_hosting/6cal4wth.png)

���������� [LibreOJ](https://loj.ac/p/2654)��

```input1
6 9
-2 -2 -1 -1 -2 -2 -2 -12 -3
-2 1 -1 2 -8 -12 2 -12 -12
-5 3 1 1 -12 4 -6 2 -2
-5 -2 -2 2 -12 -3 4 -3 -1
-5 -6 -2 2 -12 5 6 2 -1
-4 -8 -8 -10 -12 -8 -6 -6 -4
```

```output1
2
```

