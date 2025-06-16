<p>Ada the Ladybug lives in Bugladesh. It is a very specific country - there are plenty of cities, but since the goverment doesn't "waste" money, there is only one simple path between each pair of cities.</p>
<p>Ada is working as Traveling Salesman. She travels between cities, buying and selling products. A product has fixed price in each city (same for buy/sale). Since Ada travels with bike (to avoid payments for travels) so she can carry at most one item at a moment.</p>
<p>She is currently in some city, and she wants to choose such city, that she will make as much money as possible by travelling to that city (by simple path). Can you help her?</p>
<h3>Input</h3>
<p>The first line will contain <strong>0 &lt; N ¡Ü 10<sup>5</sup>, 0 &lt; Q ¡Ü 5*10<sup>5</sup></strong>, number of cities and number of queries respectively.</p>
<p>Then one line with <strong>N</strong> integers follow, <strong>1 ¡Ü A<sub>i</sub> ¡Ü     10<sup>9</sup></strong>, the price in <strong>i<sup>th</sup></strong> city.</p>
<p>Afterward <strong>N-1</strong> lines follow, each containing two numbers <strong>0 ¡Ü i,j     &lt; N</strong> (<strong>i ¡Ù j</strong>), meaning that there is a simple path between city <strong>i</strong> and city <strong>j</strong>.</p>
<p>Then <strong>Q</strong> lines follows, each containing exactly one integer <strong>0 ¡Ü i &lt; N</strong>- the city in which Ada begins.</p>
<h3>Output</h3>
<p>Print <strong>Q</strong> lines, the maximal amount of money, Ada can earn.</p>
<h3>Example Input</h3>
<pre>6 6
1 2 3 4 5 4
1 0
1 2
1 3
3 4
4 5
0
1
2
3
4
5
</pre>
<h3>Example Output</h3>
<pre>4
3
3
1
1
2
</pre>
<h3>Example Input</h3>
<pre>5 2
1 5 2 4 3
0 1
1 2
2 3
3 4
0
2
</pre>
<h3>Example Output</h3>
<pre>6
3
</pre>
<h3>Output explanations [Possible destination cities of first example input]</h3>
<pre>4
4
4
2
2
2
</pre>
<p>Note that some of the destinations might have ended somewhere else, but it would result in same income!</p>