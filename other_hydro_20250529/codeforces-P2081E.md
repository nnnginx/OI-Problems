## Description

<div><p>Given a rooted tree with $n+1$ nodes labeled from $0$ to $n$, where the root is node $0$, and <span class="tex-font-style-bf">its only child is node $1$</span>. There are $m$ <span class="tex-font-style-bf">distinct</span> chips labeled from $1$ to $m$, each colored either black or white. Initially, they are arranged on edge $(0,1)$ from top to bottom in ascending order of labels.</p><center> <img class="tex-graphics" height="189px" src="./36068/file/cpBRsRBd.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The initial position of the chips. Tree nodes are shown in blue.</span> </center><p>You can perform the following operations any number of times (possibly zero) in any order:</p><ul> <li> Select two edges ($u,v$) and ($v,w$) such that $u$ is the parent of $v$ and $v$ is the parent of $w$, where edge ($u,v$) contains at least one chip. Move the <span class="tex-font-style-bf">bottommost</span> chip on edge ($u,v$) to the <span class="tex-font-style-bf">topmost</span> place on edge ($v,w$), i.&nbsp;e., above all existing chips on ($v,w$). </li><li> Select two edges ($u,v$) and ($v,w$) such that $u$ is the parent of $v$ and $v$ is the parent of $w$, where edge ($v,w$) contains at least one chip. Move the <span class="tex-font-style-bf">topmost</span> chip on edge ($v,w$) to the <span class="tex-font-style-bf">bottommost</span> place on edge ($u,v$), i.&nbsp;e., below all existing chips on ($u,v$). </li><li> Select two <span class="tex-font-style-bf">adjacent</span> chips of the same color on the same edge, and swap their positions. </li></ul><center> <img class="tex-graphics" height="189px" src="./36068/file/AFtGXnGK.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Permitted operations.</span> </center><p>Each chip $i$ has a movement range, defined as all edges on the simple path from the root to node $d_i$. During operations, you must ensure that no chip is moved to an edge outside its movement range.</p><p>Finally, you must move all chips back to edge $(0,1)$. It can be found that the order of the chips may change. Compute the number of possible permutations of chips for the final arrangement on the edge $(0,1)$ modulo $998\,244\,353$.</p><p>A permutation of chips is defined as a sequence of length $m$ consisting of the <span class="tex-font-style-bf">labels</span> of the chips from top to bottom.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 5000$)&nbsp;！ the size of the tree minus one (i.&nbsp;e., the tree has $n+1$ nodes) and the number of chips.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($0 \le p_i &lt; i$)&nbsp;！ the parent nodes for nodes from $1$ to $n$. It is guaranteed that $p_i = 0$ if and only if $i = 1$ (the root's only child is node $1$).</p><p>The third line contains $m$ integers $c_1, c_2, \ldots, c_m$ ($c_i \in \{0, 1\}$)&nbsp;！ the color of each chip ($0$ for black, $1$ for white).</p><p>The fourth line contains $m$ integers $d_1, d_2, \ldots, d_m$ ($1\le d_i \le n$)&nbsp;！ the movement range of each chip.</p><p>It is guaranteed that the sum of $n$ does not exceed $5000$ and the sum of $m$ does not exceed $5000$ across all test cases.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of possible permutations of chips modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 5000$)&nbsp;！ the size of the tree minus one (i.&nbsp;e., the tree has $n+1$ nodes) and the number of chips.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($0 \le p_i &lt; i$)&nbsp;！ the parent nodes for nodes from $1$ to $n$. It is guaranteed that $p_i = 0$ if and only if $i = 1$ (the root's only child is node $1$).</p><p>The third line contains $m$ integers $c_1, c_2, \ldots, c_m$ ($c_i \in \{0, 1\}$)&nbsp;！ the color of each chip ($0$ for black, $1$ for white).</p><p>The fourth line contains $m$ integers $d_1, d_2, \ldots, d_m$ ($1\le d_i \le n$)&nbsp;！ the movement range of each chip.</p><p>It is guaranteed that the sum of $n$ does not exceed $5000$ and the sum of $m$ does not exceed $5000$ across all test cases.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of possible permutations of chips modulo $998\,244\,353$.</p>





```input1|2,3,4,5,10,11,12,13
4
3 2
0 1 1
0 1
2 3
4 4
0 1 1 2
0 0 1 1
1 2 3 3
6 6
0 1 1 1 4 5
0 0 0 0 1 1
5 6 1 2 4 3
16 15
0 1 1 3 1 3 4 3 3 7 1 6 11 5 8 10
1 0 1 1 0 1 1 1 1 0 1 1 0 0 0
12 14 13 10 9 16 11 14 13 15 16 10 2 2 5
```




```output1
2
8
108
328459046
```



## Note

<p>In the first test case, we can reach follow $2$ permutations: ($1,2$) and ($2,1$).</p><p>In the second test case, we can reach follow $8$ permutations: ($1,2,3,4$), ($1,2,4,3$), ($1,3,2,4$), ($1,3,4,2$), ($1,4,2,3$), ($1,4,3,2$), ($2,1,3,4$), and ($2,1,4,3$).</p>
