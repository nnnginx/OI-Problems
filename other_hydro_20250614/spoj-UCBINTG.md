<p>A popular tourist destination country is situated on a breathtakingly beautiful archipelago constantly bathed by the sun. The country's residents are very proud of their numerous islands. However, global warming has them very worried: raising sea levels are resulting in rapidly increasing loss of dry land, which is diminishing the beauty of the archipelago.</p>
<p>The map of the archipelago is represented by a grid of <strong>R</strong> by <strong>C</strong> squares (characters). The character <strong>'X'</strong> (<strong>uppercase</strong> letter x) represents dry land, while '.' (period) represents sea.</p>
<p>It has been estimated that, in fifty years, sea will have flooded every square of land that is currently surrounded by sea on <strong>three</strong> or on all <strong>four</strong> sides (north, south, east, west). Assume that all squares outside the map (along the edges) are covered by sea.</p>
<p>Your task is computing the map of the archipelago in fifty years (after the described sea level rise). Since there will probably be less land than today, you shouldn't print out the whole map, but only its <strong>smallest rectangular part that contains all land squares</strong>. It is guaranteed that at least one square of land will remain in all test cases.</p>
<h3>Input</h3>
<p>The first line of input contains two positive integers, <strong>R</strong> and <strong>C</strong> (1 ¡Ü&nbsp;<strong>R</strong>, <strong>C</strong>&nbsp;¡Ü&nbsp;10), the dimensions of the current map.</p>
<p>Each of the following <strong>R</strong> lines contains <strong>C</strong> characters. These <strong>R</strong> by <strong>C</strong> characters represent the current map of the archipelago.</p>
<h3>Output</h3>
<p>The output must contain an appropriate number of lines representing the required rectangular part of the future (flooded) map.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 3
...
.X.
.X.
.X.
...

<strong>Output:</strong>
X
</pre>
<pre><strong>Input:</strong>
3 10
..........
..XXX.XXX.
XXX.......

<strong>Output:</strong>
.XX...X
XX.....
</pre>