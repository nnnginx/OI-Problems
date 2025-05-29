## ��Ŀ����
Farmer John has recently been experimenting with cultivating different types of grass on his farm, realizing that different types of cows like different types of grass. However, he must be careful to ensure that different types of grass are planted sufficiently far away from each-other, in order to prevent them from being inextricably mixed.


FJ's farm consists of $N$ fields ($1 \leq N \leq 200,000$), where $M$ pairs of  fields are connected by bi-directional pathways ($1 \leq M \leq 200,000$).  Using these pathways, it is possible to walk from any field to any other field. Each pathway has an integer length in the range $1 \ldots 1,000,000$. Any pair of fields will be linked by at most one direct pathway.


In each field, FJ initially plants one of $K$ types of grass ($1 \leq K \leq N$). Over time, however, he might decide to switch the grass in some field to a different type. He calls this an "update"  peration. He might perform several updates over the course of time, which are all cumulative in nature.


After each update, FJ would like to know the length of the shortest path between two fields having different grass types. That is, among all pairs of fields having different grass types, he wants to know which two are closest. Ideally,

this number is large, so he can prevent grass of one type from mixing with grass of another type. It is guaranteed that the farm will always have at least two fields with different grass types.


In 30 percent of the input cases, each field will be directly connected to at most 10 pathways.




## �����ʽ
The first line of input contains four integers, $N$, $M$, $K$, and $Q$, where $Q$ is the number of updates ($1 \leq Q \leq 200,000$).

The next $M$ lines describe the paths; each one contains three integers $A$, $B$, and $L$, indicating a path from field $A$ to field $B$ (both integers in the range $1 \ldots N$) of length $L$.

The next line indicates the initial type of grass growing in each field ($N$ integers in the range $1 \ldots K$).

Finally, the last $Q$ lines each describe an update, specified by two integers $A$ and $B$, where the grass in field $A$ is to be updated to type $B$.


## �����ʽ
For each update, print the length of the shortest path between two fields with different types of grass, after the update is applied.


## ��Ŀ����
### ��Ŀ����

Farmer John ���������ũ��������ֲ��ͬ���͵Ĳݣ����ֲ�ͬ���͵���ţϲ����ͬ���͵Ĳݡ�Ȼ����������С��ȷ����ͬ���͵Ĳ���ֲ���㹻Զ���Է�ֹ���ǲ��ɷָ�ػ����һ��

FJ ��ũ���� $N$ �������ɣ�$1 \leq N \leq 200,000$�������� $M$ �����ͨ��˫��·�����ӣ�$1 \leq M \leq 200,000$����ʹ����Щ·�������Դ��κ�����ߵ��κ�������ء�ÿ��·���ĳ�����һ���� $1 \ldots 1,000,000$ ��Χ�ڵ��������κ�һ�����֮�����ֻ��һ��ֱ��·����

��ÿ������У�FJ �����ֲ�� $K$ �ֲ��е�һ�֣�$1 \leq K \leq N$����Ȼ��������ʱ������ƣ������ܻ������ĳ����صĲݸ���Ϊ��һ�����͡��������ֲ���Ϊ�����¡������������ܻ���һ��ʱ����ִ�ж�θ��£���Щ���¶����ۻ����ʵġ�

ÿ�θ��º�FJ ��֪����ֲ��ͬ�����͵��������֮������·�����ȡ�Ҳ����˵����������ֲ��ͬ�����͵���ض��У���ϣ��֪�������������ӽ�����������£��������Ӧ�ýϴ��Ա������Է�ֹһ�����͵Ĳ�����һ�����͵Ĳݻ�ϡ���֤ũ����ʼ�����������������ֲ��ͬ�Ĳ����͡�

�� 30% �����밸���У�ÿ��������ֱ������ 10 ��·����

### �����ʽ

����ĵ�һ�а����ĸ����� $N$��$M$��$K$ �� $Q$������ $Q$ �Ǹ��µĴ�����$1 \leq Q \leq 200,000$����

�������� $M$ ������·����ÿ�а����������� $A$��$B$ �� $L$����ʾ����� $A$ ����� $B$�����߶��� $1 \ldots N$ ��Χ�ڵ��������ĳ���Ϊ $L$ ��·����

��������һ�б�ʾÿ����������ֲ�Ĳ����ͣ�$N$ �� $1 \ldots K$ ��Χ�ڵ���������

������� $Q$ ��ÿ������һ�����£����������� $A$ �� $B$ ָ������ʾ����� $A$ �Ĳݸ���Ϊ���� $B$��

### �����ʽ

����ÿ�θ��£�������º���ֲ��ͬ�����͵��������֮������·�����ȡ�

```input1
3 2 3 4
1 2 3
2 3 1
1 1 2
3 3
2 3
1 2
2 2
```

```output1
1
3
3
1
```

