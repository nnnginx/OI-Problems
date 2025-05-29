## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>You are a proud teacher at the Millennium Science School. Today, a student named Alice challenges you to a guessing game.</p><p>Alice is thinking of an integer from $1$ to $n$, and you must guess it by asking her some queries.</p><p>To make things harder, she says you must <span class="tex-font-style-bf">ask all the queries first</span>, and she will <span class="tex-font-style-bf">ignore</span> exactly $1$ query.</p><p>For each query, you choose an array of $k$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $n$, where $k$ is even. Then, Alice will respond with one of the following:</p><ul><li> $\texttt{L}$: the number is one of the first $\frac{k}{2}$ elements of the array; </li><li> $\texttt{R}$: the number is one of the last $\frac{k}{2}$ elements of the array; </li><li> $\texttt{N}$: the number is not in the array; </li><li> $\texttt{?}$: this query is ignored.</li></ul><p>Alice is impatient, so you must find a strategy that <span class="tex-font-style-bf">minimizes</span> the number of queries. Can you do it?</p><p>Formally, let $f(n)$ be the minimum number of queries required to determine Alice's number. Then you must find a strategy that uses <span class="tex-font-style-bf">exactly</span> $f(n)$ queries.</p><p>Note that the interactor is <span class="tex-font-style-bf">adaptive</span>, which means Alice's number is not fixed at the beginning and may depend on your queries. However, it is guaranteed that there exists at least one number that is consistent with Alice's responses.</p><p>We can show that $f(n) \leq 20$ for all $n$ such that $2 \le n \le 2 \cdot 10^5$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the maximum possible value of Alice's number.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div><h2>Interaction</h2><p>The interaction begins by reading the integer $n$.</p><p>Then, output a single integer $q$ ($1 \leq q \leq 20$)&nbsp;！ the number of queries.</p><p>To ask a query, output a line in the following format:</p><ul><li> $k\,a_1\,a_2 \ldots a_k$ ($2 \leq k \leq n$, $k$ is even, $1 \leq a_i \leq n$, the $a_i$ are distinct)&nbsp;！ the length of the array, and the array itself. </li></ul><p>Once you've asked all $q$ queries, read a string $s$ ($|s| = q$)&nbsp;！ the responses to the queries as described above.</p><p>When you know Alice's number, output a single integer $x$ ($1 \leq x \leq n$)&nbsp;！ the value of the number.</p><p>Then, move on to the next test case, or terminate the program if there are no more test cases.</p><p>After outputting all $q$ queries, do not forget to output the end of the line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> See the documentation for other languages. </li></ul><p>Note that even if you correctly determine Alice's number but use more than $f(n)$ queries, you will get <span class="tex-font-style-tt">Wrong answer</span>.</p><p><span class="tex-font-style-bf">For this problem, hacks are disabled.</span></p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The only line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the maximum possible value of Alice's number.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>





```input1
2
3



?N

5




R?L
```




```output1
2
2 1 2
2 1 2

3

3
4 3 2 4 1
4 5 4 3 1
4 1 5 3 4

1
```



## Note

<p>In the first test case, $n = 3$. We ask $2$ queries: $[1, 2]$, and $[1, 2]$ again.</p><ul><li> For the first query, Alice's response is $\texttt{?}$, which means this query is ignored.</li><li> For the second query, Alice's response is $\texttt{N}$, which means her number is not in the array $[1, 2]$.</li></ul><p>From the information above, we can determine that Alice's number is $3$.</p><p>It can be shown that all valid strategies for $n = 3$ require at least $2$ queries.</p><p>In the second test case, $n = 5$. We ask $3$ queries: $[3, 2, 4, 1]$, $[5, 4, 3, 1]$, and $[1, 5, 3, 4]$.</p><ul> <li> For the first query, Alice's response is $\texttt{R}$, which means her number is in the array $[4, 1]$.</li><li> For the second query, Alice's response is $\texttt{?}$, which means this query is ignored.</li><li> For the third query, Alice's response is $\texttt{L}$, which means her number is in the array $[1, 5]$. </li></ul><p>From the information above, we can determine that Alice's number is $1$.</p><p>It can be shown that all valid strategies for $n = 5$ require at least $3$ queries.</p>
