## Description

<div><p><span class="tex-font-style-it">This is an interactive problem</span>.</p><p>Little Dormi was faced with an awkward problem at the carnival: he has to guess the edges of an unweighted tree of $n$ nodes! The nodes of the tree are numbered from $1$ to $n$.</p><p>The game master only allows him to ask one type of question:</p><ul><li> Little Dormi picks a node $r$ ($1 \le r \le n$), and the game master will reply with an array $d_1, d_2, \ldots, d_n$, where $d_i$ is the length of the shortest path from node $r$ to $i$, for all $1 \le i \le n$.</li></ul><p>Additionally, to <span class="tex-font-style-striked">make the game unfair</span> challenge Little Dormi the game master will allow at most $\lceil\frac{n}{2}\rceil$ questions, where $\lceil x \rceil$ denotes the smallest integer greater than or equal to $x$.</p><p>Faced with the stomach-churning possibility of not being able to guess the tree, Little Dormi needs your help to devise a winning strategy!</p><p>Note that the game master creates the tree before the game starts, and does not change it during the game.</p></div><div class="input-specification"><p>The first line of input contains the integer $n$ ($2 \le n \le 2\,000$), the number of nodes in the tree.</p><p>You will then begin interaction.</p></div><div class="output-specification"><p>When your program has found the tree, first output a line consisting of a single "<span class="tex-font-style-tt">!</span>" followed by $n-1$ lines each with two space separated integers $a$ and $b$, denoting an edge connecting nodes $a$ and $b$ ($1 \le a, b \le n$). Once you are done, terminate your program normally immediately after flushing the output stream.</p><p>You may output the edges in any order and an edge $(a,b)$ is considered the same as an edge $(b,a)$. Answering is not considered as a query.</p></div><div><h2>Interaction</h2><p>After taking input, you may make at most $\lceil\frac{n}{2}\rceil$ queries. Each query is made in the format "<span class="tex-font-style-tt">? r</span>", where $r$ is an integer $1 \le r \le n$ that denotes the node you want to pick for that query.</p><p>You will then receive $n$ space separated integers $d_1, d_2, \ldots, d_n$, where $d_i$ is the length of the shortest path from node $r$ to $i$, followed by a newline.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">If at any point you make an invalid query or try to make more than $\lceil \frac{n}{2} \rceil$ queries, the interaction will terminate immediately and you will receive a Wrong Answer verdict.</span></p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack a solution, use the following format.</p><p>The first line contains the integer $n$ ($2 \le n \le 2\,000$).</p><p>The next $n−1$ lines contain two integers $u$ and $v$ ($1 \le u,v \le n$) denoting an edge between $u$ and $v$ ($u \neq v$). These $n-1$ edges must form a tree.</p></div>

## Input

<p>The first line of input contains the integer $n$ ($2 \le n \le 2\,000$), the number of nodes in the tree.</p><p>You will then begin interaction.</p>

## Output

<p>When your program has found the tree, first output a line consisting of a single "<span class="tex-font-style-tt">!</span>" followed by $n-1$ lines each with two space separated integers $a$ and $b$, denoting an edge connecting nodes $a$ and $b$ ($1 \le a, b \le n$). Once you are done, terminate your program normally immediately after flushing the output stream.</p><p>You may output the edges in any order and an edge $(a,b)$ is considered the same as an edge $(b,a)$. Answering is not considered as a query.</p>

## Samples

```input1
4

0 1 2 2

1 0 1 1
```

```output1
? 1

? 2

!
4 2
1 2
2 3
```






```input2
5

2 2 1 1 0
```

```output2
? 5

!
4 5
3 5
2 4
1 3
```




## Note

<p>Here is the tree from the first example.</p><center> <img class="tex-graphics" src="./32149/file/KmqAJGIG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Notice that the edges can be output in any order.</p><p>Additionally, here are the answers for querying every single node in example $1$:</p><ul><li> $1$: $[0,1,2,2]$ </li><li> $2$: $[1,0,1,1]$ </li><li> $3$: $[2,1,0,2]$ </li><li> $4$: $[2,1,2,0]$</li></ul><p>Below is the tree from the second example interaction.</p><center> <img class="tex-graphics" src="./32149/file/TCeHmUyr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Lastly, here are the answers for querying every single node in example $2$:</p><ul><li> $1$: $[0,4,1,3,2]$ </li><li> $2$: $[4,0,3,1,2]$ </li><li> $3$: $[1,3,0,2,1]$ </li><li> $4$: $[3,1,2,0,1]$ </li><li> $5$: $[2,2,1,1,0]$</li></ul>
