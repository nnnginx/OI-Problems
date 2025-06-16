## Description

<div><p>Flower gives Gellyfish two permutations$^{\text{∗}}$ of $[0, 1, \ldots, n-1]$: $p_0, p_1, \ldots, p_{n-1}$ and $q_0, q_1, \ldots, q_{n-1}$.</p><p>Now Gellyfish wants to calculate an array $r_0,r_1,\ldots,r_{n-1}$ through the following method: </p><ul><li> For all $i$ ($0 \leq i \leq n-1$), $r_i = \max\limits_{j=0}^{i} \left(2^{p_j} + 2^{q_{i-j}} \right)$ </li></ul><p>But since Gellyfish is very lazy, you have to help her figure out the elements of $r$.</p><p>Since the elements of $r$ are very large, you are only required to output the elements of $r$ modulo $998\,244\,353$.</p><div class="statement-footnote"><p>$^{\text{∗}}$An array $b$ is a permutation of an array $a$ if $b$ consists of the elements of $a$ in arbitrary order. For example, $[4,2,3,4]$ is a permutation of $[3,2,4,4]$ while $[1,2,2]$ is not a permutation of $[1,2,3]$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $p_0, p_1, \ldots,p_{n-1}$ ($0 \leq p_i &lt; n$).</p><p>The third line of each test case contains $n$ integers $q_0, q_1, \ldots,q_{n-1}$ ($0 \leq q_i &lt; n$).</p><p>It is guaranteed that both $p$ and $q$ are permutations of $[0, 1, \ldots, n-1]$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $r_0, r_1, \ldots, r_{n-1}$ in a single line, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $p_0, p_1, \ldots,p_{n-1}$ ($0 \leq p_i &lt; n$).</p><p>The third line of each test case contains $n$ integers $q_0, q_1, \ldots,q_{n-1}$ ($0 \leq q_i &lt; n$).</p><p>It is guaranteed that both $p$ and $q$ are permutations of $[0, 1, \ldots, n-1]$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output $n$ integers $r_0, r_1, \ldots, r_{n-1}$ in a single line, modulo $998\,244\,353$.</p>





```input1|2,3,4,8,9,10
3
3
0 2 1
1 2 0
5
0 1 2 3 4
4 3 2 1 0
10
5 8 9 3 4 0 2 7 1 6
9 5 1 4 0 3 2 8 7 6
```




```output1
3 6 8 
17 18 20 24 32 
544 768 1024 544 528 528 516 640 516 768
```



## Note

<p>In the first test case: </p><ul> <li> $r_0 = 2^{p_0} + 2^{q_0} = 1+2=3$ </li><li> $r_1 = \max(2^{p_0} + 2^{q_1}, 2^{p_1} + 2^{q_0}) = \max(1+4, 4+2) = 6$ </li><li> $r_2 = \max(2^{p_0} + 2^{q_2}, 2^{p_1}+2^{q_1}, 2^{p_2}+2^{q_0}) = (1+1, 4+4, 2+2) = 8$ </li></ul>
