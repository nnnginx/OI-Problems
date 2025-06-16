<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p> We consider 2D arrays $A$, (0,0)-indexed, shape $N \times M$. <br>
 With $ 0 \le i &lt; N $   and  $ 0 \le j &lt; M $, we have $ 0&lt; A_{i,j} \le N \times M $.
<br>

Our interest will be to count those arrays that have the two properties : <br>
 </p><ul>
  <li>Arrays $A$ are composed with <strong>all</strong> numbers from $1$ to $N \times M$.<br>
i.e. we have $ (i,j) \neq (k,l) \implies A_{i,j} \neq A_{k,l} $</li>
  <li>$(i\oplus j) &gt; (k\oplus l) \implies A_{i,j} &gt; A_{k,l} $, where $ \oplus $ denotes bitwise XOR.</li>
</ul> 


<h3>Input</h3>
<p>The first line contains $T$, the number of test cases, and $P$ a prime number.</p>
<p>Each of the next $T$ lines contains $N$ and $M$, the shape of the arrays $A$. </p>

<h3>Output</h3>
<p>For each test case, print the number of arrays $A$ with the given properties.<br>
As the result may be large, the answer <strong>modulo</strong> $P$ is required.

</p><h3>Example</h3>
<pre><b>Input:</b>
2 1000000007
2 2
997 799

<b>Output:</b>
4
828630475
</pre>
<p>For the first case, the 4 possible 2x2 arrays are : 
$ \binom{1\; 3}{4\; 2}$, $\binom{1\; 4}{3\; 2}$, $\binom{2\; 3}{4\; 1}$, and $\binom{2\; 4}{3\; 1}$. </p>

<h3>Constraints</h3>
<p> $1 \le T \le 10^4$, <br>
$10^9 &lt; P &lt; 2\times 10^9$, a prime number, <br>
$1 \le N \le 10^9$, <br>
$1 \le M \le 10^5$. </p>
<p> Constraints allow a small kB of unoptimized PY3.4 code to get AC in the third of the TL. <strong>Have fun.</strong></p>