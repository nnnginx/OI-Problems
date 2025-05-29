<p>Two girls - Ivica and Marica - play an interesting game.</p>
<p>First, they randomly choose a natural number N. They also define M = 1.</p>
<p>Ivica plays first, then Marica, then Ivica, then Marica and so on.</p>
<p>In each move, a girl has to increase M by 1 or multiply M by 2 (that is, M = M+1 or M = 2*M). The resulting number <strong>must not be greater than N</strong>.</p>
<p>The <strong>loser</strong> of the game is the girl who gets M = N. The other girl is, of course, the winner.</p>
<p>Write a program to determine the winner, assuming that both girls play optimally.</p>
<h3>Input</h3>
<p>In the first line there is an integer T (1 ¡Ü&nbsp;T ¡Ü 5), the number of games.</p>
<p>T lines follow. In i<sup>th</sup> line there is an integer N (2 ¡Ü N ¡Ü 10<sup>15)</sup>, a chosen number for i<sup>th</sup>&nbsp;game.</p>
<h3>Output</h3>
<p>For each of the T games print the name of the winner.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>4<br>2<br>3<br>4<br>5<br></pre>
<pre><strong>Output:</strong><br><br>Marica<br>Ivica<br>Marica<br>Marica</pre>