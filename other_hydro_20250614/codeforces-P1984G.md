## Description

<div><p>The secret behind Oscar's first magic trick has been revealed! Because he still wants to impress Lura, he comes up with a new idea: he still wants to sort a permutation $p_1, p_2, \ldots, p_n$ of $[1, 2, \ldots, n]$.</p><p>This time, he chooses an integer $k$. He wants to sort the permutation in non-decreasing order using the following operation several times: </p><ol> <li> Pick a continuous subarray of length $k$ and remove it from $p$. </li><li> Insert the continuous subarray back into $p$ at any position (perhaps, in the very front or the very back). </li></ol><p>To be as impressive as possible, Oscar would like to choose the maximal value of $k$ such that he can sort his permutation. Please help him find the maximal $k$ as well as a sequence of operations that will sort the permutation. You don't need to minimize the number of operations, but you are allowed to use at most $5n^2$ operations.</p><p>We have a proof that, for the maximal $k$ such that you can sort the permutation in any number of operations, you can also sort it in at most $5n^2$ operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($5 \leq n \leq 10^3$)&nbsp;！ the length of the permutation.</p><p>The second line of each test case contains a permutation $p_1, p_2, \ldots, p_n$ of $[1, 2, \ldots, n]$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^3$.</p></div><div class="output-specification"><p>For each test case, first output the chosen value of $k$ on a new line ($1 \leq k \leq n$).</p><p>Then, output a single integer $m$&nbsp;！ the number of operations used ($0 \leq m \leq 5n^2$).</p><p>Then, on each of the next $m$ lines, output the operations denoted by two integers $i$ and $j$ ($1 \leq i, j \leq n - k + 1$), representing an operation where you remove the subarray starting from index $i$ and replace it back into $p$ at index $j$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($5 \leq n \leq 10^3$)&nbsp;！ the length of the permutation.</p><p>The second line of each test case contains a permutation $p_1, p_2, \ldots, p_n$ of $[1, 2, \ldots, n]$.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot 10^3$.</p>

## Output

<p>For each test case, first output the chosen value of $k$ on a new line ($1 \leq k \leq n$).</p><p>Then, output a single integer $m$&nbsp;！ the number of operations used ($0 \leq m \leq 5n^2$).</p><p>Then, on each of the next $m$ lines, output the operations denoted by two integers $i$ and $j$ ($1 \leq i, j \leq n - k + 1$), representing an operation where you remove the subarray starting from index $i$ and replace it back into $p$ at index $j$.</p>





```input1|2,3,6,7
3
5
5 1 2 3 4
5
2 3 5 4 1
6
1 2 3 4 5 6
```




```output1
4
1
2 1
3
2
1 3
2 1
6
0
```



## Note

<p>In the first test case, it is enough to move the last four numbers to the front.</p><p>In the second test case, it can be shown that we cannot have $k = 4$ or $k = 5$. With $k = 3$, we can move the first three numbers to the end, and then the middle three to the front to sort the permutation.</p><p>In the third test case, the permutation is already sorted. We can have $k = 6$ and use no operations.</p>
