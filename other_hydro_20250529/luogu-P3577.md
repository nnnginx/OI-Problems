## ��Ŀ����
King Byteasar believes that Byteotia, a land full of beautiful sights, should attract lots of tourists,    who should spend lots of money, which should eventually find their way to the royal treasury.

But reality does not live up to his dream.

So the king instructed his councilor to look into this issue.

The councilor found out that foreigners keep away from Byteotia due to its sparse road network.

Let us remark that there are $n$ towns in Byteotia, connected by $m$ two way roads, each road linking two different towns.

The roads may lead through picturesque overflies and somewhat less picturesque tunnels.

There is no guarantee that every town can be reached from every other town.

The councilor observed that the current road network does not allow for a long journey.

Namely, wherever one starts the journey, it is impossible to visit more than 10 towns without passing through some town twice.

Due to limited funds in the treasury, no new roads will be constructed at the time.

Instead, Byteasar has decided to build a network of tourist information points (TIPs),    staffed by officers who are to advertise the short trips that are available.

For each town, there should be a TIP either in this town or one of the towns directly    linked by a road.

Moreover, the cost of building the TIP is known for each town.

Help the king by finding the cheapest way of building TIPs that will satisfy aforementioned condition.



## �����ʽ
The first line of the standard input contains two integers $n$, $m$ ($2\le n\le 20\ 000$ ,$0\le m\le 25\ 000$), separated by a single space,    that specify the number of towns and roads in Byteotia respectively.

The towns are numbered from $1$ to $n$.

The second line of input contains $n$ integers $c_1,c_2,\cdots,c_n$ ($0\le c_i\le 10\ 000$),    separated by single spaces; the number $c_i$ specifies the cost of building a TIP in the town no. $i$.

Then, a description of the Byteotian road network follows. The $i$-th of the following $m$ lines contains two integers $a_i$,$b_i$ ($1\le a_i<b_i\le n$), separated by a single space, that indicate that the towns no. $a_i$ and $b_i$ are linked by a road. There is at most one (direct) road between any pair of towns.


## �����ʽ
Your program should print out one integer to the standard output: the total cost of building all the TIPs.

 ![](https://cdn.luogu.com.cn/upload/pic/6974.png) 



## ��Ŀ����

����һ�� $n$ ���㣬$m$ ���ߵ�����ͼ���������ڵ� $i$ ���㽨������վ��ķ���Ϊ $C_i$��������ͼ�У���������䲻���ڽڵ������� $10$ �ļ�·�������ҵ�һ�ַ�����С�Ľ�������վ��ķ�����ʹ��ÿ����Ҫô����������վ�㣬Ҫô�����б�ֱ�������ĵ���������һ���㽨��������վ�㡣

```input1
6 6
3 8 5 6 2 2
1 2
2 3
1 3
3 4
4 5
4 6

```

```output1
7

```

