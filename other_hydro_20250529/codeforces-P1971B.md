## Description

<div><p>You are given a string $s$ consisting of lowercase English letters.</p><p>Rearrange the characters of $s$ to form a new string $r$ that is <span class="tex-font-style-bf">not equal</span> to $s$, or report that it's impossible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ of length at most $10$ consisting of lowercase English letters.</p></div><div class="output-specification"><p>For each test case, if no such string $r$ exists as described in the statement, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output one line&nbsp;！ the string $r$, consisting of letters of string $s$.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If multiple answers are possible, you can output any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ of length at most $10$ consisting of lowercase English letters.</p>

## Output

<p>For each test case, if no such string $r$ exists as described in the statement, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output one line&nbsp;！ the string $r$, consisting of letters of string $s$.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If multiple answers are possible, you can output any of them.</p>





```input1|2,4,6,8
8
codeforces
aaaaa
xxxxy
co
d
nutdealer
mwistht
hhhhhhhhhh
```




```output1
YES
forcodesec
NO
YES
xxyxx
YES
oc
NO
YES
undertale
YES
thtsiwm
NO
```



## Note

<p>In the first test case, another possible answer is $\texttt{forcescode}$.</p><p>In the second test case, all rearrangements of $\texttt{aaaaa}$ are equal to $\texttt{aaaaa}$.</p>
