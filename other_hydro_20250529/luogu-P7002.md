## ��Ŀ����


The technological progress in Flatland is impressive. This year, for example, the solar power stations of a new type will be build. In these stations solar panels are mounted not on the ground, but on high towers, along their heights.

There are $n$ towers to be mounted. The towers are already bought. The height of i-th tower is $h_{i}.$ Now engineers want to choose the points where they should be mounted to get the maximal total power.

The landscape of a territory of the power plant is described by a polyline with $m$ vertices. Vertices of the landscape polyline have coordinates $(x_{i}, y_{i}),$ such that $x_{i} < x_{i+1}.$

The sun angle is always $��$ degrees in Flatland. The sun is shining from the top-left to the bottom-right. The power that is produced by a tower depends on the length of its surface illuminated by the sun.

When two towers are mounted close to each other, the shadow of the left tower may fall onto the right tower, so the power, produced by the right tower, decreases. Also, the landscape itself may contain high points that drop shadows on some towers.

![](/upload/images2/ge.png)

Your task is to find the points on the territory of the plant to mount the given towers to maximize the total length of towers surface that is illuminated by the sun.



## �����ʽ


The first line of the input file contains three integers $n , m$ and $�� (1 \le n \le 10^{4}, 2 \le m \le 10^{4}, 1 \le �� < 90)$ . The second line contains $n$ integers $h_{i}$ -- the heights of the towers $(1 \le h_{i} \le 10^{3}).$ The following $m$ lines contain pairs $x_{i}, y_{i}$ -- the coordinates of the vertices of the landscape $(|x_{i}| \le 10^{5}, x_{i} < x_{i+1}, |y_{i}| \le 10^{3}).$



## �����ʽ


On the first line output the maximal possible summary length of towers that can be illuminated by the sun with an absolute precision of at least $10^{-6}.$ On the next $n$ lines output the x-coordinates of the points where the towers should be mounted to achieve this maximum with an absolute precision of at least $10^{-9}.$ Towers should be listed in the same order they are given in the input file.



## ��Ŀ����
## ��Ŀ���� ##
ƽ���ϵļ����������˾�̾��������Ҫ����һ�����͵�̫���ܷ���վ������Щ����վ�У�̫���ܵ�ذ岻�ǰ�װ�ڵ����ϣ����ǰ�װ�ڸ����ϡ�

�ڶ�Ϊ��������Ҫ��װ$i$����������Щ�����߹̶�����$i$�����ĸ߶���$h_i$�����ڣ�����ʦ����Ҫѡ��װ�㣬�Ի�������ܹ��ʡ�

�糧��������$m$����������ӡ���Щ�ߵĶ�������Ϊ$(x_i,y_i)$����$x_i<x_{i+1}$
��ƽ���ϣ�̫���ĽǶ�����$\alpha$�ȡ�̫�������Ͻ����䵽���½ǡ��������Ĺ���ȡ��������汻̫����������(��ʵ�ǳ���)��

����װ���������˴˿���ʱ�����������Ӱ���������Ҳ����ϣ��Ӷ��Ҳ��������Ĺ��ʽ��͡����⣬�糧��������ܰ�����ĳЩ��¥��Ͷ����Ӱ�ĸߵ㡣

����������ڵ糧�������ҵ���װ�������ܵĵ㣬�Եõ�̫����������������ܱ����(����)��

## �����ʽ ##

�����һ�а�������������$n$,$m$,$\alpha$ $(1 \le n \le 10^4,2 \le m \le 10^4,1 \le \alpha <90)$���ڶ��а���$n$����$h_i$(���ߣ�$(1 \le h_i \le 10^3)$�������$m$��ÿ����$x_i$,$y_i$һ�������糧��������)$(|x_i|\le 10^5,x_i < x_{i+1},|y_i|\le 10^3)$

## �����ʽ ##

��һ��:������$10^{-6}$��������ɱ�̫�����������������ܻ������������)���ں�n���ϣ������ʱ����װ���x���꣬���Ծ�������Ϊ$10^{-9}$���������˳��Ӧ������˳����ͬ��

## ˵��/��ʾ ##
ʱ�����ƣ�1h

�ռ�˳��128PB

```input1
5 4 10
20 10 20 15 10
0 10
40 20
50 0
70 30

```

```output1
52.342888649592545
16.0
0.0
70.0
65.3
65.3

```

## ��ʾ
Time limit: 1 s, Memory limit: 128 MB. 



