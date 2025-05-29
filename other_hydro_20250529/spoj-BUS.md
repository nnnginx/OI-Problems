<p><img src="/content/ahven:bus.gif" style="float: right" width="200" vspace="5" hspace="5">The city Buscelona (as the name suggests) has a great bus transport system. All buses have circular lines. The bus drivers in Buscelona like to chat. Fortunately most bus lines have some stops in common. If a bus driver meets a colleague on a bus stop they chat a bit and exchange all news they know.</p>
<p>The operation of buses is highly synchronized. The time necessary to get from one stop to the next stop is always exactly 1 minute.</p>
<p>Each morning each bus driver has some important news that only he knows. When a busdriver meets a colleague he will tell him all news he knows. If two bus drivers share the same start station, they will exchange their news there already (before they start working). Note that exchanging news and stopping does not take any time.</p>

<h3>Input</h3>
<p>The first line of a test case contains the number of bus lines <i>n</i> (0 &lt; <i>n</i> &lt; 50). The following <i>n</i> lines start with a number <i>s</i> (0 &lt; <i>s</i> &lt; 50) indicating the stops of a busline. On the same line follow <i>s</i> numbers representing a bus station each. A bus starts at the first station. When a bus reaches the last station, the bus will drive to the first station again.</p>
<p>There are many test cases separated by an empty line. Input data terminates with <i>n</i> = 0.</p>

<h3>Output</h3>
<p>For each test case you should output the time in minutes which it takes until all bus drivers know all news. If that never happens, your program should write the word "NEVER" (without quotes).</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
3
3 1 2 3
3 2 3 1
4 2 3 4 5

2
2 1 2
2 5 8

0

<b><tt>Sample output:</tt></b>
12
NEVER
</pre>