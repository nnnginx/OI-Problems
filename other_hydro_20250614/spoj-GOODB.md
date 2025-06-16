<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Having arrived at the ACM-ICPC contest site in a fun-filled mood, The Team continues their important pre-contest preparations. Specifically, every world-class team knows the importance of making predictions about their upcoming submissions.</p>
<p>The Team knows that they'll get plenty of AC (Accepted) submissions, and they find those quite boring by now. As such, they'll focus on their incorrect ones. From their vast experience, The Team knows that they'll only get exactly $N$ ($1 \leq N \leq 300$) submissions wrong throughout the upcoming contest - in fact, they predict that, of those, exactly $W$ ($0 \leq W \leq 100$) will get WA (Wrong Answer), $T$ ($0 \leq T \leq 100$) will get TLE (Time Limit Exceeded), and the remaining $R$ ($0 \leq R \leq 100$) will get RE (Runtime Error). Note that $W+T+R=N$.</p>
<p>Assuming that their predictions will certainly be correct, the members of The Team are wondering in how many ways that might occur. In other words, how many different ordered combinations of $N$ incorrect results (each being WA, TLE, or RE) exist which satisfy their predictions? Since The Team doesn't make many mistakes, surely you can calculate this value, right? However, since it can get quite large for you, compute it modulo ($10^9+7$).</p>
<h3>Input</h3>
<p>4 integers, $N$, $W$, $T$, and $R$</p>
<h3>Output</h3>
<p>1 integer, the number of valid ordered combinations of submission results, modulo ($10^9+7$).</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3 2 1 0</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3</span></pre>
<pre><span style="font-weight: bold;">Explanation of Sample:</span></pre>
<p>Out of 3 submissions, two are WA, while the third is TLE. The following 3 ordered combinations are then possible:</p>
<p>WA, WA, TLE</p>
<p>WA, TLE, WA</p>
<p>or</p>
<p>TLE, WA, WA</p>
<p>The answer is then $3$ modulo ($10^9+7$) = $3$.</p>