<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The competition is drawing to a close, and The Team could really use another balloon to help them come out on top...good thing they're no chumps, and thought of this in advance! Before the contest started, they instructed an accomplice to go to the local balloon shop, buy an extra balloon, and deliver it to them at the conclusion of the event. It is true that their balloons then won't match up with the scoreboard's record of which problems they've solved - but, in the end, it's the balloons that count! In fact, The Team knows that, the larger their extra balloon, the more their opponents (and the judges) will be intimidated. They're not the best ACM-ICPC team in the world for nothing!</p>
<p>However, this balloon shop is rather strange. The accomplice is given an empty balloon (a balloon with size 0), and told that he can tie it closed and keep it after exactly $N$ ($1 \leq N \leq 10^6$) minutes. In the meantime, during each minute, an inflation offer is available. If offer $i$ is taken, then, at the start of the $i$th minute, the balloon's size will be increased by $a_i$ ($0 \leq a_i \leq 10^6$). However, since the balloon cannot be closed until the end, its air will leak out at a constant rate, which depends on the gas that was used - in particular, its size will immediately start to decrease at a rate of $d_i$ ($0 \leq d_i \leq 10^6$) per minute, until either another offer is taken, or the balloon deflates completely (its size can never become negative, of course).</p>
<p>The Team will not be happy if they don't receive the largest balloon possible. Unfortunately, their accomplice happens to be...you. Can you figure out the maximal size that the balloon can have at the start of minute $N+1$, before it's too late?</p>
<h3>Input</h3>
<p>First line: 1 integer, $N$</p>
<p>Next $N$ lines: 2 integers, $a_i$ and $d_i$, for $i=1..N$</p>
<h3>Output</h3>
<p>1 integer, the maximal size which the balloon can have at the start of minute $N+1$.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5</span>
<span style="font-family: 'courier new', courier;">2 3</span>
<span style="font-family: 'courier new', courier;">10 2</span>
<span style="font-family: 'courier new', courier;">0 1</span>
<span style="font-family: 'courier new', courier;">5 4</span>
<span style="font-family: 'courier new', courier;">1 10</span></pre>
<pre><span style="font-weight: bold;">Output:</span></pre>
<pre><span style="font-family: 'courier new', courier;">5</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The best option is to take only the offers at minutes 2 and 3. At the start of minute 2, the balloon will be inflated to size 10, and will deflate to size 8 by the start of minute 3. At that point, the balloon's size will not change, but its deflation rate will change to 1. As a result, by the start of minute 6, its size will be 5.</p>
<p>Note that, if the offer at minute 1 is additionally taken, the balloon will simply be inflated to size 2 before deflating back to size 0 by the start of minute 2 - therefore, this will not change the outcome.</p>
<p>Also note that, if the offer at minute 4 is additionally taken, the balloon will inflate to size 12 at the start of minute 4, but its deflation rate of 4 will result in a size of 4 at the start of minute 6, which is not optimal.</p>
<p>&nbsp;</p>