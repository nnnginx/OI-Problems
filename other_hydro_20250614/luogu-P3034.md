## ��Ŀ����
The cows are in a particularly mischievous mood today!  All Farmer John wants to do is take a photograph of the cows standing in a line, but they keep moving right before he has a chance to snap the picture.

Specifically, each of FJ's N (1 <= N <= 20,000) cows has a unique integer ID number.  FJ wants to take a picture of the cows standing in a line in a very specific ordering, represented by the contents of an array A[1...N], where A[j] gives the ID number of the jth cow in the ordering.  He arranges the cows in this order, but just before he can press the button on his camera to snap the picture, a group of zero or more cows (not necessarily a contiguous group) moves to a set of new positions in the lineup.  More precisely, a group of zero or more cows steps away from the line, with the remaining cows shifting over to close the resulting gaps in the lineup.  The cows who stepped away then re-insert themselves at different positions in the lineup (not necessarily at the locations they originally occupied).  Frustrated but not deterred, FJ again arranges his cows according to the ordering in A, but again, right before he can snap a picture, a different group of zero or more cows moves to a set of new positions in the lineup.

The process above repeats for a total of five photographs before FJ gives up.  Given the contents of each photograph, see if you can reconstruct the original intended ordering A.  Each photograph shows an ordering of the cows that differs from A in that some group of zero or more cows has moved. However, a cow only moves in at most one photograph: if a cow is part of the group that moves in one photograph, she will not actively move in any of the other four photographs (although she could end up at a different index as a consequence of other cows around her moving, of course).

Farmer John��Ȼ����������Ƭ��ÿ�ű�ʾ��ʼ��ţλ�õ��ƶ����״̬��Ȼ�����FJ����ͷţ��ʼ�������ӡ�


## �����ʽ
\* Line 1: The number of cows, N (1 <= N <= 20,000). 

\* Lines 2..5N+1: The next 5N lines describe five orderings, each one a block of N contiguous lines.  Each line contains the ID of a cow, an integer in the range 0...1,000,000,000.


## �����ʽ
\* Lines 1..N: The intended ordering A, one ID per line. 



## ��Ŀ����
## ��Ŀ����

�������ţ���ر��Ƥ��Farmer John ������ֻ�Ǹ��ų�һ�ŵ���ţ���գ���������������Ƭ֮ǰ����ţ��һֱ���ƶ���

�����˵��FJ �� $N$ ͷ��ţ��$1 \leq N \leq 20\,000$����ÿͷ��ţ����һ��Ψһȷ���ı�š�FJ ��Ҫ��һ���ض���˳������һ����ţ�ų�һ�ŵ���Ƭ�����˳�������� $A[1 \ldots N]$ ��ʾ������ $A[i]$ �������� $i$ λ�õ���ţ�ı�š�

������������˳����ţ�����кã����������¿���֮ǰ����Щ��ţ����������ͷ�������ͷ��ţ��λ��Ҳ��һ�����������Ƶ�һ���µ�λ�á���׼ȷ��˵��һЩ��ţ�뿪���У�ʣ�µ���ţ��£����Щ�뿪����ţ�ٽ��Լ����²��뵽�����е�����λ�ã���һ��������֮ǰ��λ�ã���FJ �е��ǳ���ɥ�����ٴΰ��� $A$ �����˳�����°����˶��С��������ٴΰ��¿���֮ǰ������һЩ��ţ�ƶ������µ�λ�á�

��������FJ ����������Ƭ������ÿ����Ƭ��������ݣ��� FJ ���¿���ʱ��ţ��˳�򣩣����㳢������� FJ ���Ϊ��ţ���ŵ�˳�򣨼� $A$ ���飩�����ڿ�������ţ�ƶ�����Ƭ��ʾ��˳����ԭ����˳�����������ͬ�����ǣ�һͷ��ţ���ֻ���ƶ�һ�Σ������һͷ��ţ��������һ����Ƭʱ�ƶ��ˣ�����������������Ƭ��ʱ�򶼲����ƶ�����Ȼ������������ţҲ���ƶ������ڲ�ͬ��Ƭ�е�˳�򲢲�һ����ͬ��

## �����ʽ

��һ�а���һ������ $N$��

������ $5N$ �У�ÿ $N$ ��������һ����Ƭ�и���ţ��˳��ÿ�а���һ����ţ�ı�ţ���֤���б�Ŷ��ǲ����� $1\,000\,000\,000$ �ķǸ�������

## �����ʽ

��� $N$ �У�ÿ��һ������ $A[i]$���� FJ ���Ϊ��ţ�źõ�˳��

## ��������

FJ �ĵ�������Ƭ�ֱ�Ϊ��

- `10 20 30 40 50`
- `20 10 30 40 50`
- `30 10 20 40 50`
- `40 10 20 30 50`
- `50 10 20 30 40`

```input1
5 
10 
20 
30 
40 
50 
20 
10 
30 
40 
50 
30 
10 
20 
40 
50 
40 
10 
20 
30 
50 
50 
10 
20 
30 
40 

```

```output1
10 
20 
30 
40 
50 

```

## ��ʾ
There are 5 cows, with IDs 10, 20, 30, 40, and 50.  In each of the 5 photos, a different cow moves to the front of the line (at most one cow moves in each photo here, but it is possible in other inputs that multiple cows could move in a particular photo).


The correct original ordering A[1..5] is 10, 20, 30, 40, 50.



