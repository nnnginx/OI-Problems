<p><b>A much easier version of this problem can be found here-<a href="http://www.spoj.com/problems/SUMDEC1/">SUMDEC1</a>.<br>In case you haven't tried it out,try the first part.</b></p>
<p>In this problem,You are given a number.You need to output the sum of the first 1000 decimal places of the square-root of the number(Ignore the Integral part).<br>
</p><p>For example-if the given number is 2. The square-root of 2 is 1.4142135623.....<br>
So,ignore the number before decimal (1 in this case) and add the first 1000 digits after decimal and output them as result-4482.(in this case)<br></p>
<b>NOTE-If the number is a perfect square,the output should be 0.</b>


<h3>Input</h3>
<p>the first line of input consist of t (the number of test cases).<br>
t lines follow-Each line consist of a non-negative integer n.

</p><h3>Output</h3>
<p>Output in seperate lines the result corresponding to integer n.

</p><h4>Constraints</h4>
1&lt;=t&lt;=100<br>
1&lt;=n&lt;=100000

<h3>Example</h3>

<pre><b>Input:</b>
2
4
2

<b>Output:</b>
0
4482
</pre>