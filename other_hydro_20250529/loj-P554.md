## Description


For an $n$-order permutation $p$, we set up an **undirected simple graph** $G(p)$ with $n$ vertices numbered from $1$ to $n$.
We create an edge between each vertice $i$ and the nearest vertices in each side which correspond a greater (or less) $p$ value than $p_i$.  
Formally,in this graph, $\forall u<v$, the edge $(u, v)$ exists iff at least one of the following four conditions hold:

* $p_u<p_v$, and no $u<i<v$ exists such that $p_u<p_i$;
* $p_u>p_v$, and no $u<i<v$ exists such that $p_u>p_i$;
* $p_u<p_v$, and no $u<i<v$ exists such that $p_i<p_v$;
* $p_u>p_v$, and no $u<i<v$ exists such that $p_i>p_v$.

For a segment $[l,r]$, define its **corresponding permutation** $p[l:r]$ as an $(r-l+1)$-order permutation with the same relative orders of elements as $p_l,p_{l+1},\cdots,p_r$; that is, for all $1 \leq i < j \leq r-l+1$, the boolean value $[p_{l-1+i} < p_{l-1+j}]$ is the same as the boolean value $[(p[l:r])_i < (p[l:r])_j]$.   
For instance, for the permutation $q=\{1,4,2,5,3\}$, $q[2:4]$ is a permutation of length $3$ with the same relative orders of elements as $\{4,2,5\}$, i.e. $\{2,1,3\}$.

The [chromatic number](https://en.wikipedia.org/wiki/Graph_coloring) of an undirected graph $G$ is the smallest number of colors needed to give each vertex a color such that every edge connects two vertices with different colors. We call this $c(G)$.

Given a permutation $p$ of length $n$, please find the chromatic number of $G(p)$.   
Additionally, please answer $q$ queries in the form of $[l,r]$ asking for: the greatest chromatic number among those of all **corresponding permutations** of each subsegment of $[l,r]$, $\mathrm{maxc}$; and the number of subsegment that achieve this maximum number $\mathrm{cnt}$.  
(Formally,for each given $l,r$,$\forall l\le l'\le r' \le r$,calculate the maximum possible value of $c(G(p[l':r']))$,called $\mathrm{maxc}$,and $\sum_{l\leqslant l'\leqslant r'\leqslant r}[c(G(p[l':r']))=\mathrm{maxc}]=\mathrm{cnt}$ .)

## Input format

The first line contains a positive integer $n$.

The second line contains $n$ positive integers $p_1,p_2,\cdots ,p_n$.

The third line contains an integer $q$.

The following $q$ lines each contains two positive integers $l,r$, denoting a query.

## Output Format

Output contains $q+1$ lines in total. The first one should contain a positive integer denoting the chromatic number of $G(p)$, followed by $q$ lines each containing two integers $\mathrm{maxc},\mathrm{cnt}$ for each query.

```input1
6
1 4 5 3 6 2
5
1 6
1 3
2 5
2 6
3 3
```

```output1
4
4 1
2 3
3 3
3 6
1 1
```

```input2
6
1 4 5 3 6 2
5
1 6
1 3
2 5
2 6
3 3
```

```output2
4
4 1
2 3
3 3
3 6
1 1
```

## Constraints

For all test cases, $1\le n\le 3\times 10^5,0\le q\le 3\times 10^5$.

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):

|Subtask #|Score (percentage)|$n$|$q$|
|:-:|:-:|:-:|:-:|
|$1$|$10$|$\le 10$|$\le 10$|
|$2$|$15$|$\le 100$|$\le 10^4$|
|$3$|$15$|$\le 2000$|$\le 10^4$|
|$4$|$15$|-|$=0$|
|$5$|$15$|-|$\le 5$|
|$6$|$30$|-|-|

