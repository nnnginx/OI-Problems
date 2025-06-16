## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">This temple only magnifies the mountain's power.</span></div><div class="epigraph-source">Badeline</div></div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>You are given two positive integers $n$ and $m$ ($\bf{n \le m}$).</p><p>The jury has hidden from you a rectangular matrix $a$ with $n$ rows and $m$ columns, where $a_{i,j} \in \{ -1, 0, 1 \}$ for all $1 \le i \le n$ and $1 \le j \le m$. The jury has also selected a cell $(i_0, j_0)$. Your goal is to find $(i_0,j_0)$.</p><p>In one query, you give a cell $(i, j)$, then the jury will reply with an integer. </p><ul> <li> If $(i, j) = (i_0, j_0)$, the jury will reply with $0$. </li><li> Else, let $S$ be the sum of $a_{x,y}$ over all $x$ and $y$ such that $\min(i, i_0) \le x \le \max(i, i_0)$ and $\min(j, j_0) \le y \le \max(j, j_0)$. Then, the jury will reply with $|i - i_0| + |j - j_0| + |S|$. </li></ul><p>Find $(i_0, j_0)$ by making at most $n + 225$ queries.</p><p><span class="tex-font-style-bf">Note: the grader is not adaptive</span>: $a$ and $(i_0,j_0)$ are fixed before any queries are made.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 50$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 5000$)&nbsp;！ the numbers of rows and the number of columns of the hidden matrix $a$ respectively.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $25 \cdot 10^6$.</p></div><div><h2>Interaction</h2><p>The interaction for each test case begins by reading the integers $n$ and $m$.</p><p>To make a query, output <span class="tex-font-style-tt">"? i j"</span> ($1 \le i \le n, 1 \le j \le m$) without quotes. Afterwards, you should read one single integer&nbsp;！ the answer to your query.</p><p>If you receive the integer $-1$ instead of an answer or a valid value of $n$ or $m$, it means your program has made an invalid query, has exceeded the limit of queries, or has given an incorrect answer on the previous test case. Your program must terminate immediately to receive a Wrong Answer verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>When you are ready to give the final answer, output <span class="tex-font-style-tt">"! i j"</span> ($1 \le i \le n, 1 \le j \le m$) without quotes&nbsp;！ the indices of the hidden cell. After solving a test case, your program should move to the next one immediately. After solving all test cases, your program should be terminated immediately.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format:</p><p>The first line contains an integer $t$ ($1 \le t \le 50$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 5000$)&nbsp;！ the sizes of the hidden matrix.</p><p>The second line of each test case contains two integers $i_0$ and $j_0$ ($1 \le i_0 \le n, 1 \le j_0 \le m$)&nbsp;！ the hidden cell.</p><p>Then $n$ lines follow. The $i$-th of them contains the string $s_i$ of length $n$, consisting only of the characters <span class="tex-font-style-tt">-</span>, <span class="tex-font-style-tt">0</span>, and <span class="tex-font-style-tt">+</span>. Here, $a_{ij} = -1$ if $s_{ij} = \mathtt{-}$, $a_{ij} = 0$ if $s_{ij} = \mathtt{0}$, and $a_{ij} = 1$ if $s_{ij} = \mathtt{+}$.</p><p>The sum of $n \cdot m$ over all test cases should not exceed $25 \cdot 10^6$.</p><p>As an example, the hack format for the example input is:</p><p>$\texttt{2}\\ \texttt{3}\,\texttt{4} \\ \texttt{1}\,\texttt{4} \\ \texttt{+0+0} \\ \texttt{+00+} \\ \texttt{0---} \\ \texttt{1}\,\texttt{1}\\\texttt{1}\,\texttt{1}\\\texttt{0}$</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 50$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 5000$)&nbsp;！ the numbers of rows and the number of columns of the hidden matrix $a$ respectively.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $25 \cdot 10^6$.</p>





```input1
2
3 4

5

3

5

1 1

0
```




```output1
? 1 1

? 3 3

? 3 2

! 1 4

? 1 1

! 1 1
```



## Note

<p>The hidden matrix in the first test case: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}{\textbf{0}}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$-1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$-1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$-1$</td></tr></tbody></table><p></p><p>The hidden matrix in the second test case: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\color{red}{\textbf{0}}$</td></tr></tbody></table><p></p><p>Note that the line breaks in the example input and output are for the sake of clarity, and do not occur in the real interaction.</p>
