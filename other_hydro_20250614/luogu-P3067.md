## ��Ŀ����
Farmer John's owns N cows (2 <= N <= 20), where cow i produces M(i) units of milk each day (1 <= M(i) <= 100,000,000).  FJ wants to streamline the process of milking his cows every day, so he installs a brand new milking machine in his barn.  Unfortunately, the machine turns out to be far too sensitive: it only works properly if the cows on the left side of the barn have the exact same total milk output as the cows on the right side of the barn!

Let us call a subset of cows "balanced" if it can be partitioned into two groups having equal milk output.  Since only a balanced subset of cows can make the milking machine work, FJ wonders how many subsets of his N cows are balanced.  Please help him compute this quantity.


## �����ʽ
\* Line 1: The integer N.

\* Lines 2..1+N: Line i+1 contains M(i). 



## �����ʽ
\* Line 1: The number of balanced subsets of cows.


## ��Ŀ����
���Ƕ���һ����ţ���� $S$ ��ƽ��ģ����ҽ���������������������

- $S$ �ǿա�
- $S$ ���Ա�**����**���������� $A,B$������ $A$ �����ţ������֮�͵��� $B$ �����ţ������֮�͡����ֵĺ����ǣ�$A\cup B=S$ �� $A\cap B=\varnothing$��

���ڸ�����СΪ $n$ ����ţ���� $S$��ѯ�����ж��ٸ��Ӽ���ƽ��ġ���ע�⣬��ţ֮���ǻ�����ͬ�ģ��������ǵĲ��������ܳ�����ͬ��

### �����ʽ

��һ��һ������ $n$����ʾ��ţ����Ŀ��

�� $2$ �� $n+1$ �У�ÿ��һ���� $a_i$����ʾÿͷ��ţ�Ĳ�������

### �����ʽ

���һ������ʾ����������

### ��������

���������ַ��������� $\{1,2,3\}$ ���Ի���Ϊ $\{1,2\}$ �� $\{3\}$������ $\{1,3,4\}$ ���Ի���Ϊ $\{1,3\}$ �� $\{4\}$������ $\{1,2,3,4\}$ ���Ի���Ϊ $\{1,4\}$ �� $\{2,3\}$���� $3$ ���Ӽ���

### ���ݷ�Χ��Լ��

����ȫ�����ݣ���֤ $1\le n\le 20$��$1\le a_i\le 10^8$��

```input1
4 
1 
2 
3 
4 

```

```output1
3 

```

## ��ʾ
There are 4 cows, with milk outputs 1, 2, 3, and 4.


There are three balanced subsets: the subset {1,2,3}, which can be partitioned into {1,2} and {3}, the subset {1,3,4}, which can be partitioned into {1,3} and {4}, and the subset {1,2,3,4} which can be partitioned into {1,4} and {2,3}.


