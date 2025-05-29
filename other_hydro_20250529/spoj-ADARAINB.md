<p>As you might <a href="http://www.spoj.com/problems/ADARAIN/">already     know</a> , Ada the Ladybug is growing plants. She used to have a very long furrow, yet it costs a fortune to fence it. To reduce it, she has decided to build a square field. It is so big, that most of water falling from rains drops just onto a rectangular part of the field. Ada doesn't want the plants to wither, so she records all rains to know, how much water every particular plant got. Sadly, there are so many rains that she couldn't handle this alone!</p>
<p>At first, you will be given <strong>N</strong> queries with <strong>[x,y],[X,Y]</strong> rectangles telling you, where all of the <strong>N</strong> rains has fallen (lower left / upper right corners of it). Afterward <strong>M</strong> queries follow, with number <strong>i</strong> - the i-th plant for which you want to know, the number of rains, which has fallen onto it.</p>
<h3>Input</h3>
<p>The first line will contain <strong>0&lt; N,M ¡Ü 3*10<sup>5</sup></strong>,<strong>0&lt; L     ¡Ü 5000</strong>, number of rains, number of questions and size of square field.</p>
<p>Then <strong>N</strong> lines follow, each containing four integers <strong>x, y, X, Y</strong>( <strong>1 ¡Ü x ¡Ü X ¡Ü L, 1 ¡Ü y ¡Ü Y ¡Ü L </strong>), bottom-left and upper-right corner of rectangle where i<sup>th</sup> rain has fallen.</p>
<p>Afterward <strong>M</strong> lines follow, each containing two numbers <strong>1 ¡Ü x, y ¡Ü L</strong>, asking for number of rains which has fallen onto plant on coordinates <strong>[x,y]</strong></p>
<h3>Output</h3>
<p>Print <strong>M</strong> lines (for each query of second type), with integer indicating number of rains, which has fallen onto the plant in query.</p>
<h3>Example Input</h3>
<pre>6 16 4
1 1 3 4
1 1 3 3
2 2 2 2
4 2 4 3
3 3 4 4
1 2 2 4
1 1
1 2
1 3
1 4
2 1 
2 2
2 3
2 4
3 1
3 2
3 3
3 4
4 1
4 2
4 3
4 4
</pre>
<h3>Example Output</h3>
<pre>2
3
3
2
2
4
3
2
2
2
3
2
0
1
2
1
</pre>