<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>It's time for the members of The Team to do what they do best - coding! Faster than you can say "Dijkstra", they've already produced an elegant piece of work. The program has $N$ ($1 \leq N \leq 10^6$) lines of code (conveniently numbered $1..N$), and just one integer variable, $c$, which starts with a value of 0. The program starts executing at line 1, and every line $i$ contains one of the following:</p>
<p>&nbsp; &nbsp;1. "c++;" - The value of $c$ is incremented by 1. Then, if $i=N$, the program terminates - otherwise, the program moves to line $i+1$.</p>
<p>&nbsp; &nbsp;2. "x:" - This line contains the label $x$, where $x$ is an integer such that $1 \leq x \leq 10^6$. No value of $x$ will appear as a label more than once in the program. If $i=N$, the program terminates - otherwise, the program moves to line $i+1$.</p>
<p>&nbsp; &nbsp;3. "goto x;" - The program jumps to the single line that contains the label $x$, where $x$ is an integer such that $1 \leq x \leq 10^6$. It is guaranteed that, for every such line, the corresponding label will exist in the program.</p>
<p>Now, even though this program is glorious, its creators are wondering if it's quite correct. In particular, they know that $c$ should ideally reach a value of $M$ ($1 \leq M \leq 10^{12}$), but they're not sure when. If the program terminates with $c&lt;M$, then certainly there's an issue, and the program should get a WA (Wrong Answer). If the program will never terminate, and $c$ will never reach a value of $M$, then that's also no good, and can be considered a TLE (Time Limit Exceeded). In all other cases, however, The Team would like to know exactly on which line $c$ will first attain a value of $M$. Naturally, having written the program, they instantly realized this already. But can you?</p>
<p><span style="font-size: 1.17em;"><strong>Input</strong></span></p>
<p>First line: 2 integers, $N$ and $M$</p>
<p>Next $N$ lines: The $i$th line of the program (as described above), for $i=1..N$</p>
<p><span style="font-size: 1.17em;"><strong>Output</strong></span></p>
<p>Either 1 integer, the number of the line on which $c$ will first reach a value of $M$, or the string "WA" if the program terminates with $c&lt;M$, or the string "TLE" if the program runs forever with $c&lt;M$.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">12 4
c++;
goto 6;
18:
c++;
c++;
goto 2;
goto 6;
6:
goto 18;
2:
c++;
c++;</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">11</span><span style="white-space: normal;">&nbsp;</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The program will run through the following lines, and corresponding values of $c$:</p>
<p>Line 1 ("c++;"), $c=1$</p>
<p>Line 2 ("goto 6;"), $c=1$</p>
<p>Line 8 ("6:"), $c=1$</p>
<p>Line 9 ("goto 18;"), $c=1$</p>
<p>Line 3 ("18:"), $c=1$</p>
<p>Line 4 ("c++;"), $c=2$</p>
<p>Line 5 ("c++;"), $c=3$</p>
<p>Line 6 ("goto 2;"), $c=3$</p>
<p>Line 10 ("2:"), $c=3$</p>
<p>Line 11 ("c++;"), $c=4$</p>
<p>As can be seen, $c$ first achieves a value of $M=4$ on line 11.</p>