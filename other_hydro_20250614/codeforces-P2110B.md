## Description

<div><p>In 2077, robots decided to get rid of balanced bracket sequences once and for all!</p><p>A bracket sequence is called <span class="tex-font-style-it">balanced</span> if it can be constructed by the following formal grammar. </p><ol> <li> The empty sequence $\varnothing$ is balanced. </li><li> If the bracket sequence $A$ is balanced, then $\mathtt{(}A\mathtt{)}$ is also balanced. </li><li> If the bracket sequences $A$ and $B$ are balanced, then the concatenated sequence $A B$ is also balanced. </li></ol><p>You are the head of the department for combating balanced bracket sequences, and your main task is to determine which brackets you can destroy and which you cannot.</p><p>You are given a balanced bracket sequence represented by a string $s$, consisting of the characters <span class="tex-font-style-tt">(</span> and <span class="tex-font-style-tt">)</span>. Since the robots' capabilities are not limitless, they can remove <span class="tex-font-style-bf">exactly</span> one opening bracket and <span class="tex-font-style-bf">exactly</span> one closing bracket from the string.</p><p>Your task is to determine whether the robots can delete such two brackets so that the string $s$ is no longer a balanced bracket sequence.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>Each test case consists of a single string $s$ ($2 \leq |s| \leq 2 \cdot 10^5$)&nbsp;¡ª a sequence of the characters <span class="tex-font-style-tt">(</span> and <span class="tex-font-style-tt">)</span>.</p><p>It is guaranteed that $s$ is a balanced bracket sequence.</p><p>It is also guaranteed that the sum of $|s|$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the robots can make the string stop being a balanced bracket sequence, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>Each test case consists of a single string $s$ ($2 \leq |s| \leq 2 \cdot 10^5$)&nbsp;¡ª a sequence of the characters <span class="tex-font-style-tt">(</span> and <span class="tex-font-style-tt">)</span>.</p><p>It is guaranteed that $s$ is a balanced bracket sequence.</p><p>It is also guaranteed that the sum of $|s|$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the robots can make the string stop being a balanced bracket sequence, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,4
4
(())
(())()()
()
(())(())
```




```output1
NO
YES
NO
YES
```



## Note

<p>In the first test case, it can be shown that the robots will not be able to break the correct bracket sequence.</p><p>In the second test case, one of the options for removing brackets is as follows:</p><p>$\texttt{(())}\color{red}{\texttt{(}}\texttt{)(}\color{red}{\texttt{)}} \rightarrow \texttt{(()))(}$, which is not a correct bracket sequence.</p><p>In the fourth test case, one of the options for removal is as follows:</p><p>$\texttt{(}\color{red}{\texttt{(}}\texttt{))((}\color{red}{\texttt{)}}\texttt{)}\rightarrow \texttt{())(()}$, which is not a correct bracket sequence.</p>
