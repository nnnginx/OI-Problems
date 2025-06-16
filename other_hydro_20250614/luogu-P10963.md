## 题目描述
Given a map of islands and bridges that connect these islands, a Hamilton path, as we all know, is a path along the bridges such that it visits each island exactly once. On our map, there is also a positive integer value associated with each island. We call a Hamilton path the best triangular Hamilton path if it maximizes the value described below.

Suppose there are $n$ islands. The value of a Hamilton path $C_1 C_2 \dots C_n $ is calculated as the sum of three parts. Let Vi be the value for the island $C_i$. As the first part, we sum over all the Vi values for each island in the path. For the second part, for each edge $C_i C_{i+1}$ in the path, we add the product $V_i \times V_{i+1}$. And for the third part, whenever three consecutive islands $C_i,C_{i+1},C_{i+2}$ in the path forms a triangle in the map, i.e. there is a bridge between $C_i$ and $C_{i+2}$, we add the product $V_i \times V_{i+1} \times V_{i+2}$.

Most likely but not necessarily, the best triangular Hamilton path you are going to find contains many triangles. It is quite possible that there might be more than one best triangular Hamilton paths; your second task is to find the number of such paths.

## 输入格式

The input file starts with a number $ q  (q \le 20)$ on the first line, which is the number of test cases. Each test case starts with a line with two integers $n$ and $m$, which are the number of islands and the number of bridges in the map, respectively. The next line contains $n$ positive integers, the $i$-th number being the $V_i$ value of island $i$. Each value is no more than $100$. The following $m$ lines are in the form $x\ y$, which indicates there is a (two way) bridge between island $x$ and island $y$. Islands are numbered from $1$ to $n$. You may assume there will be no more than $13$ islands.

## 输出格式
For each test case, output a line with two numbers, separated by a space. The first number is the maximum value of a best triangular Hamilton path; the second number should be the number of different best triangular Hamilton paths. If the test case does not contain a Hamilton path, the output must be $0\ 0$.

Note: A path may be written down in the reversed order. We still think it is the same path.

## 题目大意
**题目描述**

给定一张由岛屿和连接这些岛屿的桥梁构成的地图，众所周知，哈密顿路径是沿着桥梁的路径，能够恰好访问每个岛屿一次。在我们的地图中，每个岛屿还关联一个正整数值。我们定义一种哈密顿路径为 **最佳三角形哈密顿路径**，其最大化以下描述的值。

假设有 $n$ 个岛屿。哈密顿路径 $C_1,C_2,\dots,C_n$ 的值分为三部分计算。设 $V_i$ 为岛屿 $C_i$ 的值。第一部分为路径中每个岛屿的 $V_i$ 值的总和。第二部分，对于路径中的每条边 $C_i C_{i+1}$，加上 $V_i \times V_{i+1}$ 的积。第三部分，对于路径中的每三个连续岛屿 $C_i, C_{i+1}, C_{i+2}$，如果它们在地图中形成一个三角形（即 $C_i$ 和 $C_{i+2}$ 之间有桥），加上 $V_i \times V_{i+1} \times V_{i+2}$ 的积。

最佳三角形哈密顿路径很可能（但不一定）包含多个三角形。可能会存在多个最佳三角形哈密顿路径。你的第二个任务是找出这样的路径的数量。

---

**输入格式**

输入文件的第一行是一个整数 $q\ (q \le 20)$，表示测试用例的数量。

每个测试用例的第一行有两个整数 $n$ 和 $m$，分别表示地图中岛屿的数量和桥梁的数量。

接下来的第一行包含 $n$ 个正整数，第 $i$ 个数是岛屿 $i$ 的 $V_i$ 值。每个值不超过 $100$。

接下来的 $m$ 行，每行的格式为 $x\ y$，表示岛屿 $x$ 和岛屿 $y$ 之间有一座双向桥。岛屿从 $1$ 到 $n$ 编号。可以假设岛屿总数不超过 $13$。

---

**输出格式**

对于每个测试用例，输出一行，包含两个用空格分隔的数。第一个数是最佳三角形哈密顿路径的最大值；第二个数是不同最佳三角形哈密顿路径的数量。如果测试用例中不存在哈密顿路径，则输出 $0\ 0$。

注意：如果一条路径的顺序反转，仍认为它是相同的路径。

```input1

2
3 3
2 2 2
1 2
2 3
3 1 
4 6
1 2 3 4
1 2
1 3
1 4
2 3
24
34
```

```output1
22 3
69 1
```

