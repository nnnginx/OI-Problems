<p>Ada the Ladybug is visiting her friends who live on a plum <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. As
many bugs like her, she has a friend in each node. She has already planed in
which order she will visit them. She does that in following manner. If she is
standing at a node <b>i</b> in the morning, she will choose shortest path to
friend with number <b>i+1</b>. Afterward, she stays there until next morning.
First day she "magically" apears on node number
<b>1</b> and as she arrives at node <b>N</b>, she ends her journey. Your task
is to find (for each node), the number of days she visited it (this means she
either begins in it, ends in it or passes through it).


</p><h3>Input</h3>

The first line contains <b>1 ¡Ü N ¡Ü 4*10<sup>5</sup> </b>, number
of nodes on tree.

<p>Each of next <b>N-1</b> lines contains two integers <b>1 ¡Ü I, J ¡Ü
    N</b>, <b>I ¡Ù J</b>, the nodes which are connected by an edge.

</p><h3>Output</h3>
Print <b>N</b> lines with and integer indicating number of times
<b>i<sup>th</sup></b> node was visited.

<h3>Example Input</h3>
<pre>5
1 2
2 5
2 4
5 3
</pre>
<h3>Example Output</h3>
<pre>1
4
2
2
3
</pre>
<h3>Example Input 2</h3>
<pre>10
1 3
1 5
5 2
5 9
9 7
9 10
6 2
4 2
8 4
</pre>
<h3>Example Output 2</h3>
<pre>3
8
2
4
8
2
2
2
4
1
</pre>