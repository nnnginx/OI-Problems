<p>
Lumberjack Mirko needs to chop down <strong>M</strong> metres of wood. It is an easy job for him since he has a nifty&nbsp;new woodcutting machine that can take down forests like wildfire. However, Mirko is only allowed to&nbsp;cut a single row of trees.</p>

<p>Mirko‟s machine works as follows: Mirko sets a height parameter <strong>H</strong> (in metres), and the machine raises&nbsp;a giant sawblade to that height and cuts off all tree parts higher than <strong>H</strong> (of course, trees not higher than&nbsp;<strong>H</strong> meters remain intact). Mirko then takes the parts that were cut off. For example, if the tree row&nbsp;contains trees with heights of 20, 15, 10, and 17 metres, and Mirko raises his sawblade to 15 metres, the&nbsp;remaining tree heights after cutting will be 15, 15, 10, and 15 metres, respectively, while Mirko will take&nbsp;5 metres off the first tree and 2 metres off the fourth tree (7 metres of wood in total).</p>

<p>Mirko is <strong>ecologically</strong> minded, so he doesn‟t want to cut off more wood than necessary. That‟s why he&nbsp;wants to set his sawblade as high as possible. Help Mirko find the <strong>maximum integer height</strong> of the&nbsp;sawblade that still allows him to cut off <strong>at least M</strong> metres of wood.</p>

<h3>Input</h3>
<p>The first line of input contains two space-separated positive integers, <strong>N</strong> (the number of trees, 1 ≤ <strong>N</strong> ≤&nbsp;1 000 000) and <strong>M</strong> (Mirko‟s required wood amount, 1 ≤ <strong>M</strong> ≤ 2 000 000 000).</p>
<p>The second line of input contains <strong>N</strong> space-separated positive integers less than 1 000 000 000, the&nbsp;heights of each tree (in metres). The sum of all heights will exceed <strong>M</strong>, thus Mirko will always be able to&nbsp;obtain the required amount of wood.</p>

<h3>Output</h3>
<p>The first and only line of output must contain the required height setting.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 7
20 15 10 17

<strong>Output:</strong>
15</pre>

<pre><strong>Input:</strong>
5 20
4 42 40 26 46

<strong>Output:</strong>
36</pre>