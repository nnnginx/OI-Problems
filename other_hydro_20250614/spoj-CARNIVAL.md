<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Peet is very excited because he is visiting a carnival for the first time in his life! As luck would have it, the carnival he is visiting today happens to be the largest one in the galaxy. It is known throughout the universe for its gigantic and super-fast anti-gravity Ferris wheels.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Peet is looking forward to riding as many rides as he can. Each of the rides cost a certain about of money. He has brought only a limited amount of money. Peet was starting to worry. However, to complicate matters even more, each of the rides have a height requirement: one has to be at least a certain height to be allowed to ride it. Peet is pretty short for his species, and he isn't tall enough to ride most of the rides!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">There is still hope. Since he paid attention at his biophysics classes at school, Peet realises that because of centrifugal force, the super-fast anti-gravity ferries wheels will actually increase his height when he rides them!&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The carnival contains N rides. Peet initially has M intergalactic dollars with him and his height is initially H feet. For each ride i (1 &lt;= i &lt;= N), Peet has to pay m[i] intergalactic dollars and his height has to be at least t[i] feet. &nbsp;Peet has calculated that his height would increase by h[i] feet after riding the ith ride. Help him find the maximum number of rides he can ride at the carnival.</div>
<p>
</p><p>Peet is very excited because he is visiting a carnival for the first time in his life! As luck would have it, the carnival he is visiting today happens to be the largest one in the galaxy. It is known throughout the universe for its gigantic and super-fast anti-gravity Ferris wheels.</p>
<p>Peet is looking forward to riding as many rides as he can. Each of the rides cost a certain about of money. He has brought only a limited amount of money. Peet was starting to worry. However, to complicate matters even more, each of the rides have a height requirement: one has to be at least a certain height to be allowed to ride it. Peet is pretty short for his species, and he isn't tall enough to ride most of the rides!</p>
<p>There is still hope. Since he paid attention at his biophysics classes at school, Peet realises that because of centrifugal force, the super-fast anti-gravity ferries wheels will actually increase his height when he rides them!&nbsp;</p>
<p>The carnival contains N rides. Peet initially has M intergalactic dollars with him and his height is initially H feet. For each ride i (1 &lt;= i &lt;= N), Peet has to pay m[i] intergalactic dollars and his height has to be at least t[i] feet. &nbsp;Peet has calculated that his height would increase by h[i] feet after riding the ith ride. Help him find the maximum number of rides he can ride at the carnival.</p>
<p></p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>
</p><p>The first line contains 3 integers N, M and H.</p>
<p>The next N lines contain 3 integers each. The (i+1)th line contains integers t[i], m[i] and h[i].</p>
<div><strong>Output</strong></div>
<p></p>
<p>Print a single integer - the maximum number of rides Peet can take at the carnival.</p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= N &lt;= 100</p>
<p>0 &lt;= m[i] &lt;= M &lt;= 1000</p>
<p>0 &lt;= t[i], h[i], H &lt;= 10^7</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
5 10 1</pre>
<pre>3 4 5</pre>
<pre>10 1 3</pre>
<pre>2 4 0</pre>
<pre>1 10 7</pre>
<pre>1 2 2

<strong>Output:</strong>
3</pre>
<pre><strong>Explanation:</strong></pre>
<p>
</p><p>Peet can take ride 5, spending 2 intergalactic dollars and increasing his height from 1 to 3. Now that he has at least height 3, he can take ride 1. He spends 4 more dollars and his height increases to 8. Finally, he can use the remaining 4 dollars to take ride 3. He cannot take any more rides since he has run out of money. You can check that Peet cannot ride more than 3 rides in this example.</p>
<p></p>