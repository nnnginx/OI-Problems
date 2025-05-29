<p>As you might already know, Ada the Ladybug is a farmer. She decided to plant two similar rows of of tulips. She bought <strong>2*N</strong> seeds of <strong>L</strong> different colors and planted them (in both rows) in such way, that the tulip of some color was <strong>L</strong> units far from nearest tulip of the same color. As Ada is also a mathematician, she gave you a more formal description: The <strong>i<sup>th</sup></strong> position had colod <strong>i % L</strong> (where % stands for modulo).</p>
<p>Even though she tried hard, she didn't expect the power of nature. A hurricane appeared and permuted the seeds in both rows (each seed remained in the same row, but got possibly different possition in it). Now the tulips grew but the rows doesn't have the same sequences of colors.</p>
<p>Ada doesn't like that, so she wants to rip off the least number of tulips so that both rows will have same sequence of colors.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong> 1 ¡Ü T ¡Ü 1000</strong>, the number of test-cases.</p>
<p>Each of the next <strong>T</strong> test-cases begins with two integers: <strong>N, L</strong> (<strong>1 ¡Ü L     ¡Ü  N ¡Ü 2*10<sup>5</sup></strong>), the number of tulips and the number of colors.</p>
<p>Each of next <strong>2</strong> lines will contain <strong>N</strong> integers  <strong>0¡Ü     A<sub>i</sub> &lt; L</strong>, the colors of tulips.</p>
<p>As ada likes diversity, so she also assures you that <strong>N/L</strong> (integer division) won't exceed <strong>100</strong>.</p>
<p>The sum of <strong>N</strong> over all test-cases won't exceed <strong>10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>For each test-case output the minimal number of tulips, which has to be ripped to achieve same sequences</p>
<h3>Example Input</h3>
<pre>4
4 4
1 2 3 0
0 3 2 1
5 2
0 1 1 0 0
1 1 0 0 0
3 1
0 0 0
0 0 0
6 3
0 0 1 2 2 1
1 2 0 2 0 1

</pre>
<h3>Example Output</h3>
<pre>6
2
0
4


</pre>