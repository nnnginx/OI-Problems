<p>The Fibonacci sequence is defined by : <em>f<sub>n</sub></em> = <em>n</em> for <em>n</em> &lt; 2, and <em>f<sub>n</sub></em> = <em>f<sub>n-1</sub></em> + <em>f<sub>n-2</sub></em> for <em>n</em> &gt; 1. <br>
<em>f</em> = (0, 1, 1, 2, 3, 5, 8, ...)<br>

You have to count how many terms are divisible by a given integer in the beginning of the sequence.

</p><h3>Input</h3>
<p>The first line of input contains one integer:
 <em>T</em> the number of test cases.<br>
On each of the next <em>T</em> lines, your are given
three integers: <em>a</em>, <em>b</em>, and <em>k</em>.
</p>

<h3>Output</h3>
<p>
For each test case, you have to print the number of term <em>f<sub>n</sub></em> that are divisible by <em>k</em>, for <em>n</em> in [0..<em>a</em><em><sup>b</sup></em>].<br>
As the result may be a big number, simply output your result modulo 10<sup>9</sup>+7

</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
3 2 3
2 3 8
9 1 6


<b>Output:</b>
3
2
1
</pre>

<p>Explanation: For the first case, <em>a</em><em><sup>b</sup></em> = 3<sup>2</sup> = 9, and the terms with rank 0 to 9 are : <b>0</b>, 1, 1, 2, <b>3</b>, 5, 8, 13, <b>21</b>, 34.<br>
There are <b>3</b> numbers divisible by <em>k</em>=3.</p>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^4
0 &lt; a &lt; 10^18
0 &lt; b &lt; 10^18
1 &lt; k &lt; 10^18
</pre>
<p>To give more interest in the best part of the problem,
you can assume that the maximum prime factor of <em>k</em> is less than or equal to 10<sup>6</sup>.<br>
Time limit is approx 4x the time for my 1.4kB PY3.4 submission (based on my old code for problem ??? you should find).<br>
<b>Good luck, and have fun ;-)</b>
</p>
<p>
 Edit(2017-02-11) : New time limit (after compiler changes). 
</p>