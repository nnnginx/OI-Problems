<p>Given two vectors, a = ( x<sub>a</sub>, y<sub>a</sub> ), b = ( x<sub>b</sub>, y<sub>b</sub> ), their dot product is defined as follows:<br>dp( a, b ) = x<sub>a</sub>*x<sub>b</sub> + y<sub>a</sub>*y<sub>b</sub>.<br><br>Given N vectors in the plane, find a pair for each of them (among those given in the input) such that the dot product of the vector and its pair is maximal. You may pair a vector with itself too.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer N ( 1 &lt;= N &lt;= 200000 ).<br>Each of the next N lines contain a pair of real numbers, x<sub>i</sub> and y<sub>i </sub>(0 &lt;= |x<sub>i</sub>|, |y<sub>i</sub>| &lt;= 100000)<sub>,</sub> representing the i-th vector. x<sub>i</sub> and y<sub>i</sub> will be rounded to 3 decimal places.</p>
<h3>Output</h3>
<p>Output N lines, i-th one containing the maximal dot product for the i-th vector from the input rounded to 3 decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br><br>4<br>0.000 1.000<br>0.000 2.000<br>1.000 1.000<br>0.000 0.000<br><br><strong>Output:<br></strong>&nbsp;<br>2.000<br>4.000<br>2.000<br>0.000<br><br></pre>
<p><strong>Explanation: </strong>Pair the first vector with the second, the second with itself, third with itself or with the second, and the last one with any of them.</p>