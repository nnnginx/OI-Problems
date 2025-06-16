## ��Ŀ����
Farmer John has hired a professional photographer to take a picture of some of his cows.  Since FJ's cows represent a variety of different breeds, he would like the photo to contain at least one cow from each distinct breed present in his herd.

FJ's N cows are all standing at various positions along a line, each described by an integer position (i.e., its x coordinate) as well as an integer breed ID.  FJ plans to take a photograph of a contiguous range of cows along the line.  The cost of this photograph is equal its size -- that is, the difference between the maximum and minimum x coordinates of the cows in the range of the photograph.

Please help FJ by computing the minimum cost of a photograph in which there is at least one cow of each distinct breed appearing in FJ's herd.


## �����ʽ
\* Line 1: The number of cows, N (1 <= N <= 50,000). 

\* Lines 2..1+N: Each line contains two space-separated positive integers specifying the x coordinate and breed ID of a single cow.  Both numbers are at most 1 billion.


## �����ʽ
\* Line 1: The smallest cost of a photograph containing each distinct breed ID.


## ��Ŀ����
### ��������

ũ��Լ����һ��רҵ��Ӱʦ�����Ĳ���ţ���ա�����Լ����ţ�кö�Ʒ�֣���ϲ��������Ƭ����ÿ��Ʒ�ֵ�����һͷţ��

Լ����ţ��վ��һ�����ߵĲ�ͬ�ط��� ÿһͷţ��һ������λ�� $X_i$ �Լ�����Ʒ�ֱ�� $ID_i$ ��ʾ��

Լ������һ����Ƭ������Ƭ�����ߵ���ţ��������Χ��ɡ���Ƭ�ĳɱ����ģ�൱�������ζ�ţ���һϵ����Ƭ�е�������С $X$ ����Ĳ���������Ƭ�ĳɱ���

�����Լ��������С����Ƭ�ɱ�����Щ��Ƭ����ÿ����ͬ��Ʒ�ֵ�����һͷţ��û����ͷţԸ��վ��ͬһ���ص�ġ�


### �����ʽ 


�� $1$ �У�ţ������ $N$��


�� $2..1+N$ �У�ÿ�а��� 2 ���Կո�ָ��������� $X_i$ �� $ID_i$����������Ŀ������


### �����ʽ 


�����һ�У�����ÿ����ͬƷ�� $\rm ID$ ����Ƭ����ͳɱ���

```input1
6 
25 7 
26 1 
15 1 
22 3 
20 1 
30 1 

```

```output1
4 

```

## ��ʾ
There are 6 cows, at positions 25,26,15,22,20,30, with respective breed IDs 7,1,1,3,1,1.


The range from x=22 up through x=26 (of total size 4) contains each of the distinct breed IDs 1, 3, and 7 represented in FJ's herd.


