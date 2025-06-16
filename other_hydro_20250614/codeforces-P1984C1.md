## Description

<div><p><span class="tex-font-style-bf">The two versions of the problem are different. You may want to read both versions. You can make hacks only if both versions are solved.</span></p><p>You are given an array $a$ of length $n$. Start with $c = 0$. Then, for each $i$ from $1$ to $n$ (in increasing order) do <span class="tex-font-style-bf">exactly one</span> of the following: </p><ul> <li> Option $1$: set $c$ to $c + a_i$. </li><li> Option $2$: set $c$ to $|c + a_i|$, where $|x|$ is the absolute value of $x$. </li></ul><p>Let the maximum final value of $c$ after the procedure described above be equal to $k$. Find $k$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each case contains $n$ integers $a_1$, $a_2$, $a_3$, $\ldots$, $a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the value of $k$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 2 \cdot 10^5$).</p><p>The second line of each case contains $n$ integers $a_1$, $a_2$, $a_3$, $\ldots$, $a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>The sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the value of $k$.</p>





```input1|2,3,6,7,10,11
5
4
10 -9 -3 4
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
6
24
6
4000000000
22
```



## Note

<p>In the first test case, if we set $c$ to its absolute value every time we add to it, we end up with $6$. It can be shown that this is the maximum result.</p><p>In the second test case, taking the absolute value will never change anything, so we can just sum the array without doing anything to get $24$.</p><p>In the third test case, it is optimal to wait until the end to set $c$ to its absolute value, resulting in an answer of $6$.</p>
