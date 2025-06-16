## Description

<div><p>A shrink operation on an array $a$ of size $m$ is defined as follows:</p><ul> <li> Choose an index $i$ ($2 \le i \le m - 1$) such that $a_i \gt a_{i - 1}$ and $a_i \gt a_{i + 1}$. </li><li> Remove $a_i$ from the array. </li></ul><p>Define the <span class="tex-font-style-it">score</span> of a permutation$^{\text{∗}}$ $p$ as the <span class="tex-font-style-it">maximum</span> number of times that you can perform the shrink operation on $p$.</p><p>Yousef has given you a single integer $n$. Construct a permutation $p$ of length $n$ with the <span class="tex-font-style-bf">maximum</span> possible <span class="tex-font-style-it">score</span>. If there are multiple answers, you can output any of them.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the size of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output any permutation $p_1, p_2, \dots, p_n$ that maximizes the number of shrink operations.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the size of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output any permutation $p_1, p_2, \dots, p_n$ that maximizes the number of shrink operations.</p>





```input1|2
2
3
6
```




```output1
1 3 2
2 3 6 4 5 1
```



## Note

<p>In the first test case: </p><ul> <li> We choose $p = [1, 3, 2]$. </li><li> Choose index $2$, and remove $p_2$ from the array. The array becomes $p = [1, 2]$. </li></ul><p>It can be shown that the maximum number of operations we can perform is $1$. Another valid answer is $p = [2, 3, 1]$.</p><p>In the second test case:</p><ul> <li> We choose $p = [2, 3, 6, 4, 5, 1]$. </li><li> Choose index $5$, and remove $p_5$ from the array. The array becomes $p = [2, 3, 6, 4, 1]$. </li><li> Choose index $3$, and remove $p_3$ from the array. The array becomes $p = [2, 3, 4, 1]$. </li><li> Choose index $3$, and remove $p_3$ from the array. The array becomes $p = [2, 3, 1]$. </li><li> Choose index $2$, and remove $p_2$ from the array. The array becomes $p = [2, 1]$. </li></ul><p>The maximum number of operations we can perform is $4$. Any permutation with a score of $4$ is valid.</p>
