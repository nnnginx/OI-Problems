<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>At last, Santa is on his way! He's got a number of presents to deliver to various households, and he won't stop until he's disposed of them all. However, each present is only suitable for one gender - for example, men might enjoy such things as baseball bats, football helmets, and certain adult reading material, while women would prefer make-up, knitting needles, and certain other adult reading material.</p>
<p>At the moment, Santa is in a neighbourhood with $H$ ($1 \leq H \leq 50$) houses (numbered $1..H$), connected by $R$ ($1 \leq R \leq 10^{4}$) roads. The family living in house $i$ includes $M_i$ ($0 \leq M_i \leq 10$) males and $F_i$ ($0 \leq F_i \leq 10$) females. The $i$th road runs between distinct houses $A_i$ and $B_i$, and can be travelled in either direction. No pair of houses is directly connected by more than one road.</p>
<p>Santa starts at house $1$, carrying $M_S$ ($0 \leq M_S \leq 50$) male-appropriate and $F_S$ ($0 \leq F_S \leq 50$) female-appropriate presents. He then repeats the following process until he's out of gifts. First, he moves randomly to an adjacent house (a house reachable by taking one road) - it's guaranteed that there will be at least one such house. If he currently has $m$ male-appropriate and $f$ female-approrpiate presents, his probability of moving to adjacent house $i$ is proportional to the value of $M_i m + F_i f$. Of course, the probabilities for all adjacent houses must add up to $1$. Note that if this value is $0$ for all adjacent houses, then Santa will move to any of them with equal probability. After reaching the new house, he delivers a male present to it with probability $\frac{m}{m+f}$, and a female present otherwise.</p>
<p>Wanting to plan ahead to leaving this neighbourhood, Santa is curious as to where he'll end up. He'd like you to calculate the probability of him being at each of the $H$ houses when he runs out of presents.&nbsp;</p>
<h3>Input</h3>
<p>First line: $H$ and $R$</p>
<p>Next $H$ lines: $M_i$ and $F_i$, for $i = 1..H$</p>
<p>Next $R$ lines: $A_i$ and $B_i$, for $i = 1..R$</p>
<p>Next line: $M_S$ and $F_S$</p>
<h3>Output</h3>
<p>$H$ lines: The probability of Santa finishing his present-delivering process at house $i$, rounded off to 6 decimal places, for $i = 1..H$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4 3<br>1 2<br>2 1<br>1 1<br>4 0<br>1 2<br>2 4<br>3 1<br>1 1</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">0.760000<br>0.000000<br>0.000000<br>0.240000</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The neighbourhood looks as follows:</p>
<p><img src="../../../content/sourspinach:santa2.png" alt=""></p>
<p>House $1$ is adjacent to houses $2$ and $3$. The probability of Santa moving to house $2$ is proportional to $2 \cdot 1 + 1 \cdot 1 = 3$, while the probability of him moving to house $3$ is proportional to $1 \cdot 1 + 1 \cdot 1 = 2$. Therefore, he will move to house $2$ with probability $\frac{3}{5}$, and to house $3$ with probability $\frac{2}{5}$. If he moves to house $3$, then, regardless of which present he delivers, he will be guaranteed to move back to house $1$ next, where he will deliver the remaining present.</p>
<p>Otherwise, if he moves to house $2$ at first, then he will proceed to deliver a male-appropriate present there with probability $\frac{1}{1+1} = \frac{1}{2}$, and a female-appropriate one also with probability $\frac{1}{2}$. In the former case, he will then have just 1 female present remaining, so he will move on to house $4$ with probability $0$, and back to house $1$ with probability $1$. Otherwise, he will have 1 male present remaining, and will move on to house $4$ with probability $\frac{4}{5}$, and back to house $1$ with probability $\frac{1}{5}$. In any case, he will then deliver his second present and be done.&nbsp;</p>

<p><br></p>
<p>
<b><u>Editors note:</u></b>
<br>
You can deliver more male or female presents to a house, than the number of given gender inhabitants. Even if that number would be zero, you could still drop given type of presents. You only need to follow the formulas in the problem description.
</p>