## Description

<div><p><span class="tex-font-style-bf">Note that the only difference between <span class="tex-font-style-tt">String Transformation 1</span> and <span class="tex-font-style-tt">String Transformation 2</span> is in the move Koa does. In this version the letter $y$ Koa selects must be strictly greater alphabetically than $x$ (read statement for better understanding). You can make hacks in these problems independently.</span></p><p>Koa the Koala has two strings $A$ and $B$ of the same length $n$ ($|A|=|B|=n$) consisting of the first $20$ lowercase English alphabet letters (ie. from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span>).</p><p>In one move Koa:</p><ol><p> </p><li> selects some subset of positions $p_1, p_2, \ldots, p_k$ ($k \ge 1; 1 \le p_i \le n; p_i \neq p_j$ if $i \neq j$) of $A$ such that $A_{p_1} = A_{p_2} = \ldots = A_{p_k} = x$ (ie. all letters on this positions are equal to some letter $x$).<p> </p></li><li> selects a letter $y$ (from the first $20$ lowercase letters in English alphabet) such that $y&gt;x$ (ie. letter $y$ is <span class="tex-font-style-bf">strictly greater</span> alphabetically than $x$).<p> </p></li><li> sets each letter in positions $p_1, p_2, \ldots, p_k$ to letter $y$. More formally: for each $i$ ($1 \le i \le k$) Koa sets $A_{p_i} = y$.<p> <span class="tex-font-style-bf">Note that you can only modify letters in string $A$</span>.</p></li></ol><p>Koa wants to know the smallest number of moves she has to do to make strings equal to each other ($A = B$) or to determine that there is no way to make them equal. Help her!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 10$)&nbsp;�� the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the length of strings $A$ and $B$.</p><p>The second line of each test case contains string $A$ ($|A|=n$).</p><p>The third line of each test case contains string $B$ ($|B|=n$).</p><p>Both strings consists of the first $20$ lowercase English alphabet letters (ie. from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span>).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case:</p><p>Print on a single line the smallest number of moves she has to do to make strings equal to each other ($A = B$) or $-1$ if there is no way to make them equal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 10$)&nbsp;�� the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the length of strings $A$ and $B$.</p><p>The second line of each test case contains string $A$ ($|A|=n$).</p><p>The third line of each test case contains string $B$ ($|B|=n$).</p><p>Both strings consists of the first $20$ lowercase English alphabet letters (ie. from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span>).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case:</p><p>Print on a single line the smallest number of moves she has to do to make strings equal to each other ($A = B$) or $-1$ if there is no way to make them equal.</p>

## Samples

```input1
5
3
aab
bcc
4
cabc
abcb
3
abc
tsr
4
aabd
cccd
5
abcbd
bcdda
```

```output1
2
-1
3
2
-1
```




## Note

<ul> <li> In the $1$-st test case Koa: <ol> <li> selects positions $1$ and $2$ and sets $A_1 = A_2 = $ <span class="tex-font-style-tt">b</span> ($\color{red}{aa}b \rightarrow \color{blue}{bb}b$). </li><li> selects positions $2$ and $3$ and sets $A_2 = A_3 = $ <span class="tex-font-style-tt">c</span> ($b\color{red}{bb} \rightarrow b\color{blue}{cc}$). </li></ol><p> </p></li><li> In the $2$-nd test case Koa has no way to make string $A$ equal $B$.<p> </p></li><li> In the $3$-rd test case Koa: <ol> <li> selects position $1$ and sets $A_1 = $ <span class="tex-font-style-tt">t</span> ($\color{red}{a}bc \rightarrow \color{blue}{t}bc$). </li><li> selects position $2$ and sets $A_2 = $ <span class="tex-font-style-tt">s</span> ($t\color{red}{b}c \rightarrow t\color{blue}{s}c$). </li><li> selects position $3$ and sets $A_3 = $ <span class="tex-font-style-tt">r</span> ($ts\color{red}{c} \rightarrow ts\color{blue}{r}$). </li></ol> </li></ul>
