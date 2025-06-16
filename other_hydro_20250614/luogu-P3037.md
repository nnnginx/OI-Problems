## ��Ŀ����
Farmer John has been taking an evening algorithms course at his local university, and he has just learned about minimum spanning trees.  However, Farmer John now realizes that the design of his farm is not as efficient as it could be, and he wants to simplify the layout of his farm.

The farm is currently arranged like a graph, with vertices representing fields and edges representing pathways between these fields, each having an associated length.  Farmer John notes that for each distinct length, at most three pathways on his farm share this length.  FJ would like to remove some of the pathways on his farm so that it becomes a tree -- that is, so that there is one unique route between any pair of fields.  Moreover, Farmer John would like this to be a minimum spanning tree -- a tree having the smallest possible sum of edge lengths.

Help Farmer John compute not only the sum of edge lengths in a minimum spanning tree derived from his farm graph, but also the number of different possible minimum spanning trees he can create.

ũ��Լ����һ��ҹУѧϰ�㷨�γ̣����ո�ѧ������С������������Լ����ʶ������ũ����Ƶò�����Ч�������ũ���Ĳ��֡�


Լ����ũ�����Կ���һ��ͼ��ũ�����ͼ�ж��㣬���С·����ͼ�еıߣ�ÿ������һ���ĳ��ȡ�Լ��ע�⵽��ũ�������������С·������ͬ�ĳ��ȡ�Լ����ɾ��һЩС·ʹ��ũ����Ϊһ������ʹ������ũ���ֻ��һ��·��������Լ�����ũ����Ƴ���С��������Ҳ����ũ����·���ܳ�����̡�


�����Լ���ҳ���С���������ܳ��ȣ�ͬʱ�������ܹ��ж�������С��������


## �����ʽ
\* Line 1: Two integers N and M (1 <= N <= 40,000; 1 <= M <= 100,000), representing  the number of vertices and edges in the farm graph, respectively.  Vertices are numbered as 1..N.

\* Lines 2..M+1: Three integers a\_i, b\_i and n\_i (1 <= a\_i, b\_i <= N; 1 <= n\_i <= 1,000,000)  representing an edge from vertex a\_i to b\_i with length n\_i.  No edge length n\_i will occur more than three times.


## �����ʽ
\* Line 1: Two integers representing the length of the minimal spanning tree and the number of minimal spanning trees (mod

1,000,000,007).


```input1
4 5 
1 2 1 
3 4 1 
1 3 2 
1 4 2 
2 3 2 

```

```output1
4 3 

```

## ��ʾ
Picking both edges with length 1 and any edge with length 2 yields a minimum spanning tree of length 4.



