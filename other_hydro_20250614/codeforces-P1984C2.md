## Description

<div><p><span class="tex-font-style-bf">The two versions of the problem are different. You may want to read both versions. You can make hacks only if both versions are solved.</span></p><p>You are given an array $a$ of length $n$. Start with $c = 0$. Then, for each $i$ from $1$ to $n$ (in increasing order) do <span class="tex-font-style-bf">exactly one</span> of the following: </p><ul> <li> Option $1$: set $c$ to $c + a_i$. </li><li> Option $2$: set $c$ to $|c + a_i|$, where $|x|$ is the absolute value of $x$. </li></ul><p>Let the maximum final value of $c$ after the procedure described above be equal to $k$. Find the number of unique procedures that result in $c = k$. Two procedures are different if at any index $i$, one procedure chose option $1$ and another chose option $2$, even if the value of $c$ is equal for both procedures after that turn.</p><p>Since the answer may be large, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of unique procedures that result in $c = k$, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of unique procedures that result in $c = k$, modulo $998\,244\,353$.</p>





```input1|2,3,6,7,10,11
5
4
2 -5 3 -3
8
1 4 3 4 1 4 3 4
3
-1 -2 -3
4
-1000000000 1000000000 1000000000 1000000000
4
1 9 8 4
```




```output1
12
256
1
8
16
```



## Note

<p>In the first test case, it can be shown that our maximal final value of $c$ is $3$. There are $12$ ways to achieve this because in order to get $3$, we have to take absolute value at indices $2$ or $4$, or both, resulting in $3$ ways. For the other two indices, it doesn't change the value whether we take absolute value or not, so we have $2 \cdot 2 = 4$ ways for them. In total, we have $3 \cdot 4 = 12$ ways.</p><p>In the second test case, taking the absolute value will never change anything, so we can either take absolute value or not, for every index. This gives us $2^8 = 256$ possible ways.</p>
