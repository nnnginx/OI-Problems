<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Alice has received an invitation from Bob to watch some TV on $D$ ($1 \leq D \leq 100$) days! Though spending time with him is nice, she's more concerned about exactly what channels they'll be watching. After all, being a guy, Bob is sure to be interested in viewing less sophisticated programs than she is.</p>
<p>On each day, a different set of $N$ ($1 \leq N \leq 100,000$) channels are available, numbered $1..N$. Each channel $i$ has a girliness value of $G_i$ ($0 \leq G_i \leq 10^9$) associated with it, indicating how much Alice would like to watch it. When she arrives at Bob's house, the TV is set to channel 1, but she'd like to surf to a channel with maximal girliness, and as quickly as possible.</p>
<p>Alice wants to be subtle about her channel surfing, however. She believes that Bob may notice if they stay on any channel for less than $T$ ($1 \leq T \leq 1000$) seconds before switching, or if the girliness value of the new channel is more than $C$ ($1 \leq C \leq 10^9$) greater than that of the current one. She needs a plan of action to maximize the girliness of the channel they end up watching, while minimizing the amount of time it'll take her to surf to such a channel.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $D$</p>
<p><strong>For each day:</strong></p>
<p>Line 1: 3 integers, $N$, $C$, and $T$</p>
<p>Line 2: $N$ integers, $G_{1..N}$</p>
<h3>Output</h3>
<p><strong>For each day:</strong></p>
<p>2 integers, the maximum channel girliness which Alice can surf to, and the minimum number of seconds required to arrive at a channel with this girliness, respectively</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>6 3 5<br>3 4 0 8 12 6<br>4 1 2<br>5 7 7 5</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">8 10<br>5 0</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>On the first day, Alice should switch to channel 6 after 5 seconds, and to channel 4 after another 5 seconds.</p>
<p>On the second day, Alice can't surf to either channel 2 or 3, so she should stay on channel 1.</p>