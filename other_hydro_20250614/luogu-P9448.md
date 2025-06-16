## ��Ŀ����
A splitstream system is an acyclic network of nodes that processes finite sequences of numbers. There are two types of nodes (illustrated in Figure J.1):

- A *split* node takes a sequence of numbers as input and distributes them alternatingly to its two outputs. The first number goes to output $1$, the second to output $2$, the third to output $1$, the fourth to output $2$, and so on, in this order.</li>
- A *merge** node takes two sequences of numbers as input and merges them alternatingly to form its single output. The output contains the first number from input $1$, then the first from input $2$, then the second from input $1$, then the second from input $2$, and so on. If one of the input sequences is shorter than the other, then the remaining numbers from the longer sequence are simply transmitted without being merged after the shorter sequence has been exhausted.</li>

 ![](https://cdn.luogu.com.cn/upload/image_hosting/e0gr6wa3.png)
  
  Figure J.1: Illustration of how split and merge nodes work.
  
The overall network has one input, which is the sequence of positive integers $1, 2, 3, \ldots, m$. Any output of any node can be queried. A query will seek to identify the $k^{th}$ number in the sequence of numbers for a given output and a given $k$. Your task is to implement such queries efficiently.

## �����ʽ
The first line of input contains three integers $m$, $n$, and $q$, where $m$ ($1 \leq m \leq 10^9$) is the length of the input sequence, $n$ ($1 \leq n \leq 10^4$) is the number of nodes, and $q$ ($1 \leq q \leq 10^3$) is the number of queries.

The next $n$ lines describe the network, one node per line. A split node has the format $\texttt{S} \ x \ y \ z$, where $x$, $y$ and $z$ identify its input, first output and second output, respectively. A merge node has the format $\texttt{M} \ x \ y \ z$, where $x$, $y$ and $z$ identify its first input, second input and output, respectively. Identifiers $x$, $y$ and $z$ are distinct positive integers. The overall input is identified by $1$, and the remaining input/output identifiers form a consecutive sequence beginning at $2$. Every input identifier except $1$ appears as exactly one output. Every output identifier appears as the input of at most one node.

Each of the next $q$ lines describes a query. Each query consists of two integers $x$ and $k$, where $x$ ($2 \leq x \leq 10^5$) is a valid output identifier and $k$ ($1 \leq k \leq 10^9$) is the index of the desired number in that sequence. Indexing in a sequence starts with $1$.

## �����ʽ
For each query $x$ and $k$ output one line with the $k^{th}$ number in the output sequence identified by $x$, or $\texttt{none}$ if there is no element with that index number.

## ��Ŀ����
### ����
��һ���� $n$ ���ڵ�Ĵ����������е����磬���������ֽڵ㣺��ֽڵ�ͺϲ��ڵ㡣��ֽڵ�Ὣ���������е����ֽ������������������У��ϲ��ڵ�ύ�潫�������������е����ֲ�����������С����磺

$\{1,2,3,4,5\}$ ��ֵ� $\{1,3,5\}$ �� $\{2,4\}$��

$\{2,4\}$ �� $\{1,3,5\}$ �ϲ��� $\{2,1,4,3,5\}$��

�������У��� $1$ ����ÿһ������ÿһ������˶���������һ���ڵ�������,$1$ �Žڵ�������Ϊ������ˣ�ÿһ������˲�һ����������һ���ڵ������ˡ�ÿһ������˶����Ŵ� $2$ ��ʼ����������š�

��һ���������� $\{1,2,\cdots,m\}$ �� $1$ �Žڵ��������������磬����Ҫ������Ϊ  $x$ �����������������еĵ� $k$ �����֡�

### �����ʽ
��һ���������� $n,m,q$���ֱ��ʾ���ĸ�������������Ϊ $\{1,2,\cdots,m\}$����ѯ�Ĵ�����

������ $n$ �У�ÿ��һ����ĸ��ͷ���������������� $x,y,z$������ĸΪ $S$�����ʾ����һ����ֽڵ㣬$x$ ����������������ӵ�����˱�ţ�$y,z$ ��������������˵ı�ţ�����ĸΪ $M$�����ʾ����һ���ϲ��ڵ㣬$x,y$ ��������������������ӵ�����˵ı�ţ�$z$ ����������˱�š�

�ٽ����� $q$ �У�ÿ���������� $x,k$��������������������

### �����ʽ
����ÿһ��ѯ�ʣ�������Ӧ�Ļش����𰸲����ڣ���� `none`��

```input1
200 2 2
S 1 2 3
M 3 2 4
4 99
4 100

```

```output1
100
99

```

```input2
100 3 6
S 1 4 2
S 2 3 5
M 3 4 6
6 48
6 49
6 50
6 51
6 52
5 25

```

```output2
47
98
49
51
53
100

```

```input3
2 3 3
S 1 2 3
S 3 4 5
M 5 2 6
3 1
5 1
6 2

```

```output3
2
none
none

```

