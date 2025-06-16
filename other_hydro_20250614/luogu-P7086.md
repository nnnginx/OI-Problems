## ��Ŀ����


A group of biologists is trying to find a cure for a viral disease. They have tried many antibodies of various origins that could potentially fight the viral antigens, and have selected $n$ antibodies that seem to work best during experiments.

Each antibody is identified by its heavy chain -- a sequence of amino acids.

The set of antibodies form a similarity cluster, if at least one of the following holds:

k-prefixes (first $k$ amino acids) of all their heavy chains are equal;

k-suffixes (last $k$ amino acids) of all their heavy chains are equal.

In order to simplify the future research, biologists want to group antibodies to similarity clusters.

You need to split the given antibodies to a minimum number of similarity clusters.



## �����ʽ


The first line contains two integers $n$ and $k$ -- the number of heavy chains and the length of sequence of amino acids to coincide $(1 \le n \le 5 000 , 1 \le k \le 550)$ .

The following $n$ lines contain sequences of amino acids that form heavy chains of antibodies. Each amino acid described with an uppercase English letter. Each heavy chain contains at least $k$ and no more than $550$ amino acids.



## �����ʽ


The first line of output must contain a single integer -- the minimum number of similarity clusters. The following lines must contain descriptions of clusters, one per line.

Each description starts with $m_i$ -- the number of antibodies in the cluster and is followed by $m_i$ integers -- numbers of these antibodies. Antibodies are numbered in the order of appearance in the input starting from one.

Each antibody must be present in exactly one cluster.



## ��Ŀ����
����$n$�������أ�ÿһ�������ض�����ͨ������һ�����������б����ϡ�

�����һ�鿹����������������һ����������Щ�����زſ����γ�һ��������Ⱥ�塱��

1. �������п����صİ��������е�ǰ$k$��������Ԫ����ɵ�����ȫ����ͬ

2. �������п����صİ��������еĺ�$k$��������Ԫ����ɵ�����ȫ����ͬ

�ر�ģ�һ�ֿ����ؿ��Գ�Ϊһ������Ⱥ�塣

Ϊ�˼򻯺����о�������ѧ������Ҫ�������ط��࣬ʹ����$n$�������ر��ֳ����ɸ�����Ⱥ�塣����Ҫ�ҳ�һ�ַ�����ʹ�÷���������Ⱥ���������١�

------

��һ�а���������������$n$��$k$��������������������$1��n��5000��1��k��550$��

��������$n$�У�ÿ�а���һ�����������С����������б�����Ϊ�ɴ�дӢ����ĸ��ɵ��ַ�����ÿ�����а���������$k$����������$550$��Ӣ���ַ���ÿ��Ӣ���ַ�����һ�ֲ�ͬ�İ����ᡣ

------

��һ�а���һ��������$ans$����ʾ���ֳɵ�����Ⱥ����С���ܵ���Ŀ��

��������$ans$�У�ÿ�е�һ����Ϊ$m_i$����ʾ��$i$������Ⱥ����$m_i$��Ԫ�ء���������$m_i$��������$j$������ʾ�������Ⱥ����������еĵ�$j$�������ء�����Ŵ�$1$��ʼ����

ÿһ�������ر���ǡ�ó���һ�Ρ�

```input1
4 1
AA
AB
BB
BA

```

```output1
2
2 1 2
2 3 4

```

```input2
3 2
ABA
BAB
XY

```

```output2
3
1 1
1 2
1 3

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



