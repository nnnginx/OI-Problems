## ��Ŀ����

Bessie and her sister Elsie graze in different fields during the day, and in the evening they both want to walk back to the barn to rest. Being clever bovines, they come up with a plan to minimize the total amount of energy they both spend while walking. Bessie spends $B$ units of energy when walking from a field to an adjacent field, and Elsie spends $E$ units of energy when she walks to an adjacent field. However, if Bessie and Elsie are together in the same field, Bessie can carry Elsie on her shoulders and both can move to an adjacent field while spending only $P$ units of energy (where $P$ might be considerably less than $B+E$, the amount Bessie and Elsie would have spent individually walking to the adjacent field). If $P$ is very small, the most energy-efficient solution may involve Bessie and Elsie traveling to a common meeting field, then traveling together piggyback for the rest of the journey to the barn. Of course, if $P$ is large, it may still make the most sense for Bessie and Elsie to travel separately. On a side note, Bessie and Elsie are both unhappy with the term "piggyback", as they don't see why the pigs on the farm should deserve all the credit for this remarkable form of transportation. Given $B,E$, and $P$, as well as the layout of the farm, please compute the minimum amount of energy required for Bessie and Elsie to reach the barn.

**���룺**

����һ�� $n$ ���� $m$ ���ߵ�����ͼ������ Bessie �� $1$ �ŵ㣬Elsie �� $2$ �ŵ㣬���ǵ�Ŀ�ĵ�Ϊ $n$ �ŵ㡣Bessie ÿ����һ������Ҫ���� $B$ ��������Elsie ÿ����һ������Ҫ���� $E$ ������������������ʱ�����ǿ���һ�����ߣ���ʱ����ÿ����һ������Ҫ���� $P$ ���������������������� $n$ �ŵ�ʱ�������Ķ���������

## �����ʽ

The first line of input contains the positive integers $B,E,P,n$,and $m$.$B$,$E$, and $P$ are described above. $n$ is the number of fields in the farm (numbered $1\dots n$), and $m$ is the number of connections between fields. Bessie and Elsie start in fields $1$ and $2$, respectively. The barn resides in field $n$. The next $m$ lines in the input each describe a connection between a pair of different fields, specified by the integer indices of the two fields. Connections are bi-directional. It is always possible to travel from field $1$ to field $n$, and field $2$ to field $n$, along a series of such connections. 

## �����ʽ

A single integer specifying the minimum amount of energy Bessie and Elsie collectively need to spend to reach the barn.

```input1
4 4 5 8 8
1 4
2 3
3 4
4 7
2 5
5 6
6 8
7 8
```

```output1
22
```

## ����˵��

In the example shown here, Bessie travels from $1$ to $4$ and Elsie travels from $2$ to $3$ to $4$. Then, they travel together from $4$ to $7$ to $8$.

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\le B,E,P,m\le 4\times 10^4$��$3\le n \le 10^4$��

## ��Ŀ��Դ

Silver