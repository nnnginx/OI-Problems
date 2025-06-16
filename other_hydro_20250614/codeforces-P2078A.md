## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=xkUN_9HFNPg"><span class="tex-font-style-it">Testify - void (Mournfinale) feat. 星熊南巫</span></a></div><div class="epigraph-source"> </div></div><p>You are given an array $a$ of length $n$, and must perform the following operation until the length of $a$ becomes $1$.</p><p>Choose a positive integer $k &lt; |a|$ such that $\frac{|a|}{k}$ is an integer. Split $a$ into $k$ subsequences$^{\text{∗}}$ $s_1, s_2, \ldots, s_k$ such that:</p><ul> <li> Each element of $a$ belongs to exactly one subsequence.</li><li> The length of every subsequence is equal. </li></ul><p>After this, replace $a = \left[ \operatorname{avg}(s_1), \operatorname{avg}(s_2), \ldots, \operatorname{avg}(s_k) \right] $, where $\operatorname{avg}(s) = \frac{\sum_{i = 1}^{|s|} s_i}{|s|}$ is the average of all the values in the subsequence. For example, $\operatorname{avg}([1, 2, 1, 1]) = \frac{5}{4} = 1.25$.</p><p>Your task is to determine whether there exists a sequence of operations such that after all operations, $a = [x]$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) elements.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \leq n, x \leq 100$) — the length of the array $a$ and the final desired value.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$) — the array $a$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES'</span>" (without quotes) if there exists such a sequence of operations, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output <span class="tex-font-style-tt">"YES"</span> and <span class="tex-font-style-tt">"NO"</span> in any case (for example, strings <span class="tex-font-style-tt">"yES"</span>, <span class="tex-font-style-tt">"yes"</span> and <span class="tex-font-style-tt">"Yes"</span> will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$, $x$ ($1 \leq n, x \leq 100$) — the length of the array $a$ and the final desired value.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$) — the array $a$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES'</span>" (without quotes) if there exists such a sequence of operations, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output <span class="tex-font-style-tt">"YES"</span> and <span class="tex-font-style-tt">"NO"</span> in any case (for example, strings <span class="tex-font-style-tt">"yES"</span>, <span class="tex-font-style-tt">"yes"</span> and <span class="tex-font-style-tt">"Yes"</span> will be recognized as a positive response).</p>





```input1|2,3,6,7
4
1 3
3
4 9
7 11 2 5
6 9
1 9 14 12 10 8
10 10
10 10 10 10 10 10 10 10 10 10
```




```output1
YES
NO
YES
YES
```



## Note

<p>In the first test case, $x = 3$ and $a = [3]$ already holds.</p><p>In the second test case, $x = 9$, and there exists no sequence of operations such that after all operations, $a = [9]$.</p><p>In the third test case, $x = 9$, and here is one possible sequence of operations.</p><ol> <li> $k = 2$, $s_1 = [1, 12, 8]$ and $s_2 = [9, 14, 10]$. Hence, $a = [\operatorname{avg}(s_1), \operatorname{avg}(s_2)] = [7, 11]$.</li><li> $k = 1$ and $s_1 = [7, 11]$. Hence, $a = [\operatorname{avg}(s_1)] = [9]$. </li></ol><p>In the fourth test case, $x = 10$, and here is one possible sequence of operations.</p><ol> <li> $k = 1$ and $s_1 = [10, 10, 10, 10, 10, 10, 10, 10, 10, 10]$. Hence, $a = [\operatorname{avg}(s_1)] = [10]$. </li></ol>
