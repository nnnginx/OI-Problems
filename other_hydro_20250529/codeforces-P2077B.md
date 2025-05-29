## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://www.youtube.com/watch?v=LJEqM7pvClA"><span class="tex-font-style-it">ALTER EGO - Yuta Imai vs Qlarabelle</span></a></div><div class="epigraph-source"> </div></div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>There are two hidden non-negative integers $x$ and $y$ ($0 \leq x, y &lt; 2^{30}$). You can ask no more than $2$ queries of the following form.</p><ul> <li> Pick a non-negative integer $n$ ($0 \leq n &lt; 2^{30}$). The judge will respond with the value of $(n \mathbin{|} x) + (n \mathbin{|} y)$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. </li></ul><p>After this, the judge will give you another non-negative integer $m$ ($0 \leq m &lt; 2^{30}$). You must answer the correct value of $(m \mathbin{|} x) + (m \mathbin{|} y)$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p></div><div><h2>Interaction</h2><p>Two hidden integers $x$ and $y$ are chosen ($0 \leq x, y &lt; 2^{30}$). Note that $x$ and $y$ might be different for different test cases.</p><p>The interactor in this task is <span class="tex-font-style-bf">not adaptive</span>. In other words, the integers $x$ and $y$ do not change during the interaction.</p><p>To ask a query, pick an integer $n$ ($0 \leq n &lt; 2^{30}$) and print only the integer $n$ to a line.</p><p>You will receive a single integer, the value of $(n \mathbin{|} x) + (n \mathbin{|} y)$.</p><p>You may make no more than $2$ queries of the following form.</p><p>After you finish your queries, output "<span class="tex-font-style-tt">!</span>" in a line. You will receive an integer $m$ ($0 \leq m &lt; 2^{30}$). Note that the value of $m$ is also fixed before interaction.</p><p>You must output only the value of $(m \mathbin{|} x) + (m \mathbin{|} y)$ in a line. Note that this line is <span class="tex-font-style-bf">not</span> considered a query and is <span class="tex-font-style-bf">not</span> taken into account when counting the number of queries asked.</p><p>After this, proceed to the next test case.</p><p>If you make more than $2$ queries during an interaction, your program must terminate immediately, and you will receive the Wrong Answer verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>After printing a query do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, follow the test format below.</p><p>The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first and only line of each test case contains a single line with three integers $x, y, m$ ($0 \leq x, y, m &lt; 2^{30}$).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p>





```input1
2

3

4

1

0

1
```




```output1
0

1

!

4

0

!

2
```



## Note

<p>In the first test, the interaction proceeds as follows.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Solution</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Jury</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Explanation</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{2}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">There are 2 test cases.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">In the first test case, $x=1$ and $y=2$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{3}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution requests $(0 \mathbin{|} 1) + (0 \mathbin{|} 2)$, and the jury responds with $3$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{1}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{4}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution requests $(1 \mathbin{|} 1) + (1 \mathbin{|} 2)$, and the jury responds with $4$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{!}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{1}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution requests the value of $m$, and the jury responds with $1$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{4}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution knows that $(1 \mathbin{|} x) + (1 \mathbin{|} y)=4$ because of earlier queries.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">In the second test case, $x=0$ and $y=0$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{0}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution requests $(0 \mathbin{|} 0) + (0 \mathbin{|} 0)$, and the jury responds with $0$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{!}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{1}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution requests the value of $m$, and the jury responds with $1$.</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\texttt{2}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">The solution somehow deduces that $x=y=0$, so it responds with $(1 \mathbin{|} 0) + (1 \mathbin{|} 0)=2$.</td></tr></tbody></table> </center><p>Note that the empty lines in the example input and output are for the sake of clarity and do not occur in the real interaction.</p>
