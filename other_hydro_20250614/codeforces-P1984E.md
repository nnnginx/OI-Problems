## Description

<div><p>Two hungry red pandas, Oscar and Lura, have a tree $T$ with $n$ nodes. They are willing to perform the following <span class="tex-font-style-bf">shuffle procedure</span> on the whole tree $T$ <span class="tex-font-style-bf">exactly once</span>. With this shuffle procedure, they will create a new tree out of the nodes of the old tree. </p><ol> <li> Choose any node $V$ from the original tree $T$. Create a new tree $T_2$, with $V$ as the root. </li><li> Remove $V$ from $T$, such that the original tree is split into one or more subtrees (or zero subtrees, if $V$ is the only node in $T$). </li><li> Shuffle each subtree with the same procedure (again choosing any node as the root), then connect all shuffled subtrees' roots back to $V$ to finish constructing $T_2$. </li></ol><p>After this, Oscar and Lura are left with a new tree $T_2$. They can only eat leaves and are very hungry, so please find the maximum number of leaves over all trees that can be created in <span class="tex-font-style-bf">exactly one</span> shuffle.</p><p>Note that leaves are all nodes with degree $1$. Thus, the root may be considered as a leaf if it has only one child.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of every test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the number of nodes within the original tree $T$.</p><p>The next $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$)&nbsp;！ an edge within the original tree $T$. The given edges form a tree.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the maximum number of leaves achievable with exactly one shuffle procedure on the whole tree.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of every test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the number of nodes within the original tree $T$.</p><p>The next $n - 1$ lines each contain two integers $u$ and $v$ ($1 \leq u, v \leq n$)&nbsp;！ an edge within the original tree $T$. The given edges form a tree.</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the maximum number of leaves achievable with exactly one shuffle procedure on the whole tree.</p>





```input1|2,3,4,5,6,12,13,14,15,16,17
4
5
1 2
1 3
2 4
2 5
5
1 2
2 3
3 4
4 5
6
1 2
1 3
1 4
1 5
1 6
10
9 3
8 1
10 6
8 5
7 8
4 6
1 3
10 1
2 7
```




```output1
4
3
5
6
```



## Note

<p>In the first test case, it can be shown that the maximum number of leaves is $4$. To accomplish this, we can start our shuffle with selecting node $3$ as the new root. </p><center> <img class="tex-graphics" src="./34739/file/uau7KUFK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Next, we are left only with one subtree, in which we can select node $2$ to be the new root of that subtree. <center> <img class="tex-graphics" src="./34739/file/AfHPcZzj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> This will force all $3$ remaining nodes to be leaves, and once we connect them back to our new root, the shuffled subtree looks like this: <center> <img class="tex-graphics" src="./34739/file/nGMXVq9H.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> We connect the shuffled subtree back to our new root of our new tree. Our final tree has four leaves (including the root), and looks like this: <center> <img class="tex-graphics" src="./34739/file/hUOv1BzQ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In our second test case, we have a line of five nodes. It can be shown that the maximum number of leaves after one shuffle is $3$. We can start off with node $2$, which forces node $1$ to become a leaf. Then, if we select node $4$ on the right side, we will also have nodes $3$ and $5$ as leaves.</p><p>The third test case is a star graph with six nodes. The number of leaves cannot increase, thus our answer will be $5$ (if we start the shuffling with the original root node).</p>
