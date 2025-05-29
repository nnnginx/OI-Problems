## 题目描述
Having just completed a course in graph algorithms, Bessie the cow has begun
coding her very own graph visualizer! Currently, her graph visualizer is only
capable of visualizing rooted trees with nodes of distinct values, and it can
only perform one kind of operation: merging.

In particular, a merging operation takes any two distinct nodes in a tree with
the same parent and merges them into one node, with value equal to the maximum
of the values of the two nodes merged, and children a union of all the children
of the nodes merged (if any).

Unfortunately, after Bessie performed some merging operations on a tree, her
program crashed, losing the history of the merging operations she performed. All
Bessie remembers is the tree she started with and the tree she ended with after
she performed all her merging operations. 

Given her initial and final trees, please determine a sequence of merging
operations Bessie could have performed. It is guaranteed that a sequence exists.

Each input consists of $T$ independent test cases. It is
guaranteed that the sum of $N$  over all test cases does not exceed $1000$.

## 输入格式
The first line contains $T$, the number of independent test cases. Each test
case is formatted as follows.

The first line of each test case contains the number of nodes $N$ in Bessie's initial tree, which have values $1\dots N$. 

Each of the next $N-1$ lines contains two space-separated node values $v_i$ and
$p_i$ indicating that the node with value $v_i$ is a
child node of the node with value $p_i$ in Bessie's initial tree.

The next line contains the number of nodes $M$ in Bessie's
final tree. 

Each of the next $M-1$ lines contains two space-separated node values $v_i$ and
$p_i$ indicating that the node with value $v_i$ is a
child node of the node with value $p_i$ in Bessie's final tree.

## 输出格式
For each test case, output the number of merging operations, followed by an
ordered sequence of merging operations of that length, one per line. 

Each merging operation should be formatted as two distinct space-separated
integers: the values of the two nodes to merge in any order. 

If there are multiple solutions, output any.

## 题目大意
### 题目描述

刚刚完成了一门图算法课程的奶牛 Bessie 开始编写她自己的图可视化工具！目前，她的图可视化工具只能可视化具有不同节点值的有根树，并且只能执行一种操作：合并。

具体来说，合并操作会选取树中具有相同父节点的任意两个不同节点，并将它们合并为一个节点，新节点的值等于被合并的两个节点值的最大值，而新节点的子节点是被合并节点的所有子节点的并集（如果有的话）。

不幸的是，在 Bessie 对一棵树执行了一些合并操作后，她的程序崩溃了，丢失了她执行的所有合并操作的历史记录。Bessie 只记得她最初开始的树以及执行完所有合并操作后得到的最终树。

给定她的初始树和最终树，请确定 Bessie 可能执行的一系列合并操作。保证存在这样的操作序列。

每个输入包含 $T$ 个独立的测试用例。保证所有测试用例的 $N$ 之和不超过 $1000$。

### 输入格式

第一行包含 $T$，表示独立测试用例的数量。每个测试用例的格式如下。

每个测试用例的第一行包含 Bessie 初始树中的节点数 $N$，节点值为 $1 \dots N$。

接下来的 $N-1$ 行，每行包含两个以空格分隔的节点值 $v_i$ 和 $p_i$，表示在 Bessie 的初始树中，值为 $v_i$ 的节点是值为 $p_i$ 的节点的子节点。

接下来的一行包含 Bessie 最终树中的节点数 $M$。

接下来的 $M-1$ 行，每行包含两个以空格分隔的节点值 $v_i$ 和 $p_i$，表示在 Bessie 的最终树中，值为 $v_i$ 的节点是值为 $p_i$ 的节点的子节点。

### 输出格式

对于每个测试用例，首先输出合并操作的数量，然后按顺序输出相应数量的合并操作，每行一个操作。

每个合并操作应格式化为两个以空格分隔的不同整数：被合并的两个节点的值（顺序任意）。

如果有多个解，输出任意一个即可。

### 提示

$1 \le T \le 100$，$2 \leq N \leq 1000$，$1 \leq v_i, p_i \leq N$，$2 \leq M \leq N$。

- 输入 2-6：初始树和最终树的叶子节点数量相同。
- 输入 7-16：没有额外限制。

```input1
1
8
7 5
2 1
4 2
5 1
3 2
8 5
6 2
4
8 5
5 1
6 5

```

```output1
4
2 5
4 8
3 8
7 8

```

## 提示
$1\le T\le 100$, $2 \leq N \leq 1000$, $1 \leq v_i, p_i \leq N$,$2 \leq M \leq N$.

- Inputs 2-6: The initial and final trees have the same number of leaves.
- Inputs 7-16: No additional constraints.

