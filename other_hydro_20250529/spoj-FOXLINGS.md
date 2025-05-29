<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>It¡¯s Christmas time in the forest, and both the Fox and the Wolf families are celebrating. The rather large Fox family consists of two parents as well as $N$&nbsp;($1 \leq N \leq 10^9$) little Foxlings. The parents have decided to give their children a special treat this year ¨C crackers! After all, it¡¯s a well-known fact that Foxen love crackers.</p>
<p>With such a big family, the parents can¡¯t afford that many crackers. As such, they wish to minimize how many they give out, but still insure that each Foxling gets at least a bit. The parents can only give out entire crackers, which can then be divided and passed around.</p>
<p>With this many children, not all of them know one another all that well. The Foxlings have names, of course, but their parents are computer scientists, so they have also conveniently numbered them from $1$ to $N$. There are $M$&nbsp;($1 \leq M \leq 10^5$)&nbsp;unique two-way friendships among the Foxlings, where relationship $i$&nbsp;is described by the distinct integers $A_i$ and $B_i$&nbsp;($1 \leq A_i,B_i \leq N$), indicating that Foxling $A_i$&nbsp;is friends with Foxling $B_i$, and vice versa. When a Foxling is given a cracker, he can use his tail to precisely split it into as many pieces as he wants (the tails of Foxen have many fascinating uses). He can then pass these pieces around to his friends, who can repeat this process themselves.</p>
<h3>Input</h3>
<p>Line $1$: 2 integers, $N$ and $M$</p>
<p>Next $M$ lines: 2 integers, $A_i$ and $B_i$, for $i=1..M$</p>
<h3>Output</h3>
<p>A single integer ¨C the minimum number crackers must be given out, such that each Foxling ends up with at least a small part of a cracker.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">9 5</span>
<span style="font-family: 'courier new', courier;">3 1</span>
<span style="font-family: 'courier new', courier;">6 1</span>
<span style="font-family: 'courier new', courier;">7 6</span>
<span style="font-family: 'courier new', courier;">2 7</span>
<span style="font-family: 'courier new', courier;">8 9</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The parents can give one cracker to Foxling 6, who will then split it into three and give pieces to his friends (Foxlings 1 and 7). Foxling 7 can then give half of his piece to his other friend, Foxling 2.</p>
<p>They can give another cracker to Foxling 8, who will split it with Foxling 9.</p>
<p>This leaves Foxlings 4 and 5, who have no friends (don¡¯t worry, Foxen have long since outgrown the need for friends), and who must be given one cracker each. This brings the total up to 4 crackers.</p>
<p>&nbsp;</p>