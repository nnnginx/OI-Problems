## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Misuki has chosen a secret tree with $n$ nodes, indexed from $1$ to $n$, and asked you to guess it by using queries of the following type: </p><ul> <li> <span class="tex-font-style-tt">"? a b"</span>&nbsp;！ Misuki will tell you which node $x$ minimizes $|d(a,x) - d(b,x)|$, where $d(x,y)$ is the distance between nodes $x$ and $y$. If more than one such node exists, Misuki will tell you the one which minimizes $d(a,x)$. </li></ul><p>Find out the structure of Misuki's secret tree using at most $15n$ queries!</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;！ the number of test cases.</p><p>Each test case consists of a single line with an integer $n$ ($2 \le n \le 1000$), the number of nodes in the tree.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $1000$.</p></div><div><h2>Interaction</h2><p>The interaction begins by reading the integer $n$.</p><p>Then you can make up to $15n$ queries.</p><p>To make a query, output a line in the format <span class="tex-font-style-tt">"? a b"</span> (without quotes) ($1 \le a,b \le n$). After each query, read an integer&nbsp;！ the answer to your query.</p><p>To report the answer, output a line in the format <span class="tex-font-style-tt">"! $a_1$ $b_1$ $a_2$ $b_2$ ... $a_{n-1}$ $b_{n-1}$"</span> (without quotes), meaning that there is an edge between nodes $a_i$ and $b_i$, for each $1 \le i \le n-1$. You can print the edges in any order.</p><p>After $15n$ queries have been made, the response to any other query will be $-1$. Once you receive such a response, terminate the program to receive the <span class="tex-font-style-tt">Wrong Answer</span> verdict.</p><p>After printing each line, do not forget to output the end of line and flush the output buffer. Otherwise, you will receive the <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict. To flush, use: </p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hacks, use the following format: The first line contains an integer $t$ ($1 \le t \le 200$)&nbsp;！ the number of test cases.</p><p>The first line of each test contains an integer $n$&nbsp;！ the number of nodes in the hidden tree.</p><p>Then $n-1$ lines follow. The $i$-th of them contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$), meaning that there is an edge between $a_i$ and $b_i$ in the hidden tree.</p><p>The sum of $n$ over all test cases must not exceed $1000$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;！ the number of test cases.</p><p>Each test case consists of a single line with an integer $n$ ($2 \le n \le 1000$), the number of nodes in the tree.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $1000$.</p>





```input1
1
4
1
1
3
```




```output1
? 1 2

? 1 3

? 1 4

! 1 2 1 3 3 4
```



## Note

<p>A tree is an undirected acyclic connected graph. A tree with $n$ nodes will always have $n-1$ edges.</p><p>In the example case, the answer to <span class="tex-font-style-tt">"? 1 2"</span> is $1$. This means that there is an edge between nodes $1$ and $2$.</p><p>The answer to <span class="tex-font-style-tt">"? 1 3"</span> is $1$. This means that there is an edge between nodes $1$ and $3$.</p><p>The answer to <span class="tex-font-style-tt">"? 1 4"</span> is $3$. It can be proven that this can only happen if node $3$ is connected to both node $1$ and $4$.</p><p>The edges of the tree are hence $(1,2)$, $(1,3)$ and $(3,4)$.</p>
