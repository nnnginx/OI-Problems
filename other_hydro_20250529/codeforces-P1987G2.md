## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference between the two versions are the allowed characters in $s$. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given a permutation $p$ of length $n$. You are also given a string $s$ of length $n$, where each character is either <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, or <span class="tex-font-style-tt">?</span>.</p><p>For each $i$ from $1$ to $n$: </p><ul> <li> Define $l_i$ as the largest index $j &lt; i$ such that $p_j &gt; p_i$. If there is no such index, $l_i := i$. </li><li> Define $r_i$ as the smallest index $j &gt; i$ such that $p_j &gt; p_i$. If there is no such index, $r_i := i$. </li></ul><p>Initially, you have an undirected graph with $n$ vertices (numbered from $1$ to $n$) and no edges. Then, for each $i$ from $1$ to $n$, add one edge to the graph: </p><ul> <li> If $s_i =$&nbsp;<span class="tex-font-style-tt">L</span>, add the edge $(i, l_i)$ to the graph. </li><li> If $s_i =$&nbsp;<span class="tex-font-style-tt">R</span>, add the edge $(i, r_i)$ to the graph. </li><li> If $s_i =$&nbsp;<span class="tex-font-style-tt">?</span>, either add the edge $(i, l_i)$ or the edge $(i, r_i)$ to the graph at your choice. </li></ul><p>Find the maximum possible diameter over all <span class="tex-font-style-bf">connected</span>$^{\text{∗}}$ graphs that you can form. Output $-1$ if it is not possible to form any connected graphs.</p><div><p>$^{\text{∗}}$ Let $d(s, t)$ denote the smallest number of edges on any path between $s$ and $t$.</p><p>The diameter of the graph is defined as the maximum value of $d(s, t)$ over all pairs of vertices $s$ and $t$. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$)&nbsp;— the length of the permutation $p$. </p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of $p$, which are guaranteed to form a permutation.</p><p>The third line of each test case contains a string $s$ of length $n$. It is guaranteed that it consists only of the characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum possible diameter over all connected graphs that you form, or $-1$ if it is not possible to form any connected graphs.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$)&nbsp;— the length of the permutation $p$. </p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of $p$, which are guaranteed to form a permutation.</p><p>The third line of each test case contains a string $s$ of length $n$. It is guaranteed that it consists only of the characters <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum possible diameter over all connected graphs that you form, or $-1$ if it is not possible to form any connected graphs.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
8
5
2 1 4 3 5
R?RL?
2
1 2
LR
3
3 1 2
L?R
7
5 3 1 6 4 2 7
?R?R?R?
5
5 2 1 3 4
?????
6
6 2 3 4 5 1
?LLRLL
8
1 7 5 6 2 8 4 3
?R??????
12
6 10 7 1 8 5 12 2 11 3 4 9
????????????
```




```output1
3
-1
-1
4
4
3
5
8
```



## Note

<p>In the first test case, there are two connected graphs (the labels are indices): </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./34768/file/eOITurOx.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="./34768/file/qIVkVm31.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><p>The graph on the left has a diameter of $2$, while the graph on the right has a diameter of $3$, so the answer is $3$.</p><p>In the second test case, there are no connected graphs, so the answer is $-1$.</p>
