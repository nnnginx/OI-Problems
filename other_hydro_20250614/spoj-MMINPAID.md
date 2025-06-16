<p>A network of <strong>m</strong> roads connects <strong>N</strong> cities (numbered from 1 to <strong>N</strong>). There may be more than one road connecting one city with another. Some of the roads are paid. There are two ways to pay for travel on a paid road <strong>i</strong> from city <strong>a<sub>i</sub></strong> to city <strong>b<sub>i</sub></strong>:</p>
<ul>
<li>in advance, in a city <strong>c<sub>i</sub></strong> (which may or may not be the same as <strong>a<sub>i</sub></strong>);</li>
<li>after the travel, in the city <strong>b<sub>i</sub></strong>.   The payment is <strong>P<sub>i</sub></strong> in the first case and <strong>R<sub>i</sub></strong> in the second case.  Write a program to find a minimal-cost route from the city 1 to the city <strong>N</strong>.</li>
</ul>
<h3>Input</h3>
<pre>The first line of the input contains the values of <strong>N</strong> and <strong>m</strong>. Each of the following <strong>m</strong> lines describes one road by specifying the values of <strong>a<sub>i</sub></strong>, <strong>b<sub>i</sub></strong>, <strong>c<sub>i</sub></strong>, <strong>P<sub>i</sub></strong>, <strong>R<sub>i</sub></strong> (1 ¡Ü i ¡Ü m). Adjacent values on the same line are separated by one or more spaces. All values are integers, 1 ¡Ü m, N ¡Ü 10, 0 ¡Ü Pi, Ri ¡Ü 100, Pi ¡Ü Ri (1 ¡Ü i ¡Ü m). 
</pre>
<h3>Output</h3>
<pre>The first and only line of the output must contain the minimal possible cost of a trip from the city 1 to the city <strong>N</strong>. If the trip is not possible for any reason, the line must contain the word 'impossible'.
</pre>
<h3>Example</h3>
<pre><strong>Input:</strong><br>
4 5<br>1 2 1 10 10<br>2 3 1 30 50<br>3 4 3 80 80<br>2 1 2 10 10<br>1 3 2 10 50</pre>
<pre><strong>Output:</strong><br>
110</pre>