## ��Ŀ����
��ԭ����ȣ�$N$ �����ݷ�Χ����Ϊ�� $1\leq N\leq 100000$���������ݷ�Χ���ޱ仯��

## ��Ŀ����
Farmer John has constructed an obstacle course for the cow's enjoyment. The course consists of a sequence of $N$ fences ($1\le N \le 100000$) of varying lengths, each parallel to the x axis. Fence i's y coordinate is i.

The door to FJ's barn is at the origin (marked '`*`' below). The starting point of the course lies at coordinate ($S$,$N$).

```
   +--S--+-+-+
+--+--+--+
    ...
   +--+--+-+
      +--+-+-+
|==|==|==*=|=|=|
-3 -2 -1 0 1 2 3
```

FJ's original intention was for the cows to jump over the fences, but cows are much more comfortable keeping all four hooves on the ground. Thus, they will walk along the fence and, when the fence ends, they will turn towards the x axis and continue walking in a straight line until the hit another fence segment or the side of the barn. Then they decide to go left or right until they reach the end of the fence segment, and so on, until they finally reach the side of the barn and then, potentially after a short walk, the ending point.

Naturally, the cows want to walk as little as possible. Find the minimum distance the cows have to travel back and forth to get from the starting point to the door of the barn.


## �����ʽ
- Line 1: Two space-separated integers: $N$ and $S$. ($-100000\le S \le 100000$)
- Line 2~N+1: Each line contains two space-separated integers : $A_i$ and $B_i$ ($-100000\le A_i < B_i \le 100000 $) , the starting and ending x-coordinates of fence segment i. Line 2 describes fence #2; line 3 describes fence #2; and so on. The starting position will satisfy $A_N \le S \le B_N$. Note that the fences will be traversed in reverse order of the input sequence.


## �����ʽ
- Line 1: The minimum distance back and forth in the x direction required to get from the starting point to the ending point by walking around the fences. The distance in the y direction is not counted, since it is always precisely $N$.


## ��Ŀ����
### ���ⷭ��

FJ �� $N $ ��դ������������ϵ�ϣ��� $i$ ��դ��Ϊ $(A_i,i)$ �� $(B_i,i)$ ��һ���߶Σ��˵㴦����ͨ����������ĳֻţ�� $(S,N)$ �����������������ƶ����̣�����Ŀǰλ��Ϊ $(x,y)$����

- ��� $(x,y)$ ��û��դ������ô������ֱ������դ��Ϊֹ��
- ����������ˣ���ô������������ߵ� $(A_y,y)$ ���� $(B_y,y)$ Ϊֹ��
- ����Ѿ��ߵ��� $x$ ���ϣ���ô���� $x$ ���ߵ�ԭ�㡣

��ţ�ƶ���ԭ������Ҫ�� $x$ �᷽�����ƶ�����С���롣

�����һ�и��� $N$ �� $S$����� $N$ �и��� $A_i$ �� $B_i$��

ʾ��ͼΪ�����������޸ģ�ÿ���� `+` �м���һ��λ���롣

```input1
4 0
-2 1
-1 2
-3 0
-2 1
```

```output1
4
```

