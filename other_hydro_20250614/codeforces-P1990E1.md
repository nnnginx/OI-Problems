## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference is the limit on the number of queries.</span></p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>You are given a tree of $n$ nodes with node $1$ as its root node.</p><p>There is a hidden mole in one of the nodes. To find its position, you can pick an integer $x$ ($1 \le x \le n$) to make an inquiry to the jury. Next, the jury will return $1$ when the mole is in subtree $x$. Otherwise, the judge will return $0$. If the judge returns $0$ and the mole is not in root node $1$, the mole will move to the parent node of the node it is currently on.</p><p>Use at most $300$ operations to find the <span class="tex-font-style-bf">current</span> node where the mole is located.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p></div><div><h2>Interaction</h2><p>The first line of each test case contains one integer $n$ ($2 \le n \le 5000$). </p><p>The following $n-1$ lines describe the edges of the tree. Each line contains two space-separated integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$), indicating an edge between nodes $u_i$ and $v_i$.</p><p>It is guaranteed that the input data represents a tree.</p><p>The interactor in this task is <span class="tex-font-style-bf">not adaptive</span>. In other words, the node where the mole is located at first is fixed in every test case and does not change during the interaction.</p><p>To ask a query, you need to pick a vertex $x$ ($1 \le x \le n$) and print the line of the following form:</p><ul> <li> "<span class="tex-font-style-tt">? x</span>" </li></ul><p>After that, you receive:</p><ul> <li> $0$ if the mole is not in subtree $x$; </li><li> $1$ if the mole is in subtree $x$. </li></ul><p>You can make at most $300$ queries of this form for each test case.</p><p>Next, if your program has found the <span class="tex-font-style-bf">current</span> node where the mole is located, print the line of the following form:</p><ul> <li> "<span class="tex-font-style-tt">! x</span>" </li></ul><p>Note that this line is <span class="tex-font-style-bf">not</span> considered a query and is <span class="tex-font-style-bf">not</span> taken into account when counting the number of queries asked.</p><p>After this, proceed to the next test case.</p><p>If you make more than $300$ queries during an interaction, your program must terminate immediately, and you will receive the <span class="tex-font-style-tt">Wrong Answer</span> verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query or the answer for a test case, do not forget to output the end of line and flush the output. Otherwise, you will get the verdict <span class="tex-font-style-tt">Idleness Limit Exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, follow the test format below.</p><p>The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $x$ ($2 \le n \le 5000$, $1 \le x \le n$)&nbsp;¡ª the size of the tree and the initial position of the mole.</p><p>The following $n-1$ lines describe the edges of the tree. Each line contains two space-separated integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$), indicating an edge between nodes $u_i$ and $v_i$.</p><p>The input data must represent a tree.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows.</p>





```input1
2
2
1 2

1

6
1 2
1 3
1 4
4 5
5 6

0

0

1
```




```output1
? 2

! 2






? 2

? 6

? 4

! 4
```



## Note

<p>In the first test case, the mole is in node $2$ initially.</p><p>For the query "<span class="tex-font-style-tt">? 2</span>", the jury returns $1$ because the mole is in subtree $2$. After this query, the mole does not move.</p><p>The answer $2$ is the <span class="tex-font-style-bf">current</span> node where the mole is located, so the answer is considered correct.</p><p>In the second test case, the mole is in node $6$ initially.</p><p>For the query "<span class="tex-font-style-tt">? 2</span>", the jury returns $0$ because the mole is not in subtree $2$. After this query, the mole moves from node $6$ to node $5$.</p><p>For the query "<span class="tex-font-style-tt">? 6</span>", the jury returns $0$ because the mole is not in subtree $6$. After this query, the mole moves from node $5$ to node $4$.</p><p>For the query "<span class="tex-font-style-tt">? 4</span>", the jury returns $1$ because the mole is in subtree $4$. After this query, the mole does not move.</p><p>The answer $4$ is the <span class="tex-font-style-bf">current</span> node where the mole is located, so the answer is considered correct.</p><p>Please note that the example is only for understanding the statement, and the queries in the example do <span class="tex-font-style-bf">not</span> guarantee to determine the unique position of the mole.</p>
