## Description

For an $n$-order permutation $p$, we set up an **undirected simple graph** $G(p)$ with $n$ vertices numbered from $1$ to $n$.
We create an edge between each vertice $i$ and the nearest vertices in each side which correspond a greater (or less) $p$ value than $p_i$.  
Formally,in this graph, $\forall u<v$, the edge $(u, v)$ exists iff at least one of the following four conditions hold:

* $p_u<p_v$, and no $u<i<v$ exists such that $p_u<p_i$;
* $p_u>p_v$, and no $u<i<v$ exists such that $p_u>p_i$;
* $p_u<p_v$, and no $u<i<v$ exists such that $p_i<p_v$;
* $p_u>p_v$, and no $u<i<v$ exists such that $p_i>p_v$.

Now we randomly choose a permutation $p$ from all $n$-order permutations. Your task is to calculate the expected number of the $3$-cycles in $G(p)$. You only need to output the answer modulo $998244353$. 

## Input Format

The only line contains a positive integer $n$ which means the order of the permutation. 

## Output Format

Output only one line,which contains an integer $\mathrm{ans}$ which means the expected number of the $3$-cycles in $G(p)$ modulo $998244353$. 

```input1
3
```

```output1
665496236
```

```input2
91
```

```output2
116578319
```

```input3
3
```

```output3
665496236
```

```input4
91
```

```output4
116578319
```

## Constraints

For all test cases, $1\le n<998244353$.

Detailed constraints are as follows (blank grids denote the same constraints as mentioned above):

|Subtask #|Score (percentage)|$n$|
|:-:|:-:|:-:|
|$1$|$15$|$\le 10$|
|$2$|$20$|$\le 100$|
|$3$|$40$|$\le 10^6$|
|$4$|$15$|$\ge 998000000$|
|$5$|$10$|-|

