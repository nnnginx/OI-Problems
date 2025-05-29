<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>There are $N$ ($1 \leq N \leq 4$) Foxen guarding a certain valuable treasure, which you'd love to get your hands on. The problem is, the Foxen certainly aren't about to allow that - at least, not while they're awake.</p>
<p>Fortunately, through careful observation, you've seen that each Fox has a regular sleep cycle. In particular, the $i$th Fox stays awake for $A_i$ ($1 \leq A_i \leq 23$) hours, then sleeps for $S_i$ ($1 \leq S_i \leq 23$) hours, repeating this pattern indefinitely ($2 \leq A_i+S_i \leq 24$). At the start of your treasure-nabbing attempt, the $i$th Fox is exactly $O_i$ ($0 \leq O_i &lt; A_i+S_i$) hours into its cycle.</p>
<p>There are $T$ ($1 \leq T \leq 20$) scenarios as described above. For each one, you'd like to determine how soon all of the Foxen will be simultaneously asleep, allowing you to grab their treasure, or if this will simply never happen.</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 1 integer, $N$</p>
<p>Next $N$ lines: 3 integers, $A_i$, $S_i$, and $O_i$, for $i = 1..N$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>1 integer, the minimum number of hours after the start to wait until all of the Foxen are asleep during the same hour. If this will never happen, output the string "Foxen are too powerful" (without quotes) instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>2<br>2 1 2<br>2 2 1<br>3<br>1 1 0<br>1 1 0<br>1 1 1</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">6<br>Foxen are too powerful</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In scenario 1, the following table illustrates the Foxen's sleeping cycles (with A representing being awake, S representing sleep, and a bold letter representing the start of a sleep cycle):</p>
<p><img src="../../../content/sourspinach:uoftab.bmp" alt=""></p>
<p>As can be seen, the first hour during which both Foxen are asleep is 6 hours after the start.</p>
<p>In scenario 2, the first 2 Foxen are always awake and asleep at the same times. However, the third Fox's schedule is exactly flipped, which means that it will never be asleep at the same time as the others.</p>