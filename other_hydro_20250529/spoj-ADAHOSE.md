<p>As you might already know, Ada the Ladybug is a farmer. She owns a square field. There is a hose wrapped around each <strong>1x1</strong> sub-field. All hoses are additionally combined into a bigger hose everywhere where they touch (so the water can arbitrarily flow between both of them [or even all four of them]). Each hose has its own flow-per-time attribute.</p>
<p>There is a big well (an infinite source of water) above the field and a big sprinkler under the field. Additionally very big hoses (for our case we can consider them infinetly big) are lead from well to top of the field and from bottom to the sprinkler. Your quest is simple: Calculate tha maximal total flow-per-time which goes from well to sprinkler.</p>
<p><img title="Field" src="../../content/morass:flow.png" alt="Field"></p>
<p><span style="font-size: 1.17em;">Input</span></p>
<p>The first line of input contains an integer  <strong> 1 ¡Ü  N ¡Ü     1000</strong>, the size of field.</p>
<p>The next <strong>N</strong> lines contains <strong>N</strong> integers <strong>0 ¡Ü A<sub>ij</sub> ¡Ü     1000</strong>, the size of each hose wrapped around.</p>
<h3>Output</h3>
<p>Output the maximal flow-per-time achievable.</p>
<h3>Example Input</h3>
<pre>3
9 3 2
1 9 3
3 3 9
</pre>
<h3>Example Output</h3>
<pre>26
</pre>
<h3>Example Input 1</h3>
<pre>4
2 0 0 2
0 2 2 0
2 0 0 2
0 2 2 0
</pre>
<h3>Example Output 1</h3>
<pre>8
</pre>
<h3>Example Input 2</h3>
<pre>8
2 2 0 1 2 1 5 1
5 1 3 7 1 6 3 1
3 8 5 3 6 6 8 8
2 9 6 6 8 2 3 0
5 4 3 9 7 1 0 4
2 5 1 5 2 5 6 5
5 3 8 3 9 8 1 1
8 9 0 8 2 3 1 9
</pre>
<h3>Example Output 2</h3>
<pre>28
</pre>