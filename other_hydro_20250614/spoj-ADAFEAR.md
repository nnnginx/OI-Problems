<p>As you might already know, Ada the Ladybug is a farmer. She grows many vegetables. During past months, her crop was attacked by colony of parasites. Each vegetable was attacked by <strong>A<sub>i</sub></strong> parasites. Ada has only limited answer for this. She bought a few bottles with <strong>Primal Fear</strong>, which is a mixture agains parasites.</p>
<p><strong>Primal Fear</strong> works in following way: Each <strong>Primal Fear</strong> bottle has a power assigned to it (which is coincidentally a prime number). If it is applied to a vegetable with <strong> N </strong> parasites on it, either the <strong>N</strong> is divisible by its <strong>power</strong>, then the size of colony is reduced to <strong>N/power</strong>, or - if the size is not divisible - then it has no effect. Also, as soon as you apply mixture against a colony, the rest of colony will become immune agains <strong>Primal Fear</strong>.</p>
<p>Ada didn't know what to buy so she bought one bottle of every possible <strong>power</strong>. Can you find out the best strategy to fight agains parasites?</p>
<h3>Input</h3>
<p>The first line of input will contain <strong>1 ¡Ü N ¡Ü 1000</strong>, the number of vegetable.</p>
<p>&nbsp;</p>
<p>The line will contain <strong>N</strong> numbers <strong>1 ¡Ü A<sub>i</sub> ¡Ü     2000</strong>, the size of colony on <strong>i<sup>th</sup></strong> vegetable.</p>
<h3>Output</h3>
<p>Print the minimum sum of sizes of colonies which could be achieved after applying <strong>Primal Fear</strong> optimally.</p>
<h3>Example Input</h3>
<pre>3
2 8 6
</pre>
<h3>Example Output</h3>
<pre>8
</pre>
<h3>Example Input</h3>
<pre>4
6 6 6 6
</pre>
<h3>Example Output</h3>
<pre>17
</pre>
<h3>Example Input</h3>
<pre>3 
7 4 22
</pre>
<h3>Example Output</h3>
<pre>5
</pre>
<h3>Example Input</h3>
<pre>3
11 22 17
</pre>
<h3>Example Output</h3>
<pre>13
</pre>
<h3>Example Input</h3>
<pre>2
77 11
</pre>
<h3>Example Output</h3>
<pre>12
</pre>