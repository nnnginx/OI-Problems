<p>Ada the Ladybug has just bought a few servers. She is not a programming bug so she needs a server administrator to set everything for her. Yay, she have chosen you to help her. Your first job is simple - the servers are (somehow) connected with wires and you have to find out the number of components they form.</p>
<p>Easy isn't it? Well sadly the servers are raw and nothing is (can be) installed on them (at the moment), so you can only use <strong>bash</strong>.</p>
<h3>Input</h3>
<p>The first line of input containts  <strong>1 ¡Ü N ¡Ü 600, 0 ¡Ü M ¡Ü     600</strong>, the number of servers and the number of wires between them.  The next <strong> M </strong> lines contains two integers <strong>0 ¡Ü a, b &lt; N</strong>, the servers which are connected by wires.</p>
<h3>Output</h3>
<p>Print the number of connected components.</p>
<h3>Example Input</h3>
<pre>6 3
1 2
3 4
5 0
</pre>
<h3>Example Output</h3>
<pre>3
</pre>
<h3>Example Input 2</h3>
<pre>11 9
0 10
1 6
1 8
2 7
2 8
3 4
3 6
4 7
4 10
</pre>
<h3>Example Output 2</h3>
<pre>3
</pre>
<h3>Example Input 3</h3>
<pre>5 2
0 4
1 4
</pre>
<h3>Example Output 3</h3>
<pre>3
</pre>
<h3>Example Input 4</h3>
<pre>5 1
1 2
</pre>
<h3>Example Output 4</h3>
<pre>4
</pre>
<h3>Example Input 5</h3>
<pre>4 2
1 3
0 2
</pre>
<h3>Example Output 5</h3>
<pre>2
</pre>