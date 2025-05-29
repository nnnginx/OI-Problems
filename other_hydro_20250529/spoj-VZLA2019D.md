<p>Drawing stars on the last page of a notebook is a very entertaining hobby. Did you know these cute "stars" are actually called polygrams?<br><br>Given a regular polygon with <strong>p</strong> vertices, we define a <em>polygram</em> <strong>p/q</strong>, as the resultant polygon obtained after connecting every i-th vertex with the (i+q)-th vertex.<br><br>You may know the polygram 5/2 as <em>pentagram</em><br><br>Another example is the <em>hexagram </em>6/2. Given that 6 and 2 are not coprime, this polygram is composed by two 3/1 polygrams<br><br><img title="polygrams" src="file://Yo4A07Gr.png" alt="Star polygons" height="350"><br>Given a regular polygon with p vertices, its radius R (the distance from its center to any vertex) and a number q, can you calculate the area of the polygram p/q?<br><br>It is guaranteed that the resultant polygon will not be degenerated, i.e q ¡Ù p/2 and q ¡Ù p</p>
<h3>Input</h3>
<p>The first and only line of the input contains three integers <strong>p</strong>, <strong>q</strong> and <strong>r</strong></p>
<h3>Output</h3>
<p>Print in a single line the area of the resultant polygram p/q with radius r. Print the answer with exactly five decimal places</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 4 2

<strong>Output:</strong>
9.51057<br><strong><br>Input:</strong>
10 4 5
<strong><br>Output:</strong>
40.61496 <br></pre>
<h3>Constraints</h3>
<p>3 ¡Ü p ¡Ü 10<sup>3</sup> <br> 1 ¡Ü q &lt; p <br> 1 ¡Ü r ¡Ü 100 <br>q ¡Ù p/2 and q ¡Ù p</p>