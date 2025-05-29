<p>Given the value of N, you will have to find the value of G. The meaning of G is given in the following code </p>

<p>
</p><pre>G = 0;
for (i = 1; i &lt; N; i++)
  for (j = i+1; j &lt;= N; j++) 
    G += gcd(i, j);
</pre>
Here gcd() is a function that finds the greatest common divisor of the two input numbers.
<p></p>

<h3>Input</h3>
<p>The input file contains at most 20000 lines of inputs. Each line contains an integer N (1 &lt; N &lt; 1000001). The meaning of N is given in the problem statement. Input is terminated by a line containing a single zero.  </p>

<h3>Output</h3>
<p>For each line of input produce one line of output. This line contains the value of G for the corresponding N. The value of G will fit in a 64-bit signed integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
10
100
200000
0

<b>Output:</b>
67
13015
143295493160

Time limit has been changed. Some AC solutions get TLE
</pre>