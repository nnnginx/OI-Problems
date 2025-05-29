<p>Ada the Ladybug is cultivating vegetables. She has a long furrow full of different kinds of it and she wants to know the number of unique vegetables on a segment of the furrow. As the cultivation is a dynamic process, a kind (on a single position) might become another kind during this process.</p>
<p>Given furrow and a few updates, can you answer questions asking about number of unique kinds of vegetable on a segment?</p>

<h3>Input</h3>
<p>The first line contains <strong>1 ¡Ü N, Q ¡Ü 2*10<sup>5</sup> </strong>, length of furrow and number of queries.</p>
<p>Next line contains <strong>N</strong> integers <strong>0 ¡Ü A<sub>i</sub> ¡Ü     2*10<sup>5</sup></strong>, the kind of <strong>i<sup>th</sup></strong> vegetable</p>
<p>Each of following <strong>Q</strong> lines contains one of the following kinds of query:</p>
<p><em>1 I V</em>: The vegetable on index <strong> 0 ¡Ü I &lt; N</strong>, will be changed to kind <strong> 0 ¡Ü A     ¡Ü 2*10<sup>5</sup></strong></p>
<p><em>2 L R</em>: <strong> 0 ¡Ü L ¡Ü R &lt; N </strong>, the index of left/right bound of segment for which you want to know the number of unique kinds.</p>
<h3>Output</h3>
<p>For each query of second kind, print the number of unique kinds of vegetable.</p>
<h3>Example Input</h3>
<pre>8 8
1 2 3 3 1 2 3 3
2 1 3
2 0 3 
2 0 7
1 3 4
1 7 0
2 1 3
2 0 3 
2 0 7
</pre>
<h3>Example Output</h3>
<pre>1
2
0
3
4
2
</pre>