<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The government of spojland has selected number of locations in the city for road construction&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and numbered those locations as 0,1,2,3,.......500.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now, they want to construct roads between various pairs of location(say A and B ) and have fixed the cost for travelling&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">between those locations from either end &nbsp;as W.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now , Rohit being a curious boy wants to find the minimum cost for travelling from location U (source) to Q number of other locations (destination).</div>
<p>The government of <strong>Spoj_land</strong> has selected number of locations in the city for road construction and numbered those locations as 0,1,2,3,.......500.</p>
<p>Now, they want to construct roads between various pairs of location(say <strong>A</strong> and <strong>B</strong> ) and have fixed the cost for travelling between those pair of locations from either end &nbsp;as <strong>W </strong><strong>unit</strong>.</p>
<p>Now , Rohit being a curious boy wants to find the minimum cost for travelling from location <strong>U</strong> (source) to <strong>Q</strong> number of other locations (destination).</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line contains <strong>N</strong> ,the number of roads that government constructed.</p>
<p>Next N line contains three integers <strong>A</strong> ,<strong>B</strong>, and <strong>W</strong>.</p>
<p>A and B represent the locations between which the road was constructed and W is the fixed cost for travelling from A to B or from B to A.</p>
<p>Next line contains an integer <strong>U</strong> from where Rohit wants to travel to other locations.</p>
<p>Next line contain <strong>Q</strong> , the number of queries (finding cost) that he wants to perform.</p>
<p>Next Q lines contain an integer <strong>V</strong> (destination) for which minimum cost is to be found <strong>from U</strong>.</p>
<h3>Output</h3>
<p>Print the required answer in each line.</p>
<p>If he can't travel from location U to V by any means then, print '<strong>NO PATH</strong>' without quotes.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7
0 1 4
0 3 8
1 4 1
1 2 2
4 2 3
2 5 3
3 4 2
0
4
1
4
5
7

<strong>Output:</strong>
4
5
9
NO PATH</pre>
<pre><strong>Constraints:</strong></pre>
<p>1&lt;=N&lt;=500</p>
<p>0&lt;=A,B&lt;=500</p>
<p>1&lt;=W&lt;=100</p>
<p>0&lt;=U,V&lt;=500</p>
<p>1&lt;=Q&lt;=500</p>
<pre><strong>Explanation:</strong></pre>
<pre>Query #1.</pre>
<pre>0-&gt;1: cost =4</pre>
<pre>Query #2.</pre>
<pre>0-&gt;4= 0-&gt;1-&gt;4 cost=4+1=5</pre>
<pre>Query #3.</pre>
<pre>0-&gt;5= 0-&gt;1-&gt;2-&gt;5 cost=4+2+3=9</pre>
<pre>Query #4.</pre>
<pre>0-&gt;7= no path exist between 0 and 7</pre>