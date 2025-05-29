## Description

<div><p>There is an apple tree with $n$ nodes, initially with one apple at each node. You have a paper with you, initially with nothing written on it.</p><p>You are traversing on the apple tree, by doing the following action as long as there is at least one apple left:</p><ul> <li> Choose an <span class="tex-font-style-bf">apple path</span> $(u,v)$. A path $(u,v)$ is called an <span class="tex-font-style-bf">apple path</span> if and only if for every node on the path $(u,v)$, there's an apple on it. </li><li> Let $d$ be the number of apples on the path, write down three numbers $(d,u,v)$, in this order, on the paper. </li><li> Then remove all the apples on the path $(u,v)$. </li></ul><p>Here, the path $(u, v)$ refers to the sequence of vertices on the unique shortest walk from $u$ to $v$. </p><p>Let the number sequence on the paper be $a$. Your task is to find the lexicographically largest possible sequence $a$. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a number $n$ ($1 \le n \le 1.5 \cdot 10^5$).</p><p>The following $n-1$ lines of each test case contain two numbers $u,v$ ($1 \le u,v \le n$). It's guaranteed that the input forms a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1.5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the lexicographically largest sequence possible $a_1, a_2, \ldots, a_{|a|}$. It can be shown that $|a| \le 3 \cdot n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a number $n$ ($1 \le n \le 1.5 \cdot 10^5$).</p><p>The following $n-1$ lines of each test case contain two numbers $u,v$ ($1 \le u,v \le n$). It's guaranteed that the input forms a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1.5 \cdot 10^5$.</p>

## Output

<p>For each test case, output the lexicographically largest sequence possible $a_1, a_2, \ldots, a_{|a|}$. It can be shown that $|a| \le 3 \cdot n$.</p>





```input1|2,3,4,5,10,11,12,13,14,16,17,18,19,20,21,22,23
6
4
1 2
1 3
1 4
4
2 1
2 4
2 3
5
1 2
2 3
3 4
4 5
1
8
6 3
3 5
5 4
4 2
5 1
1 8
3 7
6
3 2
2 6
2 5
5 4
4 1
```




```output1
3 4 3 1 2 2 
3 4 3 1 1 1 
5 5 1 
1 1 1 
5 8 7 2 4 2 1 6 6 
5 6 1 1 3 3
```



## Note

<p>In the first test case, we do the following steps:</p><ul> <li> Choose the apple path $(4, 3)$. This path consists of the nodes $4, 1, 3$, and each of them have an apple (so it is a valid apple path). $d = 3$ as there are $3$ apples on this path. Append $3, 4, 3$ in that order to our sequence $a$. Now, remove the apples from these $3$ vertices. </li><li> Only node $2$ has an apple left. Choose the apple path $(2, 2)$. This path only consists of the single node $2$. $d = 1$ as there is $1$ apple on this path. Append $1, 2, 2$ in that order to our sequence $a$ and remove the apple from $2$. </li></ul><p>The final sequence is thus $[3, 4, 3, 1, 2, 2]$. It can be shown this is the lexicographically largest sequence possible.</p>
