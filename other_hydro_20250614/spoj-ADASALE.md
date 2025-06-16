<p>Ada the Ladybug lives in Bugladesh. It is a very specific country - there are some cities, but since the goverment doesn't "waste" money, they all lie on one simple path.</p>
<p>Ada is working as Traveling Salesman. She travels between cities, buying and selling products. A product has some varying price in each city (same for buy/sale - described later). Ada travels with bike (to avoid payments for travels) so she can carry at most <strong>K</strong> items at time in her backpack.</p>
<p>She is currently in the first city, and she wants to lineary go to last city. She wants to buy/sell items in a way to maximize her profit. Can you help her?</p>
<p>The system is following: Ada has a bag which can carry at most <strong>K</strong> items. She travels cities lineary (from city <strong>c</strong> to city <strong>c+1</strong>). Ss she is in a city <strong>c</strong>, she can either immediately move to next city <strong>or</strong> buy a licence to trade for <strong>L<sub>c</sub></strong> money. For each city it is also given magical constant <strong>P<sub>c</sub></strong>. The buying/selling system is pretty weird. Buying an item in city <strong>c</strong> while actually having <strong>i-1</strong> items in backpack costs <strong>P<sub>c</sub>*i*c%MOD</strong>. Similary selling of an item in city <strong>c</strong> while actually having <strong>i</strong> items in backpack is for <strong>P<sub>c</sub>*i*c%MOD</strong>. You can buy any number of items in a city and you can also sell any number of items in city. Anyway note that the number of items can't exceed <strong>K</strong> (and obviously can't be negative).</p>
<h3>Input</h3>
<p>The first line of input will contain three integers <strong>1 ¡Ü N, K ¡Ü     3000</strong> and <strong> 1     ¡Ü MOD ¡Ü  10<sup>4</sup></strong>.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0 &lt; L<sub>i</sub> ¡Ü     1000</strong>, the cost of licence for each city.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0 &lt; P<sub>i</sub> ¡Ü     1000</strong>, the magical constant for each city.</p>
<p>Cities are numbered from 1.</p>
<h3>Output</h3>
<p>Output the maximal number of money Ada can gain.</p>
<h3>Example Input</h3>
<pre>5 1 3
1 1 1 1 1
1 1 1 1 1
</pre>
<h3>Example Output</h3>
<pre>0
</pre>
<h3>Example Input</h3>
<pre>5 5 6
1 1 1 1 1
1 1 1 1 1
</pre>
<h3>Example Output</h3>
<pre>9
</pre>
<h3>Example Input</h3>
<pre>6 10 11
1 2 3 3 2 1
1 3 2 5 1 7
</pre>
<h3>Example Output</h3>
<pre>19
</pre>
<h3>Example Input</h3>
<pre>9 2 20
6 6 6 6 6 6 6 6 6
2 4 6 8 2 4 6 8 5
</pre>
<h3>Example Output</h3>
<pre>16
</pre>
<h3>Example Input</h3>
<pre>10 2 20
5 9 3 4 7 5 2 4 7 2
2 1 4 5 4 5 6 3 2 5
</pre>
<h3>Example Output</h3>
<pre>25
</pre>