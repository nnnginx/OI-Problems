## Description

<div><p>Kristina has an array $a$, called a <span class="tex-font-style-it">template</span>, consisting of $n$ integers. She also has $m$ strings, each consisting only of lowercase Latin letters. The strings are numbered from $1$ to $m$. She wants to check which strings match the template.</p><p>A string $s$ is considered to match the template if all of the following conditions are simultaneously satisfied: </p><ul><li> The length of the string $s$ is equal to the number of elements in the array $a$.</li><li> The same numbers from $a$ correspond to the same symbols from $s$. So, if $a_i = a_j$, then $s_i = s_j$ for ($1 \le i, j \le n$).</li><li> The same symbols from $s$ correspond to the same numbers from $a$. So, if $s_i = s_j$, then $a_i = a_j$ for ($1 \le i, j \le n$).</li></ul> In other words, there must be a one-to-one correspondence between the characters of the string and the elements of the array.<p>For example, if $a$ = [$3, 5, 2, 1, 3$], then the string "<span class="tex-font-style-tt">abfda</span>" matches the template, while the string "<span class="tex-font-style-tt">afbfa</span>" does not, since the character "<span class="tex-font-style-tt">f</span>" corresponds to both numbers $1$ and $5$.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following descriptions are for the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of elements in the array $a$.</p><p>The second line of each test case contains exactly $n$ integers $a_i$ ($-10^9 \le a_i \le 10^9$) ！ the elements of the array $a$.</p><p>The third line of each test case contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$) ！ the number of strings to check for template matching.</p><p>Following are $m$ strings, each containing a non-empty string $s_j$ ($1 \le |s_j| \le 2 \cdot 10^5$), consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$, and that the sum of the lengths of all strings does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $m$ lines. On the $i$-th line ($1 \le i \le m$) output: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if the string with index $i$ matches the template; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You may output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following descriptions are for the test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of elements in the array $a$.</p><p>The second line of each test case contains exactly $n$ integers $a_i$ ($-10^9 \le a_i \le 10^9$) ！ the elements of the array $a$.</p><p>The third line of each test case contains a single integer $m$ ($1 \le m \le 2 \cdot 10^5$) ！ the number of strings to check for template matching.</p><p>Following are $m$ strings, each containing a non-empty string $s_j$ ($1 \le |s_j| \le 2 \cdot 10^5$), consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$, and that the sum of the lengths of all strings does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $m$ lines. On the $i$-th line ($1 \le i \le m$) output: </p><ul> <li> "<span class="tex-font-style-tt">YES</span>", if the string with index $i$ matches the template; </li><li> "<span class="tex-font-style-tt">NO</span>" otherwise. </li></ul><p>You may output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,5,6,13,14,15,16,17,18,19
3
5
3 5 2 1 3
2
abfda
afbfa
2
1 2
3
ab
abc
aa
4
5 -3 5 -3
4
aaaa
bcbc
aba
cbcb
```




```output1
YES
NO
YES
NO
NO
NO
YES
NO
YES
```



## Note

<p>The first test case is explained in the problem statement.</p>
