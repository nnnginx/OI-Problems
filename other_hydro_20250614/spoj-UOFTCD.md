<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Bob is taking Alice out for an evening at the movies! He'll be deciding what movies they see, of course, and he's got $N$ ($1 \leq N \leq 100$) awesome ones in mind. All of them happen to be horror movies.</p>
<p>A given movie is $D$ ($1 \leq D \leq 10^9$) minutes long, and has $M$ ($0 \leq M \leq 100$) key moments. The $i$th moment occurs $T_i$ minutes into the movie, and causes Alice's fright level (which starts at 0) to instantly increase by $F_i$ ($-10^6 \leq F_i \leq 10^6$). If her fright level would become negative, it instead becomes 0. The moments are given in chronological order, so $0 \leq T_1 &lt; T_2 &lt; \dots &lt; T_M \leq D$. As soon as the movie ends, Alice's fright level is instantly reset to 0.</p>
<p>During each movie, Alice has two fright thresholds, $H$ and $L$ ($1 \leq H &lt; L \leq 10^9$). Whenever her fright level is at least $H$, Bob is obligated to hold her hand. However, as soon as her fright level is at least $L$, she'll be scared enough to leave the theatre - at which point, Bob will stay inside and finish the movie, and will of course no longer need to hold her hand.</p>
<p>Bob enjoys brilliant films such as Night of the Dead Living and Return of the Revenge of the Attack of the Killer Foxen, and he'd prefer to not be distracted. As such, he'd like to minimize the amount of time he spends holding Alice's hand. To help with this, he may choose to cover her eyes during at most one key moment in each movie. Alice's fright level will be unaffected by this key moment.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $N$</p>
<p><strong>For each movie:</strong></p>
<p>Line 1: 4 integers, $D$, $M$, $H$, and $L$</p>
<p>Next $M$ lines: 2 integers, $T_i$ and $F_i$, for $i=1..M$</p>
<h3>Output</h3>
<p><strong>For each movie:</strong></p>
<p>1 integer, the minimal number of minutes for which Bob needs to hold Alice's hand</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>90 5 5 50<br>12 8<br>14 -4<br>40 6<br>45 11<br>73 -50<br>105 3 5 20<br>33 15<br>39 -1<br>52 5</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">30<br>19</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>While watching the first movie, Bob should cover Alice's eyes during the third key moment. With this strategy, Alice's fright level will be at least 5 between moments 1 and 2, and between moments 4 and 5. Therefore, Bob will need to hold her hand for $2+28=30$ minutes.</p>
<p>While watching the second movie, Bob should cover Alice's eyes during the second moment. He will then need to hold her hand between moments 1 and 3, at which point her fright level will become 20, and she'll have to leave the theatre.</p>