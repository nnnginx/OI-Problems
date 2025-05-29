## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference between the two versions is that in this version, it is guaranteed that every node is adjacent to node $1$.</span></p><p><span class="tex-font-style-it">This problem is interactive.</span></p><p>Baudelaire is very rich, so he bought a tree of size $n$ that is rooted at some arbitrary node. Additionally, every node has a value of $1$ or $-1$. <span class="tex-font-style-bf">In this version, every node is adjacent to node $1$. However, please note that node $1$ is not necessarily the root.</span></p><p>Cow the Nerd saw the tree and fell in love with it. However, computer science doesn't pay him enough, so he can't afford to buy it. Baudelaire decided to play a game with Cow the Nerd, and if he won, he would gift him the tree.</p><p>Cow the Nerd does not know which node is the root, and he doesn't know the values of the nodes either. However, he can ask Baudelaire queries of two types:</p><ul> <li> $1$ $k$ $u_1$ $u_2$ $...$ $u_k$: Let $f(u)$ be the sum of the values of all nodes in the path from the root of the tree to node $u$. Cow the Nerd may choose an integer $k$ $(1 \le k \le n)$ and $k$ nodes $u_1, u_2, ..., u_k$, and he will receive the value $f(u_1) + f(u_2) + ... + f(u_k)$.</li><li> $2$ $u$: Baudelaire will toggle the value of node $u$. Specifically, if the value of $u$ is $1$ it will become $-1$, and vice versa. </li></ul><p>Cow the Nerd wins if he guesses the value of every node correctly (the values of the final tree, <span class="tex-font-style-bf">after</span> performing the queries) within $n + 200$ total queries. Can you help him win?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \le t \le 100)$, the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^3)$, the size of the tree.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u, v \le n, u \neq v)$, denoting an edge between nodes $u$ and $v$ in the tree. <span class="tex-font-style-bf">In this version, it is guaranteed that either $u = 1$ or $v = 1$</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$ and that each graph provided is a valid tree.</p></div><div><h2>Interaction</h2><p>To ask a query of type $1$, output a line in the following format (without the quotes):</p><ul> <li> <span class="tex-font-style-tt">"? 1 k $u_1$ $u_2$ $...$ $u_k$"</span>, ($1 \le k, u_i \le n$) </li></ul><p>The jury will return a single integer, $f(u_1) + f(u_2) + ... + f(u_k)$.</p><p>To ask a query of type $2$, output a line in the following format:</p><ul> <li> <span class="tex-font-style-tt">"? 2 $u$"</span> ($1 \le u \le n$) </li></ul><p>The jury will toggle the value of node $u$: if its value is $1$ it will become $-1$ and vice versa.</p><p>When you have found the answer, output a single line in the following format:</p><ul> <li> <span class="tex-font-style-tt">"! $v_1, v_2, ..., v_n$"</span> ($v_i = 1$ or $v_i = -1$, and $v_i$ is the value of node $i$ after performing the queries) </li></ul><p>After that, proceed to process the next test case or terminate the program if it was the last test case. Printing the answer does not count as a query.</p><p>The interactor is <span class="tex-font-style-bf">not</span> adaptive, meaning that the values of the tree are known before the participant asks the queries.</p><p>If your program makes more than $n + 200$ queries, your program should immediately terminate to receive the verdict <span class="tex-font-style-tt">Wrong Answer</span>. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you may get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++ </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>For hacks, use the following format.</p><p>The first line should contain a single integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases.</p><p>The first line of each test case must contain exactly two integers $n$ and $root$ $(2 \le n \le 10^3, 1 \le root \le n)$&nbsp;！ the size of the tree and the root of the tree.</p><p>The second line of each test case must contain exactly $n$ integers $a_1, a_2, ..., a_n$ $(|a_i| = 1)$&nbsp;！ where $a_i$ is the value of node $i$.</p><p>Each of the following $n-1$ lines must contain exactly two integers $u$ and $v$ $(1 \le u, v \le n)$&nbsp;！ denoting an edge of the tree between nodes $u$ and $v$.</p><p>The sum of $n$ over all test cases must not exceed $10^3$ and every graph provided must be a valid tree. <span class="tex-font-style-bf">For this version, every node must be adjacent to node $1$</span>.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \le t \le 100)$, the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^3)$, the size of the tree.</p><p>Each of the next $n-1$ lines contains two integers $u$ and $v$ $(1 \le u, v \le n, u \neq v)$, denoting an edge between nodes $u$ and $v$ in the tree. <span class="tex-font-style-bf">In this version, it is guaranteed that either $u = 1$ or $v = 1$</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$ and that each graph provided is a valid tree.</p>





```input1
1
4
1 2
3 1
1 4

0


-6
```




```output1
? 1 3 1 2 3

? 2 2
? 1 3 1 2 3

! -1 -1 -1 1
```



## Note

<p>In the example, the root of the tree is node $2$, and the values of the nodes are $[-1, 1, -1, 1]$. Therefore, $f(1) = 0, f(2) = 1, f(3) = -1, f(4) = 1$.</p><p>First, we query about the sum $f(1) + f(2) + f(3)$, so we receive the value $0$. Then, we toggle the value of node $2$, and the values are: $[-1, -1, -1, 1]$. Therefore, $f(1) = -2, f(2) = -1, f(3) = -3, f(4) = -1$, and $f(1) + f(2) + f(3) = -6$.</p><p>Finally, we figure out that the values of the nodes are $[-1, -1, -1, 1]$, so we answer that.</p><p><span class="tex-font-style-bf">Note that this is just an explanation of how the queries work, and it is not supposed to use any specific strategy to solve the problem.</span></p>
