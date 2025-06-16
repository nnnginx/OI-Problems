## ��Ŀ����
Farmer John is distributing chocolates at the barn for Valentine's day, and $B$ ($1 \le B \le 25000$) of his bulls have a special cow in mind to receive a chocolate gift.

Each of the bulls and cows is grazing alone in one of the farm's $N$ ($2\times B \le N \le 50000$) pastures conveniently numbered $1\dots N$ and connected by $M$ ($N-1 \le M \le 10^5$) bidirectional cowpaths of various lengths. Some pastures might be directly connected by more than one cowpath. Cowpath $i$ connects pastures $R_i $ and $S_i$ ($1 \le R_i \le N$; $1 \le S_i \le N$) and has length $L_i$ ($1 \le L_i \le 2000$).

Bull $i$ resides in pasture $P_i$ ($1 \le P_i \le N$) and wishes to give a chocolate to the cow in pasture $Q_i$ ($1 \le Q_i \le N$).

Help the bulls find the shortest path from their current pasture to the barn (which is located at pasture $1$) and then onward to the pasture where their special cow is grazing. The barn connects, one way or another (potentially via other cowpaths and pastures) to every pasture.

As an example, consider a farm with $6$ pastures, $6$ paths, and $3$ bulls (in pastures $2$, $3$, and $5$) who wish to bestow chocolates on their love-objects:

```cpp

                      *1  <-- Bull wants chocolates for pasture 1 cow
             [4]--3--[5]  <-- [5] is the pasture ID
            /  |
           /   |
          4    2          <-- 2 is the cowpath length
         /     |               between [3] and [4]
      [1]--1--[3]*6
     /   \    /
    9     3  2
   /       \/
 [6]      [2]*4
```
\* The Bull in pasture $2$ can travel distance $3$ (two different ways) to get to the barn then travel distance $2+1$ to pastures $[3]$ and $[4]$ to gift his chocolate. That's $6$ altogether.

\* The Bull in pasture $5$ can travel to pasture $4$ (distance $3$), then pastures $3$ and $1$ (total: $3 + 2 + 1 = 6$) to bestow his chocolate offer.

\* The Bull in pasture $3$ can travel distance $1$ to pasture $1$ and then take his chocolate $9$ more to pasture $6$, a total distance of $10$.

## �����ʽ
\* Line $1$: Three space separated integers: $N$, $M$, and $B$;

\* Lines $2\dots M+1$: Line $i+1$ describes cowpath $i$ with three space-separated integers: $R_i$, $S_i$, and $L_i$;

\* Lines $M+2\dots M+B+1$: Line $M+i+1$ contains two space separated integers: $P_i$ and $Q_i$.

## �����ʽ
\* Lines $1\dots B$: Line $i$ should contain a single integer, the smallest distance that the bull in pasture $P_i$ must travel to get chocolates from the barn and then award them to the cow of his dreams in pasture $Q_i$.

## ��Ŀ����
### ��Ŀ����

FJ �� $B$ ͷ��ţ $(1\le B\le 25000)$���� $N(2\times B\le N\le 50000)$ ��ũ������� $1$ �� $N$���� $M(N-1\le M\le 100000)$ ��˫��ߣ��� $i$ ��������ũ�� $R_i$ �� $S_i(1\le R_i\le N, 1\le S_i\le N)$���ñߵĳ����� $L_i(1\le L_i\le 2000)$����ס��ũ�� $P_i$ ����ţ A $(1\le P_i\le N)$������һ�������������ס��ũ�� $Q_i(1\le Q_i\le N)$ ����ţ B��������ţ A �����ȵ� FJ����ס�ڱ�� $1$ ��ũ��������ȡ���Ȼ�����͸���ţ B����������ǣ���ţ A ������Ҫ�߶�Զ��·�̣�

### �����ʽ
* ��һ���������� $N,M,B$��
* �� $2$ �� $M+1$ �У�ÿ�� $3$ ������ $R_i,S_i,L_i$��

* �� $M+2$ �� $M+B+1$ �У����� $B$ ��ѯ�ʣ�ÿ�� $2$ ������ $P_i ,Q_i$��

### �����ʽ
ÿ��ѯ�����һ�����������𰸡�


```input1
6 7 3 
1 2 3 
5 4 3 
3 1 1 
6 1 9 
3 4 2 
1 4 4 
3 2 2 
2 4 
5 1 
3 6 

```

```output1
6 
6 
10 

```

