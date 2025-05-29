<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p style="margin: 0px;">Matt finds himself in a desert with $N$ ($2 \leq N \leq 10$) oases, each of which may have food, water, and/or a palm tree. If oasis $i$ has food, then $F_i=1$ - otherwise, $F_i=0$. Similarly, $W_i=1$ if and only if oasis $i$ has water, and $P_i=1$ if and only if it has a palm tree. These 3 values are completely independent of one another.</p>
<p style="margin: 0px;">&nbsp;</p>
<p style="margin: 0px;">Some pairs of these oases are connected by desert paths, which each take 1 hour to traverse. There are $M$ ($0 \leq M \leq 45$) such paths, with path $i$ connecting distinct oases $A_i$ and $B_i$ in both directions ($1 \leq A_i,B_i \leq N$). No pair of oases is directly connected by more than one path, and it's not guaranteed that all oases are connected by some system of paths.</p>
<p style="margin: 0px;">&nbsp;</p>
<p style="margin: 0px;">Matt starts at an oasis $S$, and wants to end up at a different oasis $E$ ($1 \leq S,E \leq N$).</p>
<p style="margin: 0px;">Both of these oases are quite nice - it's guaranteed that $F_S=W_S=P_S=F_E=W_E=P_E=1$.</p>
<p style="margin: 0px;">Since he's in a hurry to get out of the desert, he wants to travel there in at most $H$ ($1 \leq H \leq 10^9$) hours.</p>
<p style="margin: 0px;">However, he can only survive for up to $MF$ hours at a time without food, and up to $MW$ hours at a time without water ($1 \leq MF,MW \leq 4$). For example, if $MF=1$ and $MW=2$, then every single oasis he visits along the way must have food (as he would otherwise spend more than 1 hour without it), and he cannot visit 2 or more oases without water in a row.</p>
<p style="margin: 0px;">&nbsp;</p>
<p style="margin: 0px;">Since Matt is a computer scientist, before actually going anywhere, he's interested in the number of different paths he can take that will get him from oasis $S$ to oasis $E$ alive in at most $H$ hours.</p>
<p style="margin: 0px;">Note that there may be no such paths.</p>
<p style="margin: 0px;">Being a computer scientist, he of course only cares about this number modulo ($10^9+7$).</p>
<h3>Input</h3>
<p style="margin: 0px;">Line $1$: 7 integers, $N$, $M$, $H$, $S$, $E$, $MF$, and $MW$</p>
<p style="margin: 0px;">&nbsp;</p>
<p style="margin: 0px;">Next $N$ lines: 3 integers, $F_i$, $W_i$, and $P_i$, for $i = 1..N$</p>
<p style="margin: 0px;">&nbsp;</p>
<p style="margin: 0px;">Next $M$ lines: 2 integers, $A_i$ and $B_i$, for $i = 1..M$</p>
<h3>Output</h3>
<p>1 integer, the number of different valid paths, modulo ($10^9+7$)</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong></pre>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">3 3 3 1 2 1 4</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 1 1</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 1 1</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">0 1 0</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 2</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">2 3</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 3</span></p>
<pre><span style="font-weight: bold;">Output:</span></pre>
<pre><span style="font-family: 'courier new', courier;">2</span></pre>
<pre><span style="font-weight: bold;">Explanation:</span></pre>
<p style="margin: 0px;">The two possible paths, described in terms of oases visited, are $1 \rightarrow 2$ and $1 \rightarrow 2 \rightarrow 1 \rightarrow 2$. Matt can never go to oasis 3, as it doesn't contain food, which he can't survive without for more than 1 hour. The path $1 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 1 \rightarrow 2$ is not valid, as it would take 5 hours rather than at most 3.</p>
<p>Note that oasis 3 is the only oasis without a palm tree.</p>
<h3>Example 2</h3>
<pre><strong>Input:</strong></pre>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">5 5 3 3 2 3 2</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 0 0</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 1 1</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 1 1</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">0 0 1</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">0 1 0</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 2</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 3</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">1 4</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">3 4</span></p>
<p style="margin: 0px;"><span style="font-family: 'courier new', courier;">4 2</span></p>
<pre><span style="font-weight: bold;">Output:</span></pre>
<pre><span style="font-family: 'courier new', courier;">2</span></pre>
<pre><span style="font-weight: bold;">Explanation:</span></pre>
<p>The two possible paths are $3 \rightarrow 1 \rightarrow 2$ and $3 \rightarrow 4 \rightarrow 2$.</p>
<p>This time, oases 1 and 5 are lacking in palm trees.</p>