## ��Ŀ����
Farmer John is conducting research for a new milk contract in a new territory. He intends to distribute milk to T (1 <= T <= 25,000) towns conveniently numbered 1..T which are connected by up to R (1 <= R <= 50,000) roads conveniently numbered 1..R and/or P (1 <= P <= 50,000) airplane flights conveniently numbered 1..P.

Either road i or plane i connects town A\_i (1 <= A\_i <= T) to town B\_i (1 <= B\_i <= T) with traversal cost C\_i. For roads, 0 <= C\_i <= 10,000; however, due to the strange finances of the airlines, the cost for planes can be quite negative (-10,000 <= C\_i <= 10,000).

Roads are bidirectional and can be traversed from A\_i to B\_i or B\_i to A\_i for the same cost; the cost of a road must be non-negative.

Planes, however, can only be used in the direction from A\_i to B\_i specified in the input. In fact, if there is a plane from A\_i to B\_i it is guaranteed that there is no way to return from B\_i to A\_i with any sequence of roads and planes due to recent antiterror regulation.

Farmer John is known around the world as the source of the world's finest dairy cows. He has in fact received orders for his cows from every single town. He therefore wants to find the cheapest price for delivery to each town from his distribution center in town S (1 <= S <= T) or to know that it is not possible if this is the case.

MEMORY LIMIT: 64MB

## �����ʽ
\* Line 1: Four space separated integers: T, R, P, and S

\* Lines 2..R+1: Three space separated integers describing a road: A\_i, B\_i and C\_i

\* Lines R+2..R+P+1: Three space separated integers describing a plane: A\_i, B\_i and C\_i


## �����ʽ
\* Lines 1..T: The minimum cost to get from town S to town i, or 'NO PATH' if this is not possible


## ��Ŀ����
### ��������

Farmer John ����һ���µ��������������ţ�����۷������е��顣�����ţ���͵� $T$ ������ ( $1 \le T \le 25,000$ )�����Ϊ $1$ �� $T$ ����Щ����֮��ͨ�� $R$ ����· ( $1 \le R \le 50,000$ �����Ϊ $1$ �� $R$ ) �� $P$ ������ ( $1 \le P \le 50,000$ �����Ϊ $1$ �� $P$ ) ���ӡ�ÿ����· $i$ ���ߺ��� $i$ ���ӳ��� $A_i$ ( $1 \le A_i \le T$ )�� $B_i$ ( $1 \le B_i \le T$ )������Ϊ $C_i$ ��

���ڵ�· $0 \le C_i \le 10,000$ ;Ȼ�����ߵĻ��Ѻ����棬���� $C_i$ �����Ǹ���( $-10,000 \le C_i \le 10,000$ )����·��˫��ģ����Դ� $A_i$ �� $B_i$��Ҳ���Դ� $B_i$ �� $A_i$ �����Ѷ��� $C_i$ ��Ȼ��������֮��ͬ��ֻ���Դ� $A_i$ �� $B_i$ ��

��ʵ�ϣ���������ֲ�����̫���ţ�Ϊ������г����̨ ��һЩ���߱�֤�������һ�����߿��Դ� $A_i$ ��  $B_i$����ô��֤������ͨ��һЩ��·�ͺ��ߴ� $B_i$ �ص� $A_i$ ������ $FJ$ ����ţ���繫��ʮ�ָ���������Ҫ������ţ��ÿһ�����������ҵ��ӷ������ĳ��� $S$ ( $1 \le S \le T$) ����ţ�͵�ÿ�����������˵ķ���������֪�����ǲ����ܵġ�

### �����ʽ

�� $R+P+1$ ��

�� $1$ �У��ĸ����� $T$ , $R$ , $P$ �� $S$ ���ֱ��ʾ�������������·�����������ߵ����������ĳ���

�� $2$ �� $R+1$ �У�ÿ���������� $A_i$ , $B_i$ �� $C_i$ ������һ����·��

�� $R+2$ �� $R+P+1$ �У�ÿ���������� $A_i$ , $B_i$ �� $C_i$ ������һ�����ߡ�

### �����ʽ

�� $T$ �У��� $i$ ��������� $S$ ������ $i$ ����С���ѡ�������ܵ�����`NO PATH`

```input1
6 3 3 4 
1 2 5 
3 4 5 
5 6 10 
3 5 -100 
4 6 -100 
1 3 -10 

```

```output1
NO PATH 
NO PATH 
5 
0 
-95 
-100 

```

## ��ʾ
6 towns.  There are roads between town 1 and town 2, town 3 and town 4, and town 5 and town 6 with costs 5, 5 and 10; there are planes from town 3 to town 5, from town 4 to town 6, and from town 1 to town 3 with costs -100, - 100 and -10.  FJ is based in town 4.


FJ's cows begin at town 4, and can get to town 3 on the road.  They can get to towns 5 and 6 using planes from towns 3 and 4.  However, there is no way to get to towns 1 and 2, since they cannot go

backwards on the plane from 1 to 3.


