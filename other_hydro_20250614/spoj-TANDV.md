<p>You have a treasure map that is arranged into a N _M grid. A grid square may be either sea or part of</p>
<p>an island. In addition, the map shows the treasure and an enemy Viking ship that occupies one (sea)</p>
<p>square. Finally, for convenience you have also drawn your own position.</p>
<p>Now you must set up a fixed route to get the treasure. The route must start at your position, end at</p>
<p>the treasure, and consist of a sequence of moves. In each move, you can go only to an (horizontally</p>
<p>or vertically) adjacent square that is not part of an island. But beware: The Viking ship might follow</p>
<p>you, using the same kind of moves! After each of your moves according to your route, the Viking</p>
<p>ship may move or not. Your move and the Vikings¡¯ reaction together is called a round.</p>
<p>After every round, the following checks are made:</p>
<p>_ If you are in line with the Viking ship (you are in the same vertical or horizontal line as the</p>
<p>Viking ship with only sea between the Viking ship and you), you are dead.</p>
<p>&nbsp;_ If you aren¡¯t dead and at the treasure-spot, you get the treasure.</p>
<p>Write a program that decides whether it is possible to set up a fixed route in advance such that you</p>
<p>can get the treasure by following this route and will not get killed by the Vikings ¨C no matter how the</p>
<p>Viking ship moves.</p>
<h3>Input</h3>
<p>The first line of input contains two integers N and M (1&lt;=N,M&lt;=700) , the dimensions of the map. Each of the</p>
<p>following N lines contain M characters. Each character describes a square in the map, and is either</p>
<p>. (sea), I (part of an island), V (the Viking ship), Y (your position), or T (the treasure). Each of V, Y,</p>
<p>and T will occur exactly once.</p>
<h3>Output</h3>
<p>The only line of the output must contain the string YES, if it is possible to set up a route to get the</p>
<p>treasure, or NO otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 7</pre>
<pre>Y.....V</pre>
<pre>..I....</pre>
<pre>..IIIII</pre>
<pre>.......</pre>
<pre>...T...
<strong>Output:</strong></pre>
<pre><strong>YES</strong></pre>