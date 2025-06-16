## Description

<div><p>Turtle thinks a string $s$ is a good string if there exists a sequence of strings $t_1, t_2, \ldots, t_k$ ($k$ is an arbitrary integer) such that:</p><ul> <li> $k \ge 2$. </li><li> $s = t_1 + t_2 + \ldots + t_k$, where $+$ represents the concatenation operation. For example, $\texttt{abc} = \texttt{a} + \texttt{bc}$. </li><li> For all $1 \le i &lt; j \le k$, the first character of $t_i$ <span class="tex-font-style-bf">isn't equal to</span> the last character of $t_j$. </li></ul><p>Turtle is given a string $s$ consisting of lowercase Latin letters. Please tell him whether the string $s$ is a good string!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$) ¡ª the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the string $s$ is a good string, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$) ¡ª the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the string $s$ is a good string, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,6,7
4
2
aa
3
aba
4
abcb
12
abcabcabcabc
```




```output1
No
nO
Yes
YES
```



## Note

<p>In the first test case, the sequence of strings $\texttt{a}, \texttt{a}$ satisfies the condition $s = t_1 + t_2 + \ldots + t_k$, but the first character of $t_1$ is equal to the last character of $t_2$. It can be seen that there doesn't exist any sequence of strings which satisfies all of the conditions, so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the third test case, the sequence of strings $\texttt{ab}, \texttt{cb}$ satisfies all of the conditions.</p><p>In the fourth test case, the sequence of strings $\texttt{abca}, \texttt{bcab}, \texttt{cabc}$ satisfies all of the conditions.</p>
