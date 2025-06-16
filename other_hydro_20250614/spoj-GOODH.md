<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The ACM-ICPC World Finals are over! Which team came out on top? Why, only our favourite team - everyone's favourite team - the most deserving, lovable, courteous, powerful, flawless, successful team that has ever existed. Who else?</p>
<p>It's time to celebrate, and what better way is there to celebrate than by eating cake? The contest organizers have bought $N$ ($1 \leq N \leq 200$) cakes (conveniently numbered $1..N$) - however, ever generous, The Team will only eat cake 1, leaving the rest for the other, inferior teams. They <em>will</em> need their cake to be as tasty as possible, though. To help with this, $M$ ($0 \leq M \leq 200$) globs of icing are available, which will be distributed among the cakes. Icing is always used in whole globs.</p>
<p>The cakes are arranged in a somewhat strange way - piled on top of one another. Cake 1 is directly on top of a table, while every other cake $i$ (for $i=2..N$) is directly on top of cake $c_i$. $c_1$ is considered to have a value of 0. Note that there may be multiple cakes on top of a single cake, and that the entire structure obeys the laws of physics (no cake is on top of itself, and no cakes are floating).</p>
<p>Now, the tastiness of any cake $i$ is determined by the formula $b_i + m_i(x_i + y_i)$. $b_i$ ($0 \leq b_i \leq 100$) and $m_i$ ($0 \leq m_i \leq 100$) are simply properties of cake $i$, which depend on its size, shape, weight, temperature, fluffiness, and so on. $x_i$ is the number of globs of icing that are chosen to be applied to cake $i$. If there are no cakes on top of cake $i$, $y_i=0$ - otherwise, $y_i$ is the minimal tastiness of any cake directly on top of cake $i$. No cake will ever be capable of achieving a tastiness value larger than $2^{60}$, no matter how the icing is distributed.</p>
<p>The members of The Team have already, of course, determined how the available icing could be optimally applied to the mountain of cakes to maximize the tastiness of their cake (cake 1). However, the contest organizers are the ones who will actually be distributing the icing, and they had better hope they get it right! Can you help them determine how tasty cake 1 should be? You don't want to know what The Team will do if their celebration isn't perfect...</p>
<h3>Input</h3>
<p>First line: 2 integers, $N$ and $M$</p>
<p>Next $N$ lines: 3 integers, $c_i$, $b_i$, and $m_i$, for $i=1..N$</p>
<h3>Output</h3>
<p>1 integer, the maximal tastiness of cake 1, after all of the icing has been used</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">3 2</span>
<span style="font-family: 'courier new', courier;">0 5 1</span>
<span style="font-family: 'courier new', courier;">1 3 4</span>
<span style="font-family: 'courier new', courier;">1 2 6</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">12</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The optimal icing distribution is 1 glob each on cakes 2 and 3. This gives cake 2 a tastiness of $3+4(1+0)=7$, and cake 3 a tastiness of $2+6(1+0)=8$. Since both of these cakes are on top of cake 1, it then has a tastiness of $5+1(0+min\{7,8\})=12$. No other icing distribution yields a higher tastiness for cake 1.</p>
<p>&nbsp;</p>