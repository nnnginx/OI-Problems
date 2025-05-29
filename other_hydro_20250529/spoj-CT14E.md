<div>
<p>Bob likes to draw camels: with a single hump, two humps, three humps, etc. He draws a camel by connecting points on a coordinate plane. Now he's drawing camels with <span><em>t</em></span> humps,representing them as polylines in the plane. Each polyline consists of <span><em>n</em></span> vertices withcoordinates <span>(<em>x</em><sub>1</sub>, <em>y</em><sub>1</sub>)</span>, <span>(<em>x</em><sub>2</sub>, <em>y</em><sub>2</sub>)</span>, ..., <span>(<em>x</em><sub><em>n</em></sub>, <em>y</em><sub><em>n</em></sub>)</span>. The first vertex has a coordinate <span><em>x</em><sub>1</sub> = 1</span>, the second— <span><em>x</em><sub>2</sub> = 2</span>, etc. Coordinates <span><em>y</em><sub><em>i</em></sub></span> might be any, but should satisfy the following conditions:</p>
<ul>
<li> there should be <span><em>t</em></span> humps precisely, i.e. such indexes <span><em>j</em></span> (<span>2 ≤ <em>j</em> ≤ <em>n</em> - 1</span>), so that <span><em>y</em><sub><em>j</em> - 1</sub> &lt; <em>y</em><sub><em>j</em></sub> &gt; <em>y</em><sub><em>j</em> + 1</sub></span>, </li>
<li> there should be precisely <span><em>t</em> - 1</span> such indexes <span><em>j</em></span> (<span>2 ≤ <em>j</em> ≤ <em>n</em> - 1</span>), so that <span><em>y</em><sub><em>j</em> - 1</sub> &gt; <em>y</em><sub><em>j</em></sub> &lt; <em>y</em><sub><em>j</em> + 1</sub></span>, </li>
<li> no segment of a polyline should be parallel to the <span><em>Ox</em></span>-axis, </li>
<li> all <span><em>y</em><sub><em>i</em></sub></span> are integers between 1 and 4. </li>
</ul>
<p>For a series of his drawings of camels with <span><em>t</em></span> humps Bob wants to buy a notebook, but he doesn'tknow how many pages he will need. Output the amount of different polylines that can be drawn to represent camels with <span><em>t</em></span> humps for a given number <span><em>n</em></span>.</p>
</div>
<h3>Input</h3>
<p>The first line of input contains the number of testcases , Ntest.</p>
<p>Each testcase contains a pair of integers <span><em>n</em></span> and <span><em>t</em></span> (<span>3 ≤ <em>n</em> ≤ 20</span>, <span>1 ≤ <em>t</em> ≤ 10</span>).</p>
<h3>Output</h3>
<p>For each testcase ,output the required amount of camels with <span><em>t</em></span> humps.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>6 1<br><strong>Output:</strong><br>6<br><br><strong>Note</strong><div><div>In the first sample test sequences of <span><em>y</em></span>-coordinates for six camels are: 123421, 123431,<br>&nbsp;123432, 124321, 134321 и 234321 (each digit corresponds to one value of <span><em>y</em><sub><em>i</em></sub></span>).</div><br><br></div></pre>