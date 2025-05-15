# Description

Santa Claus has a set of fields for his reindeers. In addition to the fields, there is also a set of such

roads, that each road can be used for travelling between exactly two fields. Right now, the roads are arranged in such a way that it is possible to travel from any field to any other field, in which case we say that all fields are connected. Santa is concerned that if a flood washes away a road, this may nolonger be true. Any path whose removal means that all fields are no longer connected, is calledessential. You are to write a program which, given information about the fields and roads, computesthe number of essential roads.
![image](./4346/file/dzOQpRGR_d3GxafYdodeZ.png)

Figure 2 shows fields F1, F2, F3 and F4, and a set of roads. The only essential road is the road between fields F1 and F2, and, thus, the number of essential roads is 1.

# Format

## Input

The name of the input file is break.in. The first line contains two integers, the number of Santa’s

fields F, 1 £ F £ 100000, and the number of roads R, $1 \leq  R \leq  150000$. The fields are identified with

integers from 1 to F. The next R lines each contain information about one road, integers a and b, where

a and b are the numbers of such fields that the road represented by that input file line can be used for

travelling between fields a and b. The order of a and b on the line is meaningless.

## Output

The name of the output file is break.out. The first line of the output file contains one integer: the number of essential paths.

# Samples

```input1
4 4
1 2
2 3
3 4
2 4
```

```output1
1
```

# Limitation

Motivation

The motivation of the problem comes from an algorithm to discover the biconnected components of a

graph. It is a simplification of that problem, since the original algorithm is a little too cumbersome for

an IOI-style problem. This has the additional advantage that slower algorithms are more obvious,

which allows for stratification of the results. Moreover, the solution to this problem is not a simple

extension to a core algorithm.

Solution

With no loss of generality, we may assume that the containers are numbered from 1 to N. The

following algorithm can be used to solve the problem for small inputs.

Algorithm 1

Do a depth first search with a disjoint set data structure. Any edge not in the depth first search tree is

not a bridge every time you find an edge to a visited node that isn't your parent. Mark the nodes up to

the other end of the edge (the other node is an ancestor of yours in the tree). Collapse the disjoint set

data structure when this is done. The edge between any node that isn't marked and isn't the root of the

tree and the node's parent is a bridge.

The basic marking structure is:

for (p = descendent; p != ancestor; p = parent[p]) mark(p);

You have to use depth to handle the collapsing:for (p = descendent; depth[p] > depth[ancestor]; p = parent[p]) mark(p);

Asymptotic running time for this algorithm is O(N + M log* M) .

Algorithm 2

Delete each edge and determine if graph is disconnected . Asymptotic running time for this algorithm is

O((N+M) M)

