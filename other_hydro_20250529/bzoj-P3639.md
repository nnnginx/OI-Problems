


## 题目描述
You are given a tree (an acyclic undirected connected graph) with n nodes. The tree nodes are numbered from 1 to n. 
Each node has a color, white or black, and a weight.
We will ask you to perfrom some instructions of the following form:
<ul type="disc">

0 u : ask for the maximum weight among the nodes which are connected to u, two nodes are connected iff all the node on the path from u to v (inclusive u and v) have a same color. 
1 u : toggle the color of u(that is, from black to white, or from white to black). 
2 u w: change the weight of u to w. 
## 输入格式
The first line contains a number n denoted how many nodes in the tree(1 ≤ n ≤ 10^{5}). The next n - 1 lines, each line has two numbers (u,  v) describe a edge of the tree(1 ≤ u,  v ≤ n). 
The next 2 lines, each line contains n number, the first line is the initial color of each node(0 or 1), and the second line is the initial weight, let's say W_{i}, of each node(|W_{i}| ≤ 10^{9}).
The next line contains a number m denoted how many operations we are going to process(1 ≤ m ≤ 10^{5}). The next m lines, each line describe a operation (t,  u) as we mentioned above(0 ≤ t ≤ 2, 1 ≤ u ≤ n, |w| ≤ 10^{9}).
## 输出格式
For each query operation, output the corresponding result.

```input1
5
1 2
1 3
1 4
1 5
0 1 1 1 1
1 2 3 4 5
3
0 1
1 1
0 1

```
```output1
1
5
```

## 提示
没有写明提示
## 题目来源
By xiaodao


