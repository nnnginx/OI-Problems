## Description

<div><p><span class="tex-font-style-bf">This is the Hard Version of the problem. The only difference between the two versions is that in the Hard Version the tree may be of any shape.</span></p><p><span class="tex-font-style-it">This problem is interactive.</span></p><p>Baudelaire is very rich, so he bought a tree of size $n$, rooted at some arbitrary node. Additionally, every node has a value of $1$ or $-1$. </p><p>Cow the Nerd saw the tree and fell in love with it. However, computer science doesn't pay him enough, so he can't afford to buy it. Baudelaire decided to play a game with Cow the Nerd, and if he won, he would gift him the tree.</p><p>Cow the Nerd does not know which node is the root, and he doesn't know the values of the nodes either. However, he can ask Baudelaire queries of two types:</p><ul> <li> $1$ $k$ $u_1$ $u_2$ $...$ $u_k$: Let $f(u)$ be the sum of the values of all nodes in the path from the root of the tree to node $u$. Cow the Nerd may choose an integer $k$ $(1 \le k \le n)$ and $k$ nodes $u_1, u_2, ..., u_k$, and he will receive the value $f(u_1) + f(u_2) + ... + f(u_k)$.</li><li> $2$ $u$: Baudelaire will toggle the value of node $u$. Specifically, if the value of $u$ is $1$, it will become $-1$, and vice versa. </li></ul><p>Cow the Nerd wins if he guesses the value of every node correctly (the values of the final tree, <span class="tex-font-style-bf">after</span> performing the queries) within $n + 200$ total queries. Can you help him win?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \le t \le 100)$, the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^3)$, the size of the tree.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u, v \le n, u \neq v)$, denoting an edge between nodes $u$ and $v$ in the tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$ and that each graph provided is a valid tree.</p></div><div><h2>Interaction</h2><p>To ask a query of type $1$, output a line in the following format (without the quotes):</p><ul> <li> <span class="tex-font-style-tt">"? 1 k $u_1$ $u_2$ $...$ $u_k$"</span>, ($1 \le k, u_i \le n$) </li></ul><p>The jury will return a single integer, $f(u_1) + f(u_2) + ... + f(u_k)$.</p><p>To ask a query of type $2$, output a line in the following format:</p><ul> <li> <span class="tex-font-style-tt">"? 2 $u$"</span> ($1 \le u \le n$) </li></ul><p>The jury will toggle the value of node $u$: if its value is $1$, it will become $-1$ and vice versa.</p><p>When you have found the answer, output a single line in the following format:</p><ul> <li> <span class="tex-font-style-tt">"! $v_1, v_2, ..., v_n$"</span> ($v_i = 1$ or $v_i = -1$, and $v_i$ is the value of node $i$ after performing the queries) </li></ul><p>After that, proceed to process the next test case or terminate the program if it was the last test case. Printing the answer does not count as a query.</p><p>The interactor is <span class="tex-font-style-bf">not</span> adaptive, meaning that the values of the tree are known before the participant asks the queries.</p><p>If your program makes more than $n + 200$ queries, your program should immediately terminate to receive the verdict <span class="tex-font-style-tt">Wrong Answer</span>. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you may get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++ </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hacks, use the following format.</p><p>The first line should contain a single integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases.</p><p>The first line of each test case must contain exactly two integers $n$ and $root$ $(2 \le n \le 10^3, 1 \le root \le n)$&nbsp;！ the size of the tree and the root of the tree.</p><p>The second line of each test case must contain exactly $n$ integers $a_1, a_2, ..., a_n$ $(|a_i| = 1)$&nbsp;！ where $a_i$ is the value of node $i$.</p><p>Each of the following $n-1$ lines must contain exactly two integers $u$ and $v$ $(1 \le u, v \le n)$&nbsp;！ denoting an edge of the tree between nodes $u$ and $v$.</p><p>The sum of $n$ over all test cases must not exceed $10^3$ and every graph provided must be a valid tree.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \le t \le 100)$, the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^3)$, the size of the tree.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u, v \le n, u \neq v)$, denoting an edge between nodes $u$ and $v$ in the tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$ and that each graph provided is a valid tree.</p>





```input1
3
4
1 4
4 2
2 3

1

-1


-5

-5

2
1 2

2

7
1 2
2 7
7 3
7 4
7 5
7 6

-1
```




```output1
? 1 3 1 2 4

? 1 2 3 1

? 2 4
? 1 3 1 2 4

? 1 2 3 1

! -1 -1 -1 -1


? 1 1 1

! 1 1






? 1 1 1

! -1 1 1 1 1 1 -1
```



## Note

<p>In the first example, the root of the tree is node $4$ and the values are: $[-1, -1, -1, 1]$ (the $i$-th value is the value of node $i$).</p><p>Initially, $f(1) = 0, f(2) = 0, f(3) = -1, f(4) = 1$. Therefore, the answer to our first query is $f(1) + f(2) + f(4) = 1$, and of the second query is $f(3) + f(1) = -1$.</p><p>After toggling the value of node $4$, the values are $[-1, -1, -1, -1]$. In addition, $f(1) = -2, f(2) = -2, f(3) = -3, f(4) = -1$. Therefore, $f(1) + f(2) + f(4) = -5$ and $f(3) + f(1) = -5$.</p><p>We answer that the final values of the nodes are $[-1, -1, -1, -1]$, which is correct. Notice that we report the values of the nodes <span class="tex-font-style-bf">after</span> the changes, and not before.</p><p>In the second example, the root of the tree is $2$ and the initial values are $[1, 1]$.</p><p>In the last example, the root of the tree is $1$ and the initial values are $[-1, 1, 1, 1, 1, 1, -1]$.</p><p><span class="tex-font-style-bf">Note that this is just an explanation of how the queries work, and it is not supposed to use any specific strategy to solve the problem.</span></p>
