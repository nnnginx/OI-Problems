## Description

<div><p>Now Serval is a junior high school student in Japari Middle School, and he is still thrilled on math as before. </p><p>As a talented boy in mathematics, he likes to play with numbers. This time, he wants to play with numbers on a rooted tree.</p><p>A tree is a connected graph without cycles. A rooted tree has a special vertex called the root. A parent of a node $v$ is the last different from $v$ vertex on the path from the root to the vertex $v$. Children of vertex $v$ are all nodes for which $v$ is the parent. A vertex is a leaf if it has no children.</p><p>The rooted tree Serval owns has $n$ nodes, node $1$ is the root. Serval will write some numbers into all nodes of the tree. However, there are some restrictions. Each of the nodes except leaves has an operation $\max$ or $\min$ written in it, indicating that the number in this node should be equal to the maximum or minimum of all the numbers in its sons, respectively. </p><p>Assume that there are $k$ leaves in the tree. Serval wants to put integers $1, 2, \ldots, k$ to the $k$ leaves (each number should be used exactly once). He loves large numbers, so he wants to maximize the number in the root. As his best friend, can you help him?</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 3\cdot 10^5$), the size of the tree.</p><p>The second line contains $n$ integers, the $i$-th of them represents the operation in the node $i$. $0$ represents $\min$ and $1$ represents $\max$. If the node is a leaf, there is still a number of $0$ or $1$, but you can ignore it.</p><p>The third line contains $n-1$ integers $f_2, f_3, \ldots, f_n$ ($1 \leq f_i \leq i-1$), where $f_i$ represents the parent of the node $i$.</p></div><div class="output-specification"><p>Output one integer&nbsp;�� the maximum possible number in the root of the tree.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 3\cdot 10^5$), the size of the tree.</p><p>The second line contains $n$ integers, the $i$-th of them represents the operation in the node $i$. $0$ represents $\min$ and $1$ represents $\max$. If the node is a leaf, there is still a number of $0$ or $1$, but you can ignore it.</p><p>The third line contains $n-1$ integers $f_2, f_3, \ldots, f_n$ ($1 \leq f_i \leq i-1$), where $f_i$ represents the parent of the node $i$.</p>

## Output

<p>Output one integer&nbsp;�� the maximum possible number in the root of the tree.</p>

## Samples

```input1
6
1 0 1 1 0 1
1 2 2 2 2
```

```output1
1
```






```input2
5
1 0 1 0 1
1 1 1 1
```

```output2
4
```






```input3
8
1 0 0 1 0 1 1 0
1 1 2 2 3 3 3
```

```output3
4
```






```input4
9
1 1 0 0 1 0 1 0 1
1 1 2 2 3 3 4 4
```

```output4
5
```




## Note

<p>Pictures below explain the examples. The numbers written in the middle of the nodes are their indices, and the numbers written on the top are the numbers written in the nodes.</p><p>In the first example, no matter how you arrange the numbers, the answer is $1$.</p><center> <img class="tex-graphics" src="./30118/file/xQAYaKge.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example, no matter how you arrange the numbers, the answer is $4$.</p><center> <img class="tex-graphics" src="./30118/file/nhv2LnYE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third example, one of the best solution to achieve $4$ is to arrange $4$ and $5$ to nodes $4$ and $5$.</p><center> <img class="tex-graphics" src="./30118/file/2x9jyOBE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth example, the best solution is to arrange $5$ to node $5$.</p><center> <img class="tex-graphics" src="./30118/file/MJZgLOi4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
