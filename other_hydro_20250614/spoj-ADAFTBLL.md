<p>Ada the Ladybug has many friends who live on a <a href="https://en.wikipedia.org/wiki/Tree_(data_structure)">tree</a>. Each of them is fan of a football team. Ada sometime go on a trip from one friend to another. If she meets a friend she tells him/her about all previously visited friends who are fans of the same team. The visited friend will gain <strong>+1</strong> happiness for each friend Ada told him/her about.</p>
<p>Ada is wondering (for each trip) what will be the total gaines happiness.</p>
<p>Also note that sometime a friend changes his/her mind and start to support different team.</p>
<h3>Input</h3>
<p>The first line two integers <strong>1 ¡Ü N Q ¡Ü     10<sup>5</sup></strong>, the number of friends (<strong>N</strong>) and the number of queries.</p>
<p>The next line will contain <strong>N</strong> integers <strong>0¡Ü A<sub>i</sub> ¡Ü     10<sup>5</sup></strong>, the team which <strong>i<sup>th</sup></strong> friend supports.</p>
<p>The next <strong>N-1</strong> lines will contain two integers <strong>0 ¡Ü a, b &lt;     N</strong>, the friends which will be connected by a branch (edge).</p>
<p>The next <strong>Q</strong> lines will be of two kinds:</p>
<p><strong>1 x y</strong> (<strong>0 ¡Ü x &lt; N</strong>, <strong>0 ¡Ü y ¡Ü 10<sup>5</sup></strong>),         meaning that <strong>x<sup>th</sup></strong> friend will start supporting team         <strong>y</strong> (instead of the old one).</p>
<p><strong>2 a b</strong> (<strong>0 ¡Ü a, b &lt; N</strong>), meaning that Ada will travel from friend <strong>a</strong> to friend <strong>b</strong> and wants to know the happiness.</p>
<h3>Output</h3>
<p>For each query of second kind, output the gained happiness.</p>
<h3>Example Input</h3>
<pre>7 8
0 0 1 2 1 1 2
0 1
1 5
1 2
2 4
2 3
3 6
2 4 5
2 0 6
2 1 3
1 1 2
1 2 2
2 4 5
2 0 6
2 1 3
</pre>
<h3>Example Output</h3>
<pre>3
2
0
2
6
3
</pre>