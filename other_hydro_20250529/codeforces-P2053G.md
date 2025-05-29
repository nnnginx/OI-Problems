## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">And I will: love the world that you've adored; wish the smile that you've longed for. Your hand in mine as we explore, please take me to tomorrow's shore. </span></div><div class="epigraph-source">！ Faye Wong, <a href="https://www.youtube.com/watch?v=ZoJCN0pV7Qs"><span class="tex-font-style-it">As Wished</span></a></div></div><p>Cocoly has a string $t$ of length $m$, consisting of lowercase English letters, and he would like to split it into parts. He calls a pair of strings $(x, y)$ <span class="tex-font-style-it">beautiful</span> if and only if there exists a sequence of strings $a_1, a_2, \ldots, a_k$, such that:</p><ul> <li> $t = a_1 + a_2 + \ldots + a_k$, where $+$ denotes string concatenation. </li><li> For each $1 \leq i \leq k$, at least one of the following holds: $a_i = x$, or $a_i = y$. </li></ul><p>Cocoly has another string $s$ of length $n$, consisting of lowercase English letters. Now, for each $1 \leq i &lt; n$, Cocoly wants you to determine whether the pair of strings $(s_1s_2 \ldots s_i, \, s_{i+1}s_{i+2} \ldots s_n)$ is <span class="tex-font-style-it">beautiful</span>.</p><p><span class="tex-font-style-bf">Note</span>: since the input and output are large, you may need to optimize them for this problem.</p><p>For example, in C++, it is enough to use the following lines at the start of the <span class="tex-font-style-it">main()</span> function:</p><pre class="lstlisting"><code class="prettyprint">int main() {<br>    std::ios::sync_with_stdio(false);<br>    std::cin.tie(nullptr); std::cout.tie(nullptr);<br>}<br></code></pre></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $T$ ($1 \leq T \leq 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq m \leq 5 \cdot 10^6$)&nbsp;！ the lengths of $s$ and the length of $t$.</p><p>The second line of each test case contains a single string $s$ of length $n$, consisting only of lowercase English letters.</p><p>The third line of each test case contains a single string $t$ of length $m$, consisting only of lowercase English letters.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^7$.</p></div><div class="output-specification"><p>For each test case, output a single binary string $r$ of length $n - 1$: for each $1 \leq i &lt; n$, if the $i$-th pair is beautiful, $r_i=\texttt{1}$; otherwise, $r_i=\texttt{0}$. Do not output spaces.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $T$ ($1 \leq T \leq 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq m \leq 5 \cdot 10^6$)&nbsp;！ the lengths of $s$ and the length of $t$.</p><p>The second line of each test case contains a single string $s$ of length $n$, consisting only of lowercase English letters.</p><p>The third line of each test case contains a single string $t$ of length $m$, consisting only of lowercase English letters.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^7$.</p>

## Output

<p>For each test case, output a single binary string $r$ of length $n - 1$: for each $1 \leq i &lt; n$, if the $i$-th pair is beautiful, $r_i=\texttt{1}$; otherwise, $r_i=\texttt{0}$. Do not output spaces.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
3 5
aba
ababa
4 10
czzz
czzzzzczzz
5 14
dream
dredreamamamam
5 18
tcccc
tcctccccctccctcccc
7 11
abababc
abababababc
7 26
aaaaaaa
aaaaaaaaaaaaaaaaaaaaaaaaaa
19 29
bbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbb
```




```output1
11
011
0010
0000
010100
111111
110010001100010011
```



## Note

<p>In the first test case, $s = \tt aba$, $t = \tt ababa$.</p><ul> <li> For $i = 1$: Cocoly can split $t = \texttt{a} + \texttt{ba} + \texttt{ba}$, so the string pair $(\texttt{a}, \texttt{ba})$ is <span class="tex-font-style-it">beautiful</span>. </li><li> For $i = 2$: Cocoly can split $t = \texttt{ab} + \texttt{ab} + \texttt{a}$, so the string pair $(\texttt{ab}, \texttt{a})$ is <span class="tex-font-style-it">beautiful</span>. </li></ul><p>In the second test case, $s = \tt czzz$, $t = \tt czzzzzczzz$.</p><ul> <li> For $i = 1$: It can be proven that there is no solution to give a partition of $t$ using strings $\texttt{c}$ and $\texttt{zzz}$. </li><li> For $i = 2$: Cocoly can split $t$ into $\texttt{cz} + \texttt{zz} + \texttt{zz} + \texttt{cz} + \texttt{zz}$. </li><li> For $i = 3$: Cocoly can split $t$ into $\texttt{czz} + \texttt{z} + \texttt{z} + \texttt{z} + \texttt{czz} + \texttt{z}$. </li></ul>
