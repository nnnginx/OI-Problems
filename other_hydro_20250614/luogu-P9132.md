## ��Ŀ����
**Note: The time limit for this problem is 3s, 1.5x the default.**

Bessie likes to watch shows on Cowflix, and she watches them in different places. Farmer John's farm can be represented as a tree with $N(2 \le N \le 2 \cdot 10^5)$ nodes, and for each node, either Bessie watches Cowflix there or she doesn't. It is guaranteed that Bessie watches Cowflix in at least one node.

Unfortunately, Cowflix is introducing a new subscription model to combat password sharing. In their new model, you can choose a connected component of size $d$ in the farm, and then you need to pay $d+k$ moonies for an account that you can use in that connected component. Formally, you need to choose a set of disjoint connected components $c_1,c_2, \cdots ,c_C$ so that every node where Bessie watches Cowflix must be contained within some $c_i$. The cost of the set of components is $\sum\limits^{C}_{i=1}(|c_i|+k)$, where $|c_i|$ is the number of nodes in component $c_i$. Nodes where Bessie does not watch Cowflix do not have to be in any $c_i$.

Bessie is worried that the new subscription model may be too expensive for her given all the places she visits and is thinking of switching to Mooloo. To aid her decision-making, calculate the minimum amount she would need to pay to Cowflix to maintain her viewing habits. Because Cowflix has not announced the value of $k$, calculate it for all integer values of $k$ from $1$ to $N$. 

## �����ʽ
The first line contains $N$.

The second line contains a bit string $s_1s_2s_3\cdots s_N$ where $s_i=1$ if Bessie watches Cowflix at node $i$.

Then $N - 1$ lines follow, each containing two integers $a$ and $b (1 \le a,b \le N)$, which denotes an edge between $a$ and $b$ in the tree.

## �����ʽ
The answers for each $k$ from $1$ to $N$ on separate lines. 

## ��Ŀ����
Bessie ϲ���� Cowflix �Ͽ���Ŀ������ϲ����ũ����Ĳ�ͬ�ط�����

Farmer John ��ũ�����Ա�������һ�� $n$ ���ڵ���������� Bessie ֻ���������ϵ�һЩָ���Ľڵ㴦����Ŀ��ÿ���ڵ��Ƿ�Ҫ����Ŀ���ڳ�ʼʱ��������֤������һ���ڵ㴦�ῴ��Ŀ��

���ҵ��ǣ�Cowflix Ϊ�˱�����ţ��ʹ�ù����˺ţ���ȡ��һ���µĻ�Ա���ԣ�
* Bessie ����θ��ÿ��ѡ����������һ����СΪ $d$ ��**��ͨ��**��Ϊ��֧�� $d+k$ �Ĵ��ۣ����ܹ�����Щλ�ÿ���Ŀ��

����֮��Bessie ��ѡȡ����**��ͨ��** $c_1,c_2,\dots,c_C$��֧�� $\sum_{i=1}^C(|c_i|+k)$ �Ĵ��ۣ��ſ�������Щ��ͨ��ĸ����ڵ㴦����Ŀ������**��ָ���Ľڵ���뱻ĳ����ͨ�����������ָ���Ľڵ㲻�ر�����**��

Bessie ����������ԵĴ���̫�����ˣ������Ƿ�Ҫ���� Mooloo �Ͽ���Ŀ��Ϊ�˰�������ߣ���Ӧ������֮ $k$ ȡ�� $1\sim n$ ʱ����Ŀ����С�ܴ��ۡ�

$1\le n\le2\times10^5$��

```input1
5
10001
1 2
2 3
3 4
4 5
```

```output1
4
6
8
9
10
```

```input2
7
0001010
7 4
5 6
7 2
5 1
6 3
2 5
```

```output2
4
6
8
9
10
11
12
```

## ��ʾ
### Explanation for Sample 1

For $k \le 3$, it's optimal to have two accounts: $c_1=\{1\},c_2=\{5\}$. For $k \ge 3$, it's optimal to have one account: $c_1=\{1,2,3,4,5\}$.

### SCORING

 - Inputs $3-5$: $N \le 5000$
 - Inputs $6-8$: $i$ is connected to $i+1$ for all $i \in [1,N)$.
 - Inputs $9-19$: $N \le 10^5$
 - Inputs $20-24$: No additional constraints.

