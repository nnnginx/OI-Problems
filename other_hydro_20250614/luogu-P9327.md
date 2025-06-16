## ��Ŀ����
As the newly elected mayor of Kitchener, Alanna's first job is to improve the city's road plan.

Kitchener's current road plan can be represented as a collection of $N$ intersections with $M$ roads, where the $i\text{-th}$ road has length $l_i$ meters, costs $c_i$ dollars per year to maintain, and connects intersections $u_i$ and $v_i$. To create a plan, Alanna must select some subset of the $M$ roads to keep and maintain, and that plan's cost is the sum of maintenance costs of all roads in that subset.

To lower the city's annual spending, Alanna would like to minimize the plan's cost. However, the city also requires that she minimizes travel distances between intersections and will reject any plan that does not conform to those rules. Formally, for any pair of intersections $(i, j)$, if there exists a path from $i$ to $j$ taking $l$ meters on the existing road plan, Alanna's plan must also include a path between those intersections that is at most $l$ meters.

## �����ʽ
The first line contains the integers $N$ and $M$.

Each of the next $M$ lines contains the integers $u_i,v_i,l_i$ and $c_i$, meaning that there currently exists a road from intersection $u_i$ to intersection $v_i$ with length $l_i$ and cost $c_i$$(1 \leq u_i, v_i \leq N, u_i \neq v_i)$.

The following table shows how the available 15 marks are distributed.

| Marks | Bounds on $N$ and $M$ | Bounds on $l_i$ | Bounds on $c_i$ | Additional Constraints |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
| $3$ marks | $1 \leq N\leq 2000$, $1\leq M \leq 2000$ | $l_i = 0$ | $1 \leq c_i \leq 10^9$ | None. |
| $6$ marks | $1 \leq N\leq 2000$, $1\leq M \leq 2000$ | $1 \leq l_i \leq 10^9$ | $1 \leq c_i \leq 10^9$ | There is at most one road between any unordered pair of intersections. |
| $6$ marks | $1 \leq N\leq 2000$, $1\leq M \leq 2000$ | $0 \leq l_i \leq 10^9$ | $1 \leq c_i \leq 10^9$ | None. |


## �����ʽ
Output one integer, the minimum possible cost of a road plan that meets the requirements.

## ��Ŀ����
����һ�� $N(1\leq N \leq 2000)$ ���������ͼ�� $M(1\leq M \leq 2000)$ ������ߣ��� $i$ �������ӵ� $u_i$ �� $v_i$������Ϊ $l_i(0\leq l_i \leq 10^9)$��ά�������� $c_i(1\leq c_i \leq 10^9)$������Ҫѡ������ܺ���С�ı߼���ʹ��ֻ������Щ�ߺ��������������·���Ȳ��䡣

�����С�ķ����ܺ͡�

```input1
5 7
1 2 15 1
2 4 9 9
5 2 5 6
4 5 4 4
4 3 3 7
1 3 2 7
1 4 2 1
```

```output1
25
```

## ��ʾ
Explanation of Output for Sample Input��

Here is a diagram of the intersections along with a valid road plan with minimum cost.

![](https://cdn.luogu.com.cn/upload/image_hosting/2astpvkm.png)

Each edge is labeled with a pair $(l, c)$ denoting that it has length $l$ meters and cost $c$ dollars.

Additionally, the roads that are part of the plan are highlighted in blue, with a total cost of $7 + 1 + 6 + 7 + 4 = 25$.

It can be shown that we cannot create a cheaper plan that also respects the city��s requirements.

**��������������**��

- Subtask 1��3 points�������ݱ�֤ $1\leq N \leq 2000$��$1\leq M \leq 2000$��$l_i = 0$��$1\leq c_i \leq 10^9$��

- Subtask 2��6 points�������ݱ�֤ $1\leq N\leq 2000$��$1\leq M \leq 2000$��$1\leq l_i \leq 10^9$��$1\leq c_i \leq 10^9$�������κ�һ��ʮ��·��֮�����ֻ��һ��·��

- Subtask 3��6 points�������ݱ�֤ $1\leq N\leq 2000$��$1\leq M \leq 2000$��$0\leq l_i \leq 10^9$��$1\leq c_i \leq 10^9$��

