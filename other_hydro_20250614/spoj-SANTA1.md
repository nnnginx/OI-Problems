<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>With the presents all crafted and packed into Santa's sack, it's almost time for his annual trip across the world, spreading cheer to all! However, he's first taking the time to experiment with various combinations of reindeer to pull his sleigh. For a successful journey, they'll have to work productively!</p>
<p>Every reindeer has a unique name (a string of up to 20 case-sensitive letters), as well as a seniority and a productivity value (both positive integers no larger than $10^6$). When a group of reindeer is chosen to pull the sleigh, they line up in single file, always in descending order of seniority from the front. If multiple reindeer have the same seniority, they line up in descending order of productivity within themselves (no two reindeer have both the same seniority and the same productivity). The productivity of a pair of adjacent reindeer in the lineup is the product of their individual productivity values, and the total productivity of the lineup is the sum of all such productivities. The total productivity of a group of fewer than 2 reindeer is 0.</p>
<p>Starting with an empty group of reindeer, Santa will perform $M$ ($1 \leq M \leq 10^5$) modifications. The $i$th modification will involve the reindeer with name $N_i$. If $A_i=$ 'A', then this reindeer will be added to the lineup (in its correct spot) - in this case, its seniority and productivity values, $S_i$ and $P_i$, will be given. Otherwise, if $A_i=$ 'R', then this reindeer will be removed from the lineup. Each reindeer will only be added once, and will only be removed if it's currently in the lineup.</p>
<p>To track which combinations of reindeer are more effective than others, Santa would like you to calculate the total productivity of the lineup after every modification made to it. Quickly, now, Christmas won't wait!</p>
<h3>Input</h3>
<p>First line: $M$</p>
<p>Next $M$ lines: $A_i$ and $N_i$, followed by $S_i$ and $P_i$ if $A_i=$ 'A', for $i = 1 .. M$</p>
<h3>Output</h3>
<p>$M$ lines: The total productivity of the reindeer lineup after every modification</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5</span>
<span style="font-family: 'courier new', courier;">A Dancer 5 2</span>
<span style="font-family: 'courier new', courier;">A Prancer 3 8</span>
<span style="font-family: 'courier new', courier;">A Vixen 10 9</span>
<span style="font-family: 'courier new', courier;">R Dancer</span>
<span style="font-family: 'courier new', courier;">A Rudolph 3 1</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">0</span>
<span style="font-family: 'courier new', courier;">16</span>
<span style="font-family: 'courier new', courier;">34</span>
<span style="font-family: 'courier new', courier;">72</span>
<span style="font-family: 'courier new', courier;">80</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>After the first modification, the lineup consists of just Dancer, and so the total productivity is $0$.</p>
<p>After the second modification, Prancer is standing behind Dancer. Their productivity is $2 \cdot 8 = 16$.</p>
<p>After the third modification, we have Vixen, followed by Dancer, followed by Prancer. The productivity of Vixen and Dancer is $18$, while that of Dancer and Prancer is again $16$. Thus, the total productivity is $34$.</p>
<p>After the fourth modification, the lineup consists of only Vixen and Prancer, with productivity $72$.</p>
<p>Finally, after the fifth modification, Rudolph is behind Prancer, with this pair of reindeer contributing $8$ productivity, for a total of $80$.</p>