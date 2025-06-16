## ��Ŀ����
Farmer John has just arranged his $N$ haybales ($1 \leq N \leq 100,000$) at various points along the one-dimensional road running across his farm.  To make sure they are spaced out appropriately, please help him answer $Q$ queries ($1 \leq Q \leq 100,000$), each asking for the number of haybales within a specific interval along the road.

## �����ʽ
The first line contains $N$ and $Q$.

The next line contains $N$ distinct integers, each in the range $0 \ldots 1,000,000,000$, indicating that there is a haybale at each of those locations.

Each of the next $Q$ lines contains two integers $A$ and $B$($0 \leq A \leq B \leq 1,000,000,000$) giving a query for the number of haybales between $A$ and $B$, inclusive.

## �����ʽ
You should write $Q$ lines of output.  For each query, output the number of haybales in its respective interval.

## ��Ŀ����
### ��Ŀ����

Farmer John �ոս����� $N$ ���ɲ�����$1 \leq N \leq 100,000$����������ũ����һά��·�ϵĸ���λ�á�Ϊ��ȷ������֮��ļ����ʣ���������ش� $Q$ ����ѯ��$1 \leq Q \leq 100,000$����ÿ����ѯѯ���ڵ�·���ض��������ж��ٸ��ɲ�����

### �����ʽ

��һ�а��� $N$ �� $Q$��

�ڶ��а��� $N$ ����ͬ��������ÿ�������ķ�Χ�� $0 \ldots 1,000,000,000$ ֮�䣬��ʾÿ��λ������һ���ɲ�����

�������� $Q$ ��ÿ�а����������� $A$ �� $B$��$0 \leq A \leq B \leq 1,000,000,000$������ʾһ����ѯ��ѯ���� $A$ �� $B$������ $A$ �� $B$�����������ж��ٸ��ɲ�����

### �����ʽ

����Ҫ��� $Q$ �С�����ÿ����ѯ��������Ӧ�����ڵĸɲ���������

```input1
4 6
3 2 7 5
2 3
2 4
2 5
2 7
4 6
8 10
```

```output1
2
2
3
4
1
0
```

