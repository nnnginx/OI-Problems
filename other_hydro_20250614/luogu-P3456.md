## ��Ŀ����
Byteasar loves trekking in the hills. During the hikes he explores all the ridges and valleys in vicinity.

Therefore, in order to plan the journey and know how long it will last, he must know the number of ridgesand valleys in the area he is going to visit. And you are to help Byteasar.

Byteasar has provided you with a map of the area of his very next expedition. The map is in the shape ofa $n\times n$ square. For each field $(i,j)$ belonging to the square(for $i,j\in \{1,\cdots,n\}$), its height $w_{(i,j)}$ is given.

We say two fields are adjacent if they have a common side or a common vertex (i.e. the field $(i,j)$ is adjacent to the fields $(i-1,j-1)$,$(i-1,j)$,$(i-1,j+1)$,$(i,j-1)$,$(i,j+1)$,$(i+1,j-1)$,$(i+1,j)$,$(i+1,j+1)$, provided that these fields are on the map).

We say a set of fields $S$ forms a ridge (valley) if:

all the fields in $S$ have the same height,the set $S$ forms a connected part of the map (i.e. from any field in $S$ it is possible to reach any other    field in $S$ while moving only between adjacent fields and without leaving the set $S$),if $s\in S$ and the field $s'\notin S$ is adjacent to $s$, then $w_s>w_{s'}$(for a ridge) or $w_s<w_{s'}$ (for a valley).

In particular, if all the fields on the map have the same height, they form both a ridge and a valley.

Your task is to determine the number of ridges and valleys for the landscape described by the map.

TaskWrite a programme that:

reads from the standard input the description of the map,        determines the number of ridges and valleys for the landscape described by this map,        writes out the outcome to the standard output.

����һ�ŵ���ͼ����ɽ���ɽ�ȵ�����


## �����ʽ
In the first line of the standard input there is one integer $n$ ($2\le n\le 1\ 000$)denoting the size of the map. Ineach of the following $n$ lines there is the description of the successive row of the map. In $(i+1)$'th line(for $i\in \{1,\cdots,n\}$) there are $n$ integers $w_{(i,1)},\cdots,w_{(i,n)}$($0\le w_i\le 1\ 000\ 000\ 000$), separated by single spaces. Thesedenote the heights of the successive fields of the $i$'th row of the map.


## �����ʽ
The first and only line of the standard output should contain two integers separated by a single space -thenumber of ridges followed by the number of valleys for the landscape described by the map.


## ��Ŀ����
### ��Ŀ����

**���� POI 2007 Stage 2. Day 0��[Ridges and Valleys](https://szkopul.edu.pl/problemset/problem/rd6H05Dm8ME79sO3U9_f_ga_/site/?key=statement)��**

����һ�� $n \times n$ ������״��ͼ��ÿ������ $(i,j)$ ��һ���߶� $w_{ij}$��������������й������㣬�����������ڵġ�

����ɽ���ɽ�����£�
* ���ɵ�ͼ�ϵ�һ����ͨ����ɣ�
* ���з���߶ȶ���ͬ��
* ��Χ�ķ��񣨼�������ɽ���ɽ�ȵ���ɽ���ɽ�����ڵĸ��ӣ��߶Ⱦ�����ɽ�ȵĸ߶ȣ���С��ɽ��ĸ߶ȡ�

���ͼ��ɽ���ɽ�ȵ��������ر�أ����������ͼ����ĸ߶Ⱦ���ͬ����������ͼ����һ��ɽ�ȣ�Ҳ��һ��ɽ�塣

### �����ʽ

��һ��һ������ $n$ ��$2 \le n \le 1000$������ʾ��ͼ�Ĵ�С��

������ $n$ ��ÿ�� $n$ ��������ʾ��ͼ���� $i$ ���� $n$ ������ $w_{i1}, w_{i2}, \ldots, w_{in} (0 \le w_{ij} \le 1\ 000\ 000\ 000)$����ʾ��ͼ�� $i$ �и��ӵĸ߶ȡ�

### �����ʽ

���һ�������������ֱ��ʾɽ���ɽ�ȵ�������

### ��������

![](https://cdn.luogu.com.cn/upload/image_hosting/yubj6du3.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/7ct18655.png)

���������� [LibreOJ](https://loj.ac/p/2653)��

```input1
5
8 8 8 7 7
7 7 8 8 7
7 7 7 7 7
7 8 8 7 8
7 8 8 8 8
```

```output1
2 1
```

```input2
5
5 7 8 3 1
5 5 7 6 6
6 6 6 2 8
5 7 2 5 8
7 1 0 1 7
```

```output2
3 3
```

