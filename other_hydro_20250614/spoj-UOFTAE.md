<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>You've come across $N$ ($1 \leq N \leq 200$) adorable little Foxlings, and they're hungry! Luckily, you happen to have $M$ ($1 \leq M \leq 200$) crackers on hand, and everyone knows that Foxen love crackers! You'd like to distribute all of your crackers, without splitting any of them, among the Foxlings - but you have to be careful. Foxling $i$ must be fed at least $A_i$ crackers, or it will remain hungry, but no more than $B_i$ of them, or it will become hyper ($1 \leq A_i \leq B_i \leq 200$). You certainly don't want any hungry or hyper Foxlings on your hands, and you're curious as to how many ways this can be accomplished.</p>
<p>There are $T$ ($1 \leq T \leq 100$) scenarios as described above. For each one, you'd like to determine the number of different distributions of your crackers that would satisfy all of the Foxlings, modulo $10^9+7$ (as this value can be quite large).</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 2 integers, $N$ and $M$</p>
<p>Next $N$ lines: 2 integers, $A_i$ and $B_i$, for $i = 1..N$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>Line 1: 1 integer, the number of valid cracker distributions modulo $10^9+7$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>2 5<br>1 4<br>2 6<br>3 5<br>2 2<br>2 9<br>2 3</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3<br>0</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In the first scenario, you can give either 1, 2, or 3 crackers to the first Foxling, and the remaining 4, 3, or 2 (respectively) to the second.</p>
<p>In the second scenario, each Foxling must receive at least 2 crackers, while you only have 5 to give out, so you have no valid options.</p>