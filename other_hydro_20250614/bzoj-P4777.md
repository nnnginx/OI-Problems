## 题目描述

Farmer John has recently been experimenting with cultivating different types of grass on his farm, realizing that different types of cows like different types of grass. However, he must be careful to ensure that different types of grass are planted sufficiently far away from each-other, in order to prevent them from being inextricably mixed.

FJ&#039;s farm consists of $n$ fields, where $m$ pairs of fields are connected by bi-directional pathways. Using these pathways, it is possible to walk from any field to any other field. Any pair of fields will be linked by at most one direct pathway.

In each field, FJ initially plants one of $k$ types of grass. Over time, however, he might decide to switch the grass in some field to a different type. He calls this an "update" peration. He might perform several updates over the course of time, which are all cumulative in nature.

After each update, FJ would like to know the length of the shortest path between two fields having different grass types. That is, among all pairs of fields having different grass types, he wants to know which two are closest. Ideally,

this number is large, so he can prevent grass of one type from mixing with grass of another type. It is guaranteed that the farm will always have at least two fields with different grass types.

In $30$ percent of the input cases, each field will be directly connected to at most $10$ pathways.

## 输入格式

The first line of input contains four integers, $n$, $m$, $k$, and $Q$, where $Q$ is the number of updates.  
The next $m$ lines describe the paths; each one contains three integers $a$, $b$, and $l$, indicating a path from field $a$ to field $b$ (both integers in the range $1 \ldots n$) of length $l$.  
The next line indicates the initial type of grass growing in each field ($n$ integers in the range $1 \ldots k$).  
Finally, the last $Q$ lines each describe an update, specified by two integers $a$ and $b$, where the grass in field $a$ is to be updated to type $b$.

## 输出格式

For each update, print the length of the shortest path between two fields with different types of grass, after the update is applied.



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

## 数据规模与约定

对于 $100\%$ 的数据，$1 \leq k \leq n$，$1\le n,m\le 2\times 10^5$，$1 \leq Q \leq 2\times 10^5$。  
Each pathway has an integer length in the range $[1,10^6]$. 

## 题目来源

Platinum