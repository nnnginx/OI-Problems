<p>We can represent a grid of skyscrapers by an NxN matrix of their positive  heights. A skyscraper is made out of square blocks, and you may travel  through them using a special elevator that can move as any other, but  also sideways (four possible directions on a fixed floor). They may move  anywhere as long as they don't exit the skyscrapers. In other words, if  the elevator is inside a skyscraper, it may move to the neighboring  skyscraper only if its height is greater or equal to the current level  the elevator is at.</p>
<p>Moving sideways (in one of the 4 directions, that is, N, E, S, W...) is done for free when using this elevator, but moving one floor up or down costs exactly one unit.</p>
<p>Given  the positions of two skyscrapers, find the cost of moving from the<strong> top  block</strong> of the first to the <strong>top block</strong> of the second using the described  elevator.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer N ( 1 &lt;= N &lt;= 1000 ). The next line contains four integers, x<sub>a</sub>, y<sub>a</sub>, x<sub>b</sub>, y<sub>b</sub>, (between 1 and N), representing the positions of the two skyscrapers.</p>
<p>The next line contains three integers: A, B and C (1 &lt;= A, B, C &lt;= 10<sup>9</sup>).</p>
<p>Generate the height of the skyscraper at coordinates (i, j) using the formula h<sub>ij</sub> = (((i-1)*N+j-1)*A + B) mod C (indicies are 1-based).</p>
<h3>Output</h3>
<p>To the first and only line of input output the solution.</p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br>3<br>1 1 3 3<br>5 5 7<br><br><strong>Output:</strong> <br>2<br></pre>