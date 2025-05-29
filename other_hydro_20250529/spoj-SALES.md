<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Bosco has gotten his hands on $B$&nbsp;($1 \leq B \leq 50$)&nbsp;dollars! Being a Magic the Gathering™ enthusiast, he wishes to spend some amount of his budget on cards to improve his deck.</p>
<p>He has located a local store that has $N$&nbsp;($1 \leq N \leq 30,000$) cards for sale. Card $i$&nbsp;costs $c_i$&nbsp;($1 \leq c_i \leq&nbsp;50$) dollars, and will improve Bosco’s DQI (Deck Quality Index) by $v_i$&nbsp;($1 \leq v_i \leq&nbsp;1000$) points. Only one copy of each card is for sale.</p>
<p>Business hasn’t been too great lately, so the store is offering sales on various days. Though the term “price adjustments” would be more accurate, as card prices can increase, “sales” are much more appealing – and, indeed, Bosco wants to go do all of his shopping on one of the $D$&nbsp;($1 \leq D \leq 3000$) days of the sales. In fact, he’s already acquired a list of the price adjustments that will be made.</p>
<p>On day $i$, the cost of card $a_i$&nbsp;($1 \leq a_i \leq&nbsp;N$) is changed to $b_i$&nbsp;($1 \leq b_i \leq&nbsp;50$), while all other cards remain unchanged. That is, before day $1$, all cards have their initial costs ($c_{1..N}$), and from then on, price adjustments accumulate from day to day.</p>
<p>Additionally, on each day, only certain cards from the store’s inventory are actually up for sale. In particular, on day $i$, only cards $x_i$ to $y_i$&nbsp;($1 \leq x_i \leq y_i \leq N$), inclusive, may be purchased.</p>
<p>Bosco doesn’t care how much of his budget he spends, but he absolutely must have the best possible deck. As such, for each of the $D$&nbsp;days, he wants to consider buying some (possibly empty) set of cards, such that the sum of their costs is no larger than $B$, and the sum of their DQI points is maximal. Determine this DQI sum for each day, so that Bosco will know when to go to take full advantage of the “sales”.</p>
<h3>Input</h3>
<p>Line $1$: 3 integers, $B$, $N$, and $D$</p>
<p>Next $N$ lines: 2 integers, $c_i$ and $v_i$, for $i=1..N$</p>
<p>Next $D$ lines: 4 integers, $a_i$, $b_i$, $x_i$, and $y_i$, for $i=1..D$</p>
<h3>Output</h3>
<p>For each day, output the maximal DQI sum of cards up for purchase that day which Bosco can purchase without going over his budget, considering all price changes that have occurred so far.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre><span style="font-family: 'courier new', courier;">5 5 3</span>
<span style="font-family: 'courier new', courier;">9 6</span>
<span style="font-family: 'courier new', courier;">1 5</span>
<span style="font-family: 'courier new', courier;">2 3</span>
<span style="font-family: 'courier new', courier;">3 11</span>
<span style="font-family: 'courier new', courier;">2 7</span>
<span style="font-family: 'courier new', courier;">1 1 1 4</span>
<span style="font-family: 'courier new', courier;">4 6 3 5</span>
<span style="font-family: 'courier new', courier;">4 1 1 4</span></pre>
<p><strong>Output:</strong></p>
<pre><span style="font-family: 'courier new', courier;">22</span>
<span style="font-family: 'courier new', courier;">10</span>
<span style="font-family: 'courier new', courier;">25</span></pre>
<p><strong>Explanation of Sample:</strong></p>
<p>At first, the 5 cards (with point values 6, 5, 3, 11, and 7, respectively) have costs of 9, 1, 2, 3, and 2 dollars, in that order.</p>
<p>On the first day, the cost of the first card is reduced to 1 dollar, and the first 4 cards are up for purchase.</p>
<p>On the second day, the cost of the fourth card is increased to 6 dollars, and only the last 3 cards can be bought.</p>
<p>On the final day, the cost of card 4 is changed again, this time to 1 dollar, and the first 4 cards are once again considered.</p>
<p>&nbsp;</p>
<p>On the first day, Bosco should buy the first, second, and fourth cards, costing a total of 5 dollars.</p>
<p>On the second, cards 3 and 5 should be purchased with 4 dollars, as card 4 is now too expensive.</p>
<p>On the final day, all of the cards up for sale can be bought for 5 dollars. Notice that card 1 still costs 1 dollar, from the first price change.</p>
<p>&nbsp;</p>