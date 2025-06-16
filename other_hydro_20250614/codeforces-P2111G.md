## Description

<div><p><span class="tex-font-style-bf">Technically, this is an interactive problem.</span></p><p>An array $a$ of $m$ numbers is called <span class="tex-font-style-it">divisible</span> if at least one of the following conditions holds:</p><ul> <li> There exists an index $i$ ($1 \le i &lt; m$) and an integer $x$ such that for all indices $j$ ($j \le i$), it holds that $a_{j} \le x$ and for all indices $k$ ($k &gt; i$), it holds that $a_{k} &gt; x$. </li><li> There exists an index $i$ ($1 \le i &lt; m$) and an integer $x$ such that for all indices $j$ ($j \le i$), it holds that $a_{j} &gt; x$ and for all indices $k$ ($k &gt; i$), it holds that $a_{k} \le x$. </li></ul><p>You are given a permutation $p$ of integers $1, 2, \dots, n$. Your task is to answer queries of the following form fast: if we take only the segment [$l$, $r$] from the permutation, that is, the numbers $p_{l}, p_{l + 1}, \dots, p_{r}$, is this subarray of numbers <span class="tex-font-style-it">divisible</span>?</p><p>Queries will be submitted in interactive mode in groups of $10$, meaning you will not receive the next group of queries until you output all answers for the current group.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^{5}$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $p_{i}$ ($1 \le p_{i} \le n$)&nbsp;— the permutation of natural numbers itself.</p><p>The third line contains one integer $q$ ($10 \le q \le 10^{6}, q \bmod 10 = 0$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \le l &lt; r \le n$)&nbsp;— the parameters of the query.</p></div><div class="output-specification"><p>For each query, output the string "<span class="tex-font-style-tt">YES</span>" if the subarray from this query is <span class="tex-font-style-it">divisible</span> and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>After printing the answers to a group of queries, do not forget to output the end of line and flush the output buffer. Otherwise, you may get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict. To flush the buffer, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in <span class="tex-font-style-tt">C++</span>; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in <span class="tex-font-style-tt">Java</span>; </li><li> <span class="tex-font-style-tt">flush(output)</span> in <span class="tex-font-style-tt">Pascal</span>; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in <span class="tex-font-style-tt">Python</span>; </li><li> refer to the documentation for other languages. </li></ul><p>You have to flush the output buffer after the $10$-th, $20$-th, $30$-th query (and so on), i. e. after each query with index divisible by $10$. After that, you can read the next group of queries.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^{5}$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $p_{i}$ ($1 \le p_{i} \le n$)&nbsp;— the permutation of natural numbers itself.</p><p>The third line contains one integer $q$ ($10 \le q \le 10^{6}, q \bmod 10 = 0$)&nbsp;— the number of queries.</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \le l &lt; r \le n$)&nbsp;— the parameters of the query.</p>

## Output

<p>For each query, output the string "<span class="tex-font-style-tt">YES</span>" if the subarray from this query is <span class="tex-font-style-it">divisible</span> and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>After printing the answers to a group of queries, do not forget to output the end of line and flush the output buffer. Otherwise, you may get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict. To flush the buffer, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in <span class="tex-font-style-tt">C++</span>; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in <span class="tex-font-style-tt">Java</span>; </li><li> <span class="tex-font-style-tt">flush(output)</span> in <span class="tex-font-style-tt">Pascal</span>; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in <span class="tex-font-style-tt">Python</span>; </li><li> refer to the documentation for other languages. </li></ul><p>You have to flush the output buffer after the $10$-th, $20$-th, $30$-th query (and so on), i. e. after each query with index divisible by $10$. After that, you can read the next group of queries.</p>





```input1|
7
4 2 3 6 1 5 7
20
1 2
1 3
1 4
1 5
1 6
2 3
2 4
2 5
2 6
3 4
3 5
3 6
4 5
4 6
5 6
1 7
2 7
3 7
4 7
5 7
```




```output1
YES
YES
YES
YES
NO
YES
YES
YES
NO
YES
YES
NO
YES
YES
YES
YES
YES
YES
YES
YES
```


