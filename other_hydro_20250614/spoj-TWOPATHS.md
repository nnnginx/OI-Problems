<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 1em; margin-left: 0px; padding: 0px;">In Flatland there are <em>N</em>&nbsp;cities, connected by <em>N-1</em>&nbsp;two-way roads. The cities are numbered from 1 to <em>N</em>. You can get from one city to another moving along the roads.</p>
<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 1em; margin-left: 0px; padding: 0px;">The "Two Paths" company, has won a tender to repair two paths in Flatland. A path is a sequence of different cities, connected sequentially by roads. The company is allowed to choose by itself the paths to repair. The only condition they have to meet is that the two paths shouldn't cross (i.e. shouldn't have common cities).</p>
<p style="margin-top: 0px; margin-right: 0px; margin-bottom: 1em; margin-left: 0px; padding: 0px;">It is known that the profit, the "Two Paths" company will get, equals the product of the lengths of the two paths. Let's consider the length of each road equals 1, and the length of a path equals the amount of roads in it. Find the maximum possible profit for the company.</p>
<h3>Input</h3>
<p>The first line contains an integer <em>N</em> (2 ¡Ü&nbsp;<em>N</em> ¡Ü&nbsp;100000), where <em>N</em>&nbsp;is the amount of cities in the country. The following <em>N-1&nbsp;</em>lines contain the information about the roads. Each line contains a pair of numbers of the cities, connected by the road <em>a</em> and <em>b (1 ¡Ü&nbsp;a, b ¡Ü&nbsp;N)</em></p>
<h3>Output</h3>
<p>Output the maximum possible profit.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><strong><span style="font-weight: normal;">4</span></strong></pre>
<pre>1 2</pre>
<pre>2 3</pre>
<pre>3 4</pre>
<pre><strong><br></strong></pre>
<pre><strong>Output:</strong></pre>
<pre>1</pre>