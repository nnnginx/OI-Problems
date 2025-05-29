## 题目描述
Kasra and Arshia commute so much with each other these days and Arshia has made him perverted. They drive...

Wait, wait, wait... why so long stories?

We have a directed graph, we want to choose a sequence of directed simple cycles from it, such that no vertex comes in more than one cycle, and we can start from some node in the graph and go through the cycles one by one, this means that we should be able to go from the first node to the first cycle, and then be able to go from any cycle to the next cycle using edges of the graph, keep care that the vertices we traverse to go from some cycle to the next cycle are not important and it's ok to go to some vertices more than once in these paths.

Now we want to know, in how many ways we can choose these cycles, since this question can be a bit hard, it's enough to determine the parity of the answer.

Note that the sequence can be empty, and two ways of choosing cycles is different if and only if the set of cycles we choose in these two ways will be different.

## 输入格式
In the first line of input there is two integer $n$ and $m$, the number of vertices and edges of the graph.

In next $m$ lines edges of the graph will be given.

## 输出格式
If the parity of answer if even, print the phrase "Daddy: We should have a date...", and if the parity is odd print "Mistletoe: Time to go home!".

```input1
4 4
3 1
1 2
3 4
2 3
```

```output1
Daddy: We should have a date...
```

```input2
6 8
1 4
1 2
4 5
5 1
6 2
2 3
3 1
6 1
```

```output2
Mistletoe: Time to go home!
```

```input3
12 16
8 6
1 2
7 8
10 11
1 4
4 5
11 12
5 1
1 6
12 10
2 3
6 9
3 1
6 7
9 8
5 10
```

```output3
Daddy: We should have a date...
```

## 提示
### Constraints

- $1 \leq n \leq 5000$
- $0 \leq m \leq \min (\binom{n}{2},10^6)$
- $1 \leq u_{i}, v_{i} \leq n$

### Subtasks

| subtask | score | limits |
| :---: | :---: | :---: |
| 1 | 13 | The undirected underlying graph is a cactus ${ }^{1}$ |
| 2 | 36 | $1 \leq n \leq 500$ Graph is strongly connected. |
| 3 | 51 | No extra limits |

${}^1$: Cactus is an undirected graph which every two cycles have at most one common vertex.

